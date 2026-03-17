# Jira Setup and Automation Configuration

## Prerequisites
- A Jira account with administrative privileges.
- Access to the project's settings in Jira.
- Required tools installed (such as a code editor, terminal, etc.).

## API Token Generation
1. Log in to your Jira account.
2. Navigate to **Account settings** > **Security**.
3. Under **API Token**, select **Create and manage API tokens**.
4. Click on **Create API token**.
5. Enter a label for the token and click **Create**.
6. Copy the generated token and keep it secure.

## Webhook Configuration
1. Go to your Jira project.
2. Navigate to **Project settings** > **Webhooks**.
3. Click on **Create a webhook**.
4. Provide a name and the URL for the webhook to send data to.
5. Select the events you want to trigger the webhook.
6. Save the webhook configuration.

## Environment Variables Setup
- Set the following environment variables to integrate with the Jira API:
  - `JIRA_API_URL`: The base URL for your Jira instance.
  - `JIRA_API_TOKEN`: The API token generated earlier.
  - `JIRA_USERNAME`: Your Jira username.

Ensure that these variables are correctly set in your development environment or CI/CD pipeline.