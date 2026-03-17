# OpenAI API Key Configuration and Model Setup

## API Key Configuration

1. Sign up for an API key at [OpenAI's website](https://beta.openai.com/signup/).
2. Store your API key securely, and do not expose it in public repositories.
3. You can set your API key as an environment variable:
   
   ```bash
   export OPENAI_API_KEY='your_api_key_here'
   ```

## Model Setup

1. Choose the OpenAI model you would like to use. Common options include:
   - `gpt-3.5-turbo`
   - `gpt-4`
   
2. In your code, initialize the model with the API key:
   
   ```python
   import openai
   
   openai.api_key = os.getenv("OPENAI_API_KEY")
   model = "gpt-3.5-turbo"
   ```

3. Make requests to the model:
   
   ```python
   response = openai.ChatCompletion.create(
       model=model,
       messages=[{"role": "user", "content": "Hello!"}]
   )
   print(response)
   ```

4. Refer to the [OpenAI API documentation](https://platform.openai.com/docs/api-reference) for more details on how to use various features and models.

