{
  "version": 2,
  "builds": [
    {
      "src": "cupcake-backend/server.js",
      "use": "@vercel/node"
    }
  ],
  "routes": [
    {
      "src": "/api/(.*)",
      "dest": "/cupcake-backend/server.js"
    }
  ]
}
