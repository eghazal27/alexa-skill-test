# Battery Status Alexa Skill

## Description
This Alexa skill allows users to check their system battery level by calling a webhook endpoint.

## Usage
Users can say:
- "Alexa, ask Battery Status what's my battery level"
- "Alexa, ask Battery Status for battery percentage"
- "Alexa, open Battery Status"

## Setup
1. Import this skill package into the Alexa Developer Console
2. Choose Alexa-hosted (Node.js) when prompted
3. Build and test the skill
4. Deploy when ready

## Webhook Endpoint
The skill calls: `https://accepted-marten-relieved.ngrok-free.app/webhook/alexa/battery`

## Response Format
Expected webhook response:
```json
{
  "version": "1.0",
  "response": {
    "outputSpeech": {
      "type": "PlainText",
      "text": "Your system battery in Beirut is at 58 percent."
    },
    "shouldEndSession": true
  }
}