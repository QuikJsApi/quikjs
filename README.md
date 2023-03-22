# QuikJS

QuikJS is an easy-to-use API framework based on Express.js, designed to follow design patterns like Convention over Configuration, Don't Repeat Yourself, and Fat Model Thin Controller. The framework also utilizes environment-based configurations and a separate database schema with a migration system.

## Getting Started

1. Clone the repository:

```bash
  git clone https://github.com/yourusername/quikjs.git
```

2. Install dependencies:

```bash
cd quikjs
npm install
```

3. Set up your environment:

- Copy `config/environments/development.js` to `config/environments/local.js`.
- Update `local.js` with your MongoDB URI and other local settings.
- Add `local.js` to `.gitignore` to avoid committing sensitive information.

4. Run the application in development mode:

```bash
NODE_ENV=local node app.js
```

5. Run migrations:

```bash
  NODE_ENV=local ./migration.js up
```

6. Access the API at `http://localhost:3000/api/example`.

## License

[MIT License](https://opensource.org/licenses/MIT)
