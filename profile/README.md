<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./logo-dark.svg">
  <img src="./logo.svg" alt="Momobase" width="72">
</picture>

# Momobase

**Payment infrastructure you control.**
<br>
One self-hosted API for collections, disbursements, routing, provider health, and reconciliation.

[![Container](https://img.shields.io/badge/ghcr.io-momobasehq%2Fserver-2496ed?logo=docker&logoColor=white)](https://github.com/momobasehq/server/pkgs/container/server)
[![Go Reference](https://pkg.go.dev/badge/github.com/momobasehq/momobase.svg)](https://pkg.go.dev/github.com/momobasehq/momobase)
[![npm](https://img.shields.io/npm/v/momobase?label=sdk&logo=npm)](https://www.npmjs.com/package/momobase)
[![Server](https://img.shields.io/github/v/release/momobasehq/server?label=server)](https://github.com/momobasehq/server/releases/latest)
[![library](https://img.shields.io/github/v/release/momobasehq/momobase?label=library)](https://github.com/momobasehq/momobase/releases/latest)

[![Docs](https://img.shields.io/badge/docs-momobasehq.github.io-informational)](https://momobasehq.github.io/)
[![License](https://img.shields.io/badge/license-MIT-blue)](https://github.com/momobasehq/server/blob/main/LICENSE.txt)

</div>

## Why?

Several developers and organizations manage many payment providers for their apps, each provider with its own interface. When one payment provider is down or slow, your apps are down and affected. Migrating from one provider to another is a hustle as well. That's why we built Momobase so that you manage all your apps' payments in one place, switch providers seamlessly on the fly.  

Applications get one payment contract. Provider adapters absorb the credentials, payloads, and status models behind it. Run it as a server or compile it into your own Go program — both are the same engine.

## Get started

1. **Server** 
  
    The HTTP API, its provider adapters, and an admin dashboard in one process.

    ```sh
    docker run -p 9090:9090 -v momobase-data:/data ghcr.io/momobasehq/server
    ```

    [Releases](https://github.com/momobasehq/server/releases/latest) · [Install guide](https://momobasehq.github.io/server/install) · [Repo](https://github.com/momobasehq/server)

<br>

2. **Go library** 

    Embed the engine to compile in your own adapters, hooks, and routes.

    ```sh
    go get github.com/momobasehq/momobase
    ```

    [pkg.go.dev](https://pkg.go.dev/github.com/momobasehq/momobase) · [Docs](https://momobasehq.github.io/library/) · [Repo](https://github.com/momobasehq/momobase)

<br>

3. **TypeScript SDK**
    
    A dependency-free client, token refresh handled for you.

    ```sh
    npm install momobase
    ```

    [npm](https://www.npmjs.com/package/momobase) · [Docs](https://momobasehq.github.io/sdk/) · [Repo](https://github.com/momobasehq/sdk)

<br>

>Not sure which? [Compare the server and the library](https://momobasehq.github.io/guide/choose).
