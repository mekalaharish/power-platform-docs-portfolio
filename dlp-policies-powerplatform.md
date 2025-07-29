# Using Data Loss Prevention (DLP) Policies in Power Platform Admin Center

## Overview
Data Loss Prevention (DLP) policies help administrators control how data flows across connectors in Power Platform environments. This guide walks you through creating and assigning a DLP policy.

## Prerequisites
- Power Platform admin role
- Access to the Power Platform Admin Center: https://admin.powerplatform.microsoft.com

## Step 1: Sign In
1. Go to the Power Platform Admin Center
2. Sign in with your admin credentials.

## Step 2: Create a New DLP Policy
1. Select **Data policies** from the left navigation.
2. Click **+ New policy**.
3. Enter a name and optional description for your policy.

<!-- Insert: Screenshot showing "Create policy" interface with name and environment scope -->

## Step 3: Define Connector Groups
1. Under **Choose connectors**, classify each connector into either:
   - **Business data only**
   - **No business data allowed**
   - **Blocked**
2. Drag and drop connectors as needed to enforce compliance.

<!-- Insert: Diagram of connectors grouped into 'Business' and 'Blocked' buckets -->

## Step 4: Apply to Environments
1. Choose the environments where this policy should apply.
2. Click **Next** and **Create policy**.

## Step 5: Review and Confirm
1. Confirm the policy settings and click **Create policy**.
2. The policy will now be enforced across selected environments.

## Best Practices
- Review policies quarterly to adapt to organizational changes.
- Avoid placing critical connectors (like SharePoint or Outlook) in the Blocked group without business justification.
- Use audit logs to monitor policy effectiveness.

## Resources
- https://learn.microsoft.com/power-platform/admin/wp-data-loss-prevention
- https://learn.microsoft.com/power-platform/admin/environments-overview