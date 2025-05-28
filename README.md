
# Omni Stack

Omni Stack provides a unified approach to monitoring and accessing information sets and information flows across the entire digital landscape. It is a data integration platform designed to connect, monitor, and analyse data sets and information flows from diverse sources in real-time, with out-of-the-box integrations for hundreds of popular applications, databases, cloud services, and data streams, whilst offering advanced monitoring capabilities to ensure all connections are operational and healthy.

<!-- ![Omni Stack Dashboard](https://raw.githubusercontent.com/econic-ai/omni-stack/main/docs/images/dashboard-preview.png) -->

Omni Stack is open source, however running and maintaining your own deployment can be cumbersome and cost prohibitive. Leverage our SaaS and managed solutions to reduce costs and gain access to advanced features.

| Feature | Open Source | SaaS | Enterprise |
|---------|-------------|------|------------|
| **Core Integrations** | ✅ | ✅ | ✅ |
| **Real-time Monitoring** | ✅ | ✅ | ✅ |
| **Basic Analytics** | ✅ | ✅ | ✅ |
| **Community Support** | ✅ | ✅ | ✅ |
| **Self-hosted** | ✅ | ❌ | ✅ |
| **Managed Infrastructure** | ❌ | ✅ | ✅ |
| **Advanced Analytics** | ❌ | ✅ | ✅ |
| **Premium Integrations** | ❌ | ✅ | ✅ |
| **Priority Support** | ❌ | ✅ | ✅ |
| **Custom Integrations** | ❌ | ❌ | ✅ |
| **On-premise Deployment** | ✅ | ❌ | ✅ |
| **SSO & Advanced Security** | ❌ | ❌ | ✅ |
| **SLA Guarantees** | ❌ | ✅ | ✅ |
| **White-label Options** | ❌ | ❌ | ✅ |

### SaaS Platform
Get started immediately with our fully managed cloud platform.

<a href="/docs/technology/ai-models/why-graphs" class="__link small sk-mt-12 sk-mb-12" style="text-decoration: none;">
    <span>Try Our SaaS</span>
    <!-- <i class="fa-solid fa-arrow-right"></i> -->
</a>

### Enterprise Solutions
Custom deployments, integrations, and support for large organisations.

<a href="/flow/register" class="__link small sk-mt-12 sk-mb-12 " style="text-decoration: none;">
    <span>Enterprise Sales</span>
    <!-- <i class="fa-solid fa-arrow-right"></i> -->
</a>



## Quick Start

### Docker (Recommended)

```bash
# Pull and run the latest version
docker run -d \
  --name omni-stack \
  -p 3000:3000 \
  -p 8080:8080 \
  -v omni-data:/app/data \
  econicai/omni-stack:latest

# Access the dashboard at http://localhost:3000
```

### Build from Source

```bash
# Clone the repository
git clone https://github.com/econic-ai/omni-stack.git
cd omni-stack

# Install dependencies
npm install

# Configure environment
cp .env.example .env
# Edit .env with your configuration

# Build and start
npm run build
npm start
```

### Environment Variables

```bash
# Database
DATABASE_URL=postgresql://user:password@localhost:5432/omnistack

# Redis (for caching and queues)
REDIS_URL=redis://localhost:6379

# Application
PORT=3000
NODE_ENV=production

# Authentication (optional)
JWT_SECRET=your-secret-key
OAUTH_GOOGLE_CLIENT_ID=your-google-client-id
OAUTH_GOOGLE_CLIENT_SECRET=your-google-client-secret
```

### Custom Integrations

```javascript
// config/integrations.js
module.exports = {
  gmail: {
    enabled: true,
    credentials: {
      clientId: process.env.GOOGLE_CLIENT_ID,
      clientSecret: process.env.GOOGLE_CLIENT_SECRET
    }
  }
}
```

## Progress of Integrations


| Integraiton | Status |
|-------------|-------------|
| **Google** | |
| - Gmail | ✅ |
| - Google Calendar | 🔄 | 
| - Google Drive | 📋 |
| - Google Docs | 📋 |
| **Microsoft** | |
| - Outlook | 📋 |
| - Teams | 📋 |
| - OneDrive | 📋 |
| **Messaging** | |
| - Slack | 📋 |
| - Discord | 📋 |
| - WhatsApp | 📋 |
| - Messenger | 📋 |
| - Twilio | 📋 |
| **Cloud Services** | |
| - AWS S3 | 📋 |
| - Azure Blob Storage | 📋 |
| - vGoogle Cloud Storage | 📋 |
| - Dropbox | 📋 |
| **Databases** | |
| - PostgreSQL | 📋 |
| - MySQL | 📋 |
| - Redis | 📋 |
| **Business Applications** | |
| - Salesforce | 📋 |
| - HubSpot | 📋 |
| - Notion | 📋 |
| **Developer Tools** | |
| - GitHub | 📋 |
| - Jira | 📋 |
| - Vercel | 📋 |

**Legend:** ✅ Complete | 🔄 In Progress | 📋 Planned

### Request an Integration

Which integrations is of most valuable to you? We are actively prioritising the list.

## Development Roadmap

We are in the early stages of Omni Stack development and are actively shaping its roadmap based on community feedback and enterprise requirements.

### 1. **Phase 1** (Q2-Q3 2025)
   * Core integration engine
   * Universal data model implementation
   * Real-time monitoring dashboard
   * Initial integration suite (Google, Microsoft, Databases)
   * REST API framework
   * Containerisation

### 2. **Phase 2** (Q3-Q4 2025)
   * Event-driven architecture
   * Semantic search across all data sources
   * Advanced monitoring and alerting system  
   * Enterprise authentication (SSO, LDAP)

### 3. **Phase 3** (Q1-Q2 2026)
   * Advanced analytics
   * Multi-tenant architecture
   * White-label
   * Marketplace


## Support and Contributions

- **Community:** [GitHub Discussions](https://github.com/econic-ai/omni-stack/discussions)
- **Issues:** [GitHub Issues](https://github.com/econic-ai/omni-stack/issues)

We welcome contributions! Please see our [Contributing Guide](CONTRIBUTING.md) for details.

## License

Apache 2.0 - see [LICENSE](LICENSE) for details.

---

*Part of the [Econic AI](https://econic.ai) technology stack*