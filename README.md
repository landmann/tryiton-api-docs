# Mintlify Starter Kit

Click on `Use this template` to copy the Mintlify starter kit. The starter kit contains examples including

- Guide pages
- Navigation
- Customizations
- API Reference pages
- Use of popular components

### Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mintlify) to preview the documentation changes locally. To install, use the following command

```
npm i -g mintlify
```

Run the following command at the root of your documentation (where mint.json is)

```
mintlify dev
```

Run the following command to auto fetch all the endpoints and them move them around in the `api-reference` folder

```
npx @mintlify/scraping@latest openapi-file <path-to-openapi-file>
```

### Publishing Changes

Install our Github App to autopropagate changes from youre repo to your deployment. Changes will be deployed to production automatically after pushing to the default branch. Find the link to install on your dashboard. 

#### Troubleshooting

- Mintlify dev isn't running - Run `mintlify install` it'll re-install dependencies.
- Page loads as a 404 - Make sure you are running in a folder with `mint.json`
- If you have issues with "sharp", something I tried (and it worked) was to follow these stackoverflow solutions in order:
- 1. (https://stackoverflow.com/a/67566332)
  2. (https://stackoverflow.com/a/75852216)