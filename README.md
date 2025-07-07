
const http = require('http');

const server = http.createServer((req, res) => {
  res.statusCode = 200;
  res.setHeader('Content-Type', 'text/plain');
  res.end('Hello, World!\n');
});

server.listen(4221, () => {
  console.log('Server running on port 4221');
});

// 保持主线程运行（Node.js 会自动保持服务器运行）
