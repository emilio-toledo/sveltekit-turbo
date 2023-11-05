# Sveltekit Turbo

This is a cutting-edge template for creating Sveltekit monorepos using the latest tools available in the ecosystem (propably already outdated). 

## Tools
- [biomejs](https://biomejs.dev/) (replacement for eslint and prettier made in rust)
- [bun.sh](https://bun.sh/) (replacement for nodejs)
- [turborepo](https://turbo.build/repo) (incremental bundler and build system)
- [semantic-release](https://semantic-release.gitbook.io/semantic-release/) (automated version management)

## Prerequisites

Before you begin, ensure you have met the following requirements:

- **Bun**: Make sure you have bun installed on your system. You can download it from [bun.sh](https://bun.sh/).

## Getting Started

To get started with this template, follow these steps:

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/sveltekit-turborepo-template.git
   ```

2. Change into the project directory:

   ```bash
   cd sveltekit-turborepo-template
   ```

3. Install the project dependencies:

   ```bash
   bun install
   ```

4. Start the development server:

   ```bash
   bun dev
   ```

   This will start the the `web` and `docs` development servers.

## Project Structure

This template follows a TurboRepo structure for managing multiple packages within a single repository. Here's a brief overview of the project structure:

- `apps/`: This directory **contains the various applications** within your turborepo. Each app is a complete sveltekit web application.

- `packages/`: This directory **contains the various packages** within your turborepo. In this template, you'll find the package: `ui` (dedicated to shared svelte components).

## Development

1. Create new sveltekit apps in `apps/`

   ```
   bun create svelte@latest my-app
   ```

2. Add your monorepo `packages/` dependencies inside your new apps package.json files

   ```
   "dependencies": {
		"ui": "*"
	},
   ```

3. Enjoy building scalable sveltekit monorepos.

## Versioning and Releases

This template is configured to use Semantic Release for versioning and creating releases. Make sure to follow the commit message conventions outlined in the Semantic Release documentation (made easier with the `bun commit` command).

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

- [SvelteKit](https://kit.svelte.dev/)
- [Biomejs](https://biomejs.dev/)
- [Bun.sh](https://bun.sh/)
- [Semantic Release](https://semantic-release.gitbook.io/semantic-release/)

Enjoy building your SvelteKit application with TurboRepo, Biome.js, Bun.js, and Semantic Release! If you have any questions or need assistance, please refer to the documentation of the respective tools or seek help from the community.