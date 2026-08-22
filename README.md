# WhatsApp Bot

A WhatsApp bot built with Node.js and Express that can handle incoming messages and send automated responses.

## Features

- Receive incoming WhatsApp messages
- Send automated responses
- Process and parse user interactions
- Extract view-once message contents
- Webhook-based message delivery

## Setup

### Prerequisites

- Node.js (v14 or higher)
- WhatsApp Business Account
- Access to WhatsApp API

### Installation

1. Clone the repository
```bash
git clone https://github.com/brightjoshua543-stack/brightjoshua543-stack-whatsapp-bot.git
cd brightjoshua543-stack-whatsapp-bot
```

2. Install dependencies
```bash
npm install
```

3. Set up environment variables
```bash
cp .env.example .env
# Edit .env with your WhatsApp API credentials
```

### Configuration

Update the `.env` file with your WhatsApp Business Account details:

- `WHATSAPP_API_URL`: WhatsApp Graph API URL
- `WHATSAPP_PHONE_NUMBER_ID`: Your WhatsApp phone number ID
- `WHATSAPP_BUSINESS_ACCOUNT_ID`: Your business account ID
- `WHATSAPP_ACCESS_TOKEN`: Your API access token
- `WHATSAPP_VERIFY_TOKEN`: Your webhook verification token

### Running the Bot

**Development mode:**
```bash
npm run dev
```

**Production mode:**
```bash
npm start
```

The bot will start listening on the configured PORT (default: 3000).

## API Endpoints

### GET /
Health check endpoint

### GET /webhook
Webhook verification endpoint for WhatsApp API setup

### POST /webhook
Receives incoming WhatsApp messages

## Implementation Details

- Uses WhatsApp Business API for message handling
- Webhook-based message delivery system
- Message parsing and routing logic
- Automated response generation

## Next Steps

1. Implement message processing logic
2. Add natural language processing for better responses
3. Set up database for conversation history
4. Add error handling and logging
5. Deploy to production environment

## License

MIT
