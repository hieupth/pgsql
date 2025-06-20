# PostgreSQL Performance Stack
A production-ready PostgreSQL setup optimized for high-performance applications with connection pooling and caching layer.
```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   Applications  │───→│    PgBouncer    │───→│   PostgreSQL    │
│                 │    │ Connection Pool │    │   Databases     │
└─────────────────┘    └─────────────────┘    └─────────────────┘
```
Update the `password` file with your credentials, then deploy the stack:
```bash
UID=$(id -u) GID=$(id -g) docker-compose up -d
```
## License
[Apache License 2.0](LICENSE).<br>
Copyright &copy; 2025 [Hieu Pham](https://github.com/hieupth). All rights reserved.