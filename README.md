# NxRemixDocker

```sh
❯ npx create-nx-workspace@latest --ci skip nx-remix-docker
 NX   Let's create a new workspace [https://nx.dev/getting-started/intro]
✔ Which stack do you want to use? · none
✔ Package-based monorepo, integrated monorepo, or standalone project? · integrated

❯ npm i -D @nx/remix
❯ npx nx g @nx/remix:application --help

 NX   generate @nx/remix:application [name] [options,...]


From:  @nx/remix (v19.1.0)
Name:  application (aliases: app)


  Generate a new Remix application.


Options:
    --directory, -dir             A directory where the app is placed.                                          [string]
    --e2eTestRunner               Test runner to use for e2e tests           [string] [choices: "playwright", "cypress",
                                                                                         "none"] [default: "playwright"]
    --js                          Generate JavaScript files rather than                                        [boolean]
                                  TypeScript files.
    --linter                      The tool to use for running lint checks.          [string] [choices: "eslint", "none"]
                                                                                                     [default: "eslint"]
    --name                                                                                                      [string]
    --projectNameAndRootFormat    Whether to generate the project name and             [string] [choices: "as-provided",
                                  root directory as provided (`as-provided`)                                  "derived"]
                                  or generate them composing their values and
                                  taking the configured layout into account
                                  (`derived`).
    --skipFormat                  Skip formatting files                                                        [boolean]
    --tags, -t                    Add tags to the project (used for linting)                                    [string]
    --unitTestRunner              Test runner to use for unit tests.                [string] [choices: "vitest", "jest",
                                                                                             "none"] [default: "vitest"]
    --rootProject                 undefined                                                                    [boolean]



Find more information and examples at: https://nx.dev/packages/remix/generators/application


❯ npx nx g @nx/remix:application \
  --directory apps/remix-app \
  --name remix-app \
  --projectNameAndRootFormat as-provided \
  --unitTestRunner vitest \
  --e2eTestRunner playwright
```
