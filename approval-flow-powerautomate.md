# Create an Approval Workflow with Power Automate

## Overview
Power Automate allows you to automate routine approvals such as leave requests, expense reports, or content reviews. This guide explains how to create an approval flow triggered by a new SharePoint list item.

## Prerequisites
- Power Automate access via Microsoft 365
- A SharePoint list with a title column and requester details

## Step 1: Start from a Template
1. Go to https://make.powerautomate.com
2. Select **Templates** from the left pane.
3. Search for "Start approval when a new item is added to SharePoint".
4. Select the template and click **Continue**.

<!-- Insert: Screenshot of selected approval template -->

## Step 2: Configure the Trigger
1. Choose your SharePoint site and list.
2. Map columns like **Title** and **Requester Name**.

## Step 3: Define Approval Details
1. Under **Start and wait for an approval**, select:
   - Approval type: *Approve/Reject – First to respond*
   - Title: “Approval Request for [Title]”
   - Assigned To: Enter manager’s email or dynamic value

2. Add a **Condition** step:
   - If outcome is *Approve*, send confirmation email.
   - If outcome is *Reject*, send rejection message.

<!-- Insert: Visual flow from trigger → approval → condition → outcomes -->

## Step 4: Save and Test
1. Click **Save** at the top.
2. Add a test item in your SharePoint list to trigger the flow.
3. Monitor execution in **My Flows > Run History**.

## Optional Enhancements
- Add a parallel branch for multi-approver scenarios.
- Log approval responses in a SharePoint log list.

## Resources
- https://learn.microsoft.com/power-automate/
- https://learn.microsoft.com/power-automate/approvals-overview