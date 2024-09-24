This is the output of the platformatic CLI:

```
$ pnpm create platformatic@latest
 Hello oshox, welcome to Platformatic 1.53.3!
? What kind of project do you want to create? Application
? Where would you like to create your project? platformatic-error
✔ Installing @platformatic/runtime...
? Which kind of project do you want to create? @platformatic/db
✔ Installing @platformatic/db...
? What is the name of the service? platformatic-db-error
? What is the connection string? postgresql://postgres:postgres@localhost:5432/postgres
? Do you want to create default migrations? no
? Do you want to create another service? no
? Do you want to use TypeScript? yes
? What port do you want to use? 3042
[23:13:35] INFO: /home/oshox/platformatic-error/package.json written!
[23:13:35] INFO: /home/oshox/platformatic-error/platformatic.json written!
[23:13:35] INFO: /home/oshox/platformatic-error/.env written!
[23:13:35] INFO: /home/oshox/platformatic-error/.env.sample written!
[23:13:35] INFO: /home/oshox/platformatic-error/tsconfig.json written!
[23:13:35] INFO: /home/oshox/platformatic-error/.gitignore written!
[23:13:35] INFO: /home/oshox/platformatic-error/README.md written!
[23:13:35] INFO: /home/oshox/platformatic-error/services/platformatic-db-error/package.json written!
[23:13:35] INFO: /home/oshox/platformatic-error/services/platformatic-db-error/platformatic.json written!
[23:13:35] INFO: /home/oshox/platformatic-error/services/platformatic-db-error/tsconfig.json written!
[23:13:35] INFO: /home/oshox/platformatic-error/services/platformatic-db-error/plugins/example.ts written!
[23:13:35] INFO: /home/oshox/platformatic-error/services/platformatic-db-error/routes/root.ts written!
[23:13:35] INFO: /home/oshox/platformatic-error/services/platformatic-db-error/test/helper.ts written!
[23:13:35] INFO: /home/oshox/platformatic-error/services/platformatic-db-error/test/plugins/example.test.ts written!
[23:13:35] INFO: /home/oshox/platformatic-error/services/platformatic-db-error/test/routes/root.test.ts written!
[23:13:35] INFO: /home/oshox/platformatic-error/services/platformatic-db-error/.gitignore written!
[23:13:35] INFO: /home/oshox/platformatic-error/services/platformatic-db-error/README.md written!
[23:13:35] INFO: /home/oshox/platformatic-error/services/platformatic-db-error/global.d.ts written!
? Do you want to init the git repository? yes
[23:13:37] INFO: Git repository initialized.
✔ Installing dependencies...
[23:13:40] INFO: Project created successfully, executing post-install actions...
[23:13:40] INFO: You are all set! Run `npm start` to start your project.
```

I have committed my .env file to show it did not get created with the correct values.
To get the app to start from here, I need to manually:
1. Create the folder `./services/platformatic-db-error/migrations`
1. Update the .env to the correct connection string
