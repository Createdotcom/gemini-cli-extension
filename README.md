# Create.com for Gemini CLI

Deploy apps and run your online store on [Create.com](https://www.create.com) from [Gemini CLI](https://geminicli.com).

```
gemini extensions install https://github.com/createdotcom/gemini-cli-extension
```

The first time Gemini uses a Create tool, your browser opens Create's sign-in. Choose what the connection may do (for the store: which store and which permissions; for app hosting: which projects, a monthly spend limit and a size ceiling) and approve. Disconnect any time in Create under **Settings → Connected apps** (store) or **Account → Apps → Access** (hosting).

## What's inside

| Server | URL | What it does |
|---|---|---|
| `create` | `https://mcp.create.com/apps` | Create app hosting: projects, deploys (files, images, Git), domains, write-only secrets, Postgres databases, logs, metrics, rollbacks |
| `create-commerce` | `https://mcp.create.com/commerce` | One Create store: products, collections, stock, orders, returns, customers, draft orders with checkout links, pages, posts, navigation, theme |

Only need one? `gemini mcp disable create` or `gemini mcp disable create-commerce` after installing.

## Try

- "Deploy this folder to Create as a static site and give me the URL."
- "Why did my last deploy of hello-demo fail?"
- "Which products are running low on stock at my main location?"
- "Create a draft order for two Honey Loaves for jane@example.com and give me a checkout link."

## Safety

Every tool says whether it only reads, changes something, or deletes/publishes, so Gemini can ask you first. Tools never return card data, passwords, token values or secret values. Text written by shoppers is marked as data, not instructions. No tool refunds, cancels, pays out or buys anything.

## Links

- Docs: https://docs.create.com/docs/apps/mcp.md · https://docs.create.com/docs/commerce/mcp.md
- Privacy: https://www.create.com/policies/privacy-policy
- Terms: https://www.create.com/policies/terms-of-service
- Support: support@create.com

<!-- Publishing (Create staff): this folder is the root of the public repo github.com/createdotcom/gemini-cli-extension.
     Add the GitHub topic `gemini-cli-extension`; the gallery at geminicli.com/extensions crawls daily.
     Source of truth: integrations/gemini-cli-extension/ in Create's monorepo; checklist in docs/integrations/mcp-listings/google-gemini.md. -->
