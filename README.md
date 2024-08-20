# Site Status Data

This repository contains JSON files used to manage the site’s status and announcements. It includes configuration files for handling site maintenance and displaying announcements.

## Files

### `announcement.json`

The `announcement.json` file contains the data for announcements displayed on the site. It includes information about the announcement type, message, and an optional link.

#### JSON Structure

```json
{
  "type": "maintenance",
  "message": "Test New Message, 05:00-06:00 PST.",
  "link": {
    "text": "Learn more",
    "url": "https://status.epicspro.com"
  }
}
```

- **`type`**: Specifies the type of announcement. Possible values are:
  - `"update"`: Indicates a general update or new feature release.
  - `"maintenance"`: Indicates scheduled maintenance or downtime.
- **`message`**: The message to display in the announcement banner.
- **`link`** (optional): An object containing `text` and `url`. If provided, `text` is the link text, and `url` is the destination URL.

### `maintenance.json`

The `maintenance.json` file indicates whether the site is under maintenance. It is used to conditionally display a maintenance page.

#### JSON Structure

```json
{
  "maintenanceMode": true
}
```
