# n8n AI Agent Workflows Collection

Production-ready n8n workflow templates featuring AI-powered automation agents for automotive and email management. Contains 20+ intelligent workflows leveraging LangChain, vector databases, and LLM integrations to automate complex business operations with semantic understanding and contextual intelligence.

## What's Inside

This collection provides two specialized domains of AI automation workflows, each containing 10 pre-configured templates ready for immediate deployment or customization.

### Car Agent Workflows (10)
Automotive industry automation covering dealerships, fleet management, and connected vehicles:

- **VIN Decoder** - Decode Vehicle Identification Numbers
- **Car Insurance Quote Generator** - Automated insurance quotes
- **Dealer Lead Qualifier** - Intelligent lead scoring for dealerships
- **Fleet Fuel Efficiency Report** - Fleet-wide fuel consumption analysis
- **EV Battery Degradation Report** - Battery health monitoring
- **Connected Car Alert** - Real-time vehicle diagnostic notifications
- **Recall Notice Tracker** - Automated recall tracking
- **ADAS Event Annotator** - ADAS event classification
- **Autonomous Vehicle Log Summarizer** - Self-driving log summaries
- **Ride-Share Surge Predictor** - Demand prediction for ride-sharing

### Email Agent Workflows (10)
Email automation with AI classification and response generation:

- **Auto Reply to FAQs** - RAG-powered FAQ responses
- **Auto Archive Promotions** - Smart email classification
- **Daily Email Digest** - Curated daily summaries
- **Follow-Up Emails** - Intelligent follow-up scheduling
- **Forward Attachments** - Automated attachment handling
- **Lead to HubSpot** - Email leads to CRM sync
- **Parse Invoice Emails** - Invoice data extraction
- **Product Launch Email** - Announcement campaigns
- **Mailchimp Campaign Tracking** - Campaign analytics
- **SendGrid Bounce Alert** - Delivery failure monitoring

## Key Benefits

- **Rapid Deployment** - Import JSON files and go live in minutes
- **AI-Powered Intelligence** - Semantic understanding using vector embeddings
- **Scalable Architecture** - Redis-based vector storage for production workloads
- **Contextual Memory** - Agents maintain conversation history for better responses
- **Integration Ready** - Pre-configured connections to popular services
- **Audit Trails** - Automatic logging to Google Sheets for compliance

## Use Cases

These workflows solve real-world automation challenges:
- **Customer Support** - Automate FAQ responses with 90%+ accuracy
- **Lead Management** - Qualify and route leads without manual intervention
- **Document Processing** - Extract structured data from unstructured emails
- **Fleet Operations** - Monitor vehicle health and optimize maintenance schedules
- **Campaign Analytics** - Track email performance across platforms

## Architecture

Each workflow follows this pattern:
1. **Webhook Trigger** - HTTP endpoint
2. **Text Splitter** - Document chunking
3. **Embeddings** - HuggingFace/Cohere models
4. **Vector Store** - Redis-based semantic search
5. **LLM Agent** - Context-aware responses with memory
6. **Actions** - Sheets logging, emails, CRM updates

##  Quick Start

**Prerequisites:** n8n instance, Redis, API credentials (HuggingFace, Google Sheets)

1. Import JSON files into n8n (Workflows → Import)
2. Configure credentials (HuggingFace, Redis, Google Sheets, email)
3. Activate workflows and test webhooks

**Example:**
```bash
curl -X POST https://n8n.example.com/webhook/vin_decoder \
  -d '{"vin": "1HGBH41JXMN109186"}'
```

## 🔧 Customization

Modify workflows by adjusting:
- Agent prompts for different responses
- Chunk sizes in Text Splitter
- Embedding models and parameters
- Vector store configurations

Each workflow logs to Google Sheets for monitoring and analytics.

---

**Built for n8n** • **LangChain & AI Powered** • **Ready to Deploy**
