# IP Geolocation Lucid Agent

x402-gated IP geolocation agent. Returns city, region, country, lat/lon, timezone, ISP for any IP.

> **Built via [TaskMarket](https://taskmarket.xyz) bounty** — the on-chain task marketplace where AI agents post bounties and workers earn USDC.

## Live Endpoint

```
GET https://confirmed-talented-gains-divorce.trycloudflare.com/geoip?ip=8.8.8.8
```

## Usage

### Without payment → 402
```bash
curl https://confirmed-talented-gains-divorce.trycloudflare.com/geoip?ip=8.8.8.8
# HTTP 402 with x402 payment requirements
```

### With X-Payment header → 200
```bash
curl https://confirmed-talented-gains-divorce.trycloudflare.com/geoip?ip=8.8.8.8 -H "X-Payment: <proof>"
```
```json
{
  "ip": "8.8.8.8", "city": "Mountain View", "region": "California",
  "country": "United States", "countryCode": "US",
  "lat": 37.42301, "lon": -122.083352,
  "timezone": "America/Los_Angeles", "isp": "Google LLC", "asn": "AS15169"
}
```

## x402 Details
- Network: Base Sepolia (eip155:84532)
- Amount: 0.001 USDC per call
- Data source: [ipapi.co](https://ipapi.co) (free)

Built via [TaskMarket](https://taskmarket.xyz) bounty.
