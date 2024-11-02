# KeyRephrase 
## Overview
KeyRephrase is a Windows application designed to help you rephrase text using a simple shortcut key. By selecting the text and pressing **Shift + Alt + X**, the application will automatically replace the selected text with a rephrased version. This functionality works in any text writing window on Windows.

## Features
- Rephrase text using a shortcut key (**Shift + Alt + X**).
- Supports multiple Large Language Model (LLM) providers.
- Easy configuration through a `credentials.yml` file.

## Supported LLM Providers
- OpenAI
- OpenRouter
- Groq
- Cerebras
- AzureAI
- Gemini

## Configuration
To configure KeyRephrase, you need to update the `credentials.yml` file with your API key and other necessary details. Below is an example of the `credentials.yml` file:

```yaml
# Configuration for AI provider credentials
credential:
  provider: 'gemini'  # Supported providers: openai, openrouter, groq, cerebras, azureai, gemini
  api_key: 'xxxxx' # Your API key here
  model_name: 'gemini-1.5-pro' # Model name to use (e.g., gemini-1.5-pro, gpt-4)
  api_endpoint: '' # Custom API endpoint if required e.g: https://api.xxx.ai/v1
  api_version: '' # API version if required (mainly for Azure)
```

## Obtaining API Keys
You can obtain API keys from the following providers:

| Provider  | URL                                                                                     |
|-----------|-----------------------------------------------------------------------------------------|
| OpenAI    | https://platform.openai.com/settings/profile/api-keys                                   |
| AzureAI   | https://azure.microsoft.com/en-us/services/cognitive-services/openai-service/          |
| Groq      | https://console.groq.com/keys : Free                                                  |
| Gemini    | https://ai.google.dev/gemini-api/docs/api-key : Free                                   |
| Cerebras  | https://cloud.cerebras.ai/ : Free                                                      |

## Usage
1. Select the text you want to rephrase.
2. Press **Shift + Alt + X**.
3. The selected text will be automatically replaced with the rephrased text.

## Support
For any issues or support, please refer to the documentation provided by your LLM provider or raise issue in current repo.

