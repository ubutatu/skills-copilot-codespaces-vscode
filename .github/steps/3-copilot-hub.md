## Step 3: Enforcing Enterprise-wide Copilot Policies

_Great progress! Now let's look at how to scale these policies._

Enterprise administrators can manage Copilot access and settings across multiple organizations. This ensures consistency and compliance at scale.

### :keyboard: Activity: Create an Enterprise Policy Configuration

1. Create a new file named `enterprise-governance.yml`.
2. Define the organizations and policies that should be active.

Add the following content to `enterprise-governance.yml`:

```yaml
enterprise:
  policies:
    copilot:
      access:
        organizations:
          - engineering
          - security
      settings:
        public_code_filter: blocked
        chat_in_ide: enabled
        chat_on_github: enabled
```

3. Commit and push this file to your `main` branch.

**Wait about 60 seconds then refresh your repository landing page for the next step.**
