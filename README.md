# Dating Backend

A backend service for an international dating app MVP, built with:

- **.NET 8** (ASP.NET Core)
- **SignalR** for real-time messaging
- **SQL Server** (Azure SQL Edge locally, AWS RDS in production)
- **DynamoDB** for high-write chat message storage
- **Auth0** for authentication
- **AWS S3 + FCM** for media and push notifications (planned)

## Features (MVP)

- User registration & profile management
- Preference-based recommendations
- Like/Pass decisions
- Match creation & conversation start
- Real-time chat with SignalR
- Push notifications (planned)

## Local Development

### Prerequisites

- .NET 8 SDK
- Docker (for Azure SQL Edge)
- Azure Data Studio (or any SQL client)
- Auth0 tenant

### Run Locally

```bash
# Start local SQL Server (Azure SQL Edge)
docker run -e "ACCEPT_EULA=1" -e "MSSQL_SA_PASSWORD=YourStrong!Passw0rd" \
  -p 1433:1433 --name sqledge -d mcr.microsoft.com/azure-sql-edge

# Start API
cd src/App.Api
dotnet run
```

## **2. LICENSE file (MIT License)**

**LICENSE**

```text
MIT License

Copyright (c) 2025 monica-ty

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
