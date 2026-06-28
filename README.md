# e-plantShopping

**Paradise Nursery — E-Plant Shopping**

> Repository: **e-plantShopping**

A single-page plant shopping cart application for **Paradise Nursery**, _"Where Green Meets Serenity."_ Browse a catalog of houseplants organized by category, add them to a cart, and manage quantities — all powered by React and Redux Toolkit.

## Features

- **Landing page** with a "Get Started" call-to-action and an About Us section.
- **Product catalog** grouped into categories such as Air Purifying, Aromatic Fragrant, Insect Repellent, Medicinal, and Low Maintenance plants.
- **Shopping cart** with add-to-cart, remove, and quantity update actions, plus running totals.
- **Global state** managed with Redux Toolkit (`cart` slice).

## Tech Stack

- [React 18](https://react.dev/)
- [Redux Toolkit](https://redux-toolkit.js.org/) + [React Redux](https://react-redux.js.org/)
- [Vite](https://vitejs.dev/) for development and bundling
- ESLint for linting

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (LTS recommended)
- npm

### Installation

```bash
npm install
```

### Development

Start the local dev server with hot reloading:

```bash
npm run dev
```

### Build

Create a production build in the `dist/` directory:

```bash
npm run build
```

### Preview

Build and serve the production bundle locally:

```bash
npm run preview
```

### Lint

```bash
npm run lint
```

## Project Structure

```
src/
├── main.jsx          # App entry point; wires up the Redux Provider
├── App.jsx           # Landing page + product list toggle
├── store.js          # Redux store configuration
├── CartSlice.jsx     # Cart state, reducers, and actions
├── ProductList.jsx   # Plant catalog and category rendering
├── CartItem.jsx      # Individual cart item with quantity controls
├── AboutUs.jsx       # About Us section
└── *.css             # Component styles
```

## Deployment

The project is configured for static deployment via [gh-pages](https://www.npmjs.com/package/gh-pages). Note that `vite.config.js` sets `base: "/shoppingreact"`, so the app expects to be served from that path.

## License

See [LICENSE](LICENSE) for details.
