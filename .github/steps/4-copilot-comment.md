## Step 4: Monitoring Usage and Audit Logs

_The final piece of the compliance puzzle is visibility._

GitHub provides audit logs that track when Copilot settings are changed and by whom. Monitoring these logs is essential for maintaining a compliant environment.

### :keyboard: Activity: Set up an Audit Log Monitoring script

1. Create a new file named `monitor-compliance.js`.
2. Add a simple script that would simulate checking for compliance events.

Add the following content to `monitor-compliance.js`:

```javascript
// Simulate checking GitHub Audit Logs for Copilot events
function checkCopilotAuditLogs() {
    console.log("Fetching audit logs for enterprise...");
    const complianceEvents = [
        { event: "copilot.policy_change", actor: "admin", timestamp: "2023-10-27T10:00:00Z" },
        { event: "copilot.access_granted", actor: "admin", timestamp: "2023-10-27T10:05:00Z" }
    ];

    complianceEvents.forEach(e => {
        console.log(`Compliance Event: ${e.event} by ${e.actor} at ${e.timestamp}`);
    });
}

checkCopilotAuditLogs();
```

3. Commit and push this file to your `main` branch.

**Wait about 60 seconds then refresh your repository landing page for the finish!**
