## Next.js Marketplace

Now updated to connect to the new dashboard and [Cosmic JavaScript SDK](https://www.npmjs.com/package/@cosmicjs/sdk). [Read the article](https://www.cosmicjs.com/blog/4-steps-to-update-the-nextjs-marketplace-template) to learn about the latest updates.

The Next.js Marketplace is a template that you can use to start your own digital art marketplace. Download for free.

![Cosmic uNFT](https://user-images.githubusercontent.com/1950722/178328933-c6f0008f-a188-4678-9420-404dd1f02871.gif)

## Technology used

This template uses the following technologies:

- [Next.js](https://nextjs.org/) - scalable and high-performance **React.js** framework for modern web development. Provides a large set of features, such as hybrid rendering, route prefetching, automatic image optimization, and internationalization, out of the box.
- [Cosmic](https://www.cosmicjs.com/) - fast, fully managed [headless CMS](https://www.cosmicjs.com/headless-cms) that enables us to quickly manage and create website content including UGC (user-generated content).
- [Stripe](https://stripe.com/) - payments infrastructure that provides API tools to receive one-time and subscription payments.

### Links

- [View the live demo](https://c-marketplace-cosmicjs.vercel.app/)
- [Install the template](https://www.cosmicjs.com/marketplace/templates/nextjs-marketplace)
- [Read how it was built](https://www.cosmicjs.com/articles/build-a-digital-art-marketplace-with-nextjs-cosmic-and-stripe)

## Getting started

1. First, install the [template](https://www.cosmicjs.com/marketplace/templates/unft-marketplace) into your Cosmic account to get the demo content ready.
2. Then download and install the code on your machine.

```bash
git clone https://github.com/cosmicjs/unft-marketplace
cd unft-marketplace
pnpm install
# or
yarn
# or
npm install
```

### Environment variables

You'll need to create a `.env` file in the root of the project and add the access keys for Cosmic and Stripe. This can be done by copying the `.env.example`.

```bash
cp .env.example .env
```

**Cosmic**: Go to [Cosmic](https://app.cosmicjs.com/) and from the Bucket that you installed the app template go to _Bucket Settings > API Access_ and get your API access keys.

**Stripe**: Log in to [Stripe](https://dashboard.stripe.com/) and get your keys in the **for developers** section.

Add your keys to the `.env` file like so:

```bash
# .env
NEXT_PUBLIC_COSMIC_BUCKET_SLUG=your_cosmic_slug
NEXT_PUBLIC_COSMIC_READ_KEY=your_cosmic_read_key
COSMIC_WRITE_KEY=your_cosmic_write_key

NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=your_stripe_key
STRIPE_SECRET_KEY=your_stripe_secret_key
```

### Then run the development server

```bash
pnpm dev
# OR
yarn dev
# OR
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Deploy on Vercel

<p>Use the following button to deploy to <a href="https://vercel.com/" rel="noopener noreferrer" target="_blank">Vercel</a>. You will need to add your environment variables before deployment.</p>
<p>
<a href="https://vercel.com/import/git?c=1&s=https://github.com/cosmicjs/unft-marketplace&env=NEXT_PUBLIC_COSMIC_BUCKET_SLUG,NEXT_PUBLIC_COSMIC_READ_KEY,COSMIC_WRITE_KEY,NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY,STRIPE_SECRET_KEY&envDescription=Required%20to%20connect%20the%20app%20with%20Cosmic&envLink=https://vercel.link/cms-cosmic-env" rel="noopener noreferrer" target="_blank"><img src="https://cdn.cosmicjs.com/d3f0d5e0-c064-11ea-9a05-6f8a16b0b14c-deploy-to-vercel.svg" style="width: 100px;" class="fr-fic fr-dib fr-fil"></a>
</p>

Check out the [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.

## License

This project is published under the [MIT](LICENSE) license.
