## Step 1: Public Code Filter (Enterprise Enforced)

_Welcome to the "GitHub Copilot Enterprise Compliance Pro" course! :shield:_

GitHub Copilot for Enterprise allows organizations to enforce policies that ensure code suggestions meet their compliance standards. One of the most critical settings is the **Public Code Filter**.

When enabled, this filter checks code suggestions against a set of public code on GitHub. If a suggestion matches public code, it is blocked, helping to prevent potential licensing and intellectual property issues.

### :keyboard: Activity: Configure the Public Code Filter

1. In your GitHub organization settings, navigate to **Copilot** > **Policies**.
2. Locate the **Suggestions matching public code** setting.
3. Set this policy to **Blocked**.
4. In this exercise, we will simulate this by creating a configuration file.

Create a new file named `copilot-policy.json` in the root of your repository with the following content:

```json
{
  "public_code_filter": "enabled",
  "enterprise_enforcement": "required"
}
```

5. Commit and push this file to your `main` branch.

**Wait about 60 seconds then refresh your repository landing page for the next step.**
