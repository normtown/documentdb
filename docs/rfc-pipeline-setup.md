# RFC Pipeline - GitHub Setup Guide

This guide documents the manual setup steps for the RFC Pipeline as specified in RFC-0003.

**Target Repository:** https://github.com/documentdb/documentdb

## 1. Create GitHub Projects Board

### Step 1.1: Create the Project

1. Navigate to https://github.com/documentdb/documentdb
2. Click **Projects** tab
3. Click **New project** (green button)
4. Select **Board** layout
5. Name: `RFC Pipeline`
6. Description: `Tracks RFC lifecycle from draft to completion`
7. Click **Create**

### Step 1.2: Configure Columns

Add these columns in order (left to right):

| Column | Description |
|--------|-------------|
| Draft | Initial RFC submissions, problem statement only |
| Under Review | PR opened, awaiting review |
| Accepted | RFC PR merged, approved for implementation |
| Implementing | Implementation PRs in progress |
| Complete | All implementation merged |
| Archived | Superseded or abandoned RFCs |

**To add columns:**
1. Click **+** on the right side of the board
2. Enter column name
3. Drag columns to reorder as needed

### Step 1.3: Add Required Fields

1. Click **Settings** (gear icon) in project
2. Navigate to **Custom fields**
3. Add these fields:

| Field Name | Type | Required |
|------------|------|----------|
| Champion | Person | Yes |
| Issue Link | URL | Yes |
| Target Version | Text | Yes |

### Step 1.4: Add Optional Fields

| Field Name | Type | Required |
|------------|------|----------|
| Discussion Link | URL | No |

## 2. Set Up GitHub Discussions

### Step 2.1: Enable Discussions

1. Navigate to **Settings** > **Features**
2. Enable **Discussions** if not already enabled

### Step 2.2: Create RFC Categories

Navigate to **Discussions** > **Categories** (gear icon) and create:

| Category | Description | Format |
|----------|-------------|--------|
| RFC Ideas | Validate RFC ideas before formal submission | Open-ended |
| RFC Questions | Clarification questions about existing RFCs | Q&A |
| Implementation Help | Coordination for RFC implementation | Open-ended |
| Process Feedback | Suggestions for improving the RFC process | Open-ended |

**For each category:**
1. Click **New category**
2. Enter name and description
3. Select appropriate format
4. Save

## 3. Verification Checklist

After setup, verify:

- [ ] Projects board "RFC Pipeline" exists
- [ ] All 6 columns are present in correct order
- [ ] Champion field exists (Person type)
- [ ] Issue Link field exists (URL type)
- [ ] Target Version field exists (Text type)
- [ ] Discussion Link field exists (URL type, optional)
- [ ] Discussions enabled
- [ ] RFC Ideas category exists
- [ ] RFC Questions category exists
- [ ] Implementation Help category exists
- [ ] Process Feedback category exists

## 4. Post-Setup

After completing manual setup:

1. Update RFC-0003 Story 1.4 status to COMPLETE
2. Close bead `do-7dt`
3. Proceed with Story 1.5 (RFC Automation workflows)

---

*Generated for RFC-0003 Story 1.4 implementation*
*Reference: rfcs/0003-rfc-process.md*
