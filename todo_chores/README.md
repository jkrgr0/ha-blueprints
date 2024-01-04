# Chore Management <!-- omit in toc -->

> Manages your tasks/chores stored in a To-do list.

![GitHub issues by-label](https://img.shields.io/github/issues/jkrgr0/ha-blueprints/todo_chores) ![Static Badge](https://img.shields.io/badge/latest--version-0.1.0-brightgreen)

## Table of Contents <!-- omit in toc -->

- [Features](#features)
- [Configuration](#configuration)
- [Roadmap](#roadmap)

## Features

- 🔔 Receive notification when a task/chore is overdue or nearly due.
- ✅ Complete the task/chore directly through the received notification.
  - ⏭️ Automatically reschedule a completed task/chore for the next interval.
- 🕒 Postpone the task/chore for a specific time directly through the received notification.

**❗ IMPORTANT: The minimum required version of Home Assistant is `2024.1.0` ❗**

## Configuration

1. Add **Local To-do** integration.  
    In order to use this blueprint you need to create a To-do list with the [Local To-do](https://www.home-assistant.io/integrations/local_todo) integration.  
    To add the **Local To-do** integration to your Home Assistant instance, use this button:  

    [![Open your Home Assistant instance and start setting up a new integration.](https://my.home-assistant.io/badges/config_flow_start.svg)](https://my.home-assistant.io/redirect/config_flow_start/?domain=local_todo)

2. Add a new To-do list.  
    This should already be done when adding the integration for the first time.  
    If not, simply head over to the **Local To-do** integration and click on **ADD ENTRY** to create a new To-do list.
3. Create tasks/chores in the new created To-do list.  
    Configure the tasks/chores like follows:  

    | Field | Description | Example |
    | ----- | ----------- | ------- |
    | Task name | Name of the task/chore<br/>This is displayed in the notification | Vacuum living room |
    | Description | This text box is used to store additional configuration of the task/chore.<br/><br/>The following options are currently available:<br/><ul><li><code>repeat</code> - How often should the task/chore be performed.<br/>Use the format <code>X day</code></li><li><code>icon</code> - The icon to display in the notification (mdi icons - **Android only**)</ul> | <pre><code>repeat=1 day; icon=mdi:test-tube</code></pre> |
    | Due date | Set the initial due date | N/A |

4. Import this blueprint and use it for a new automation:  

    [![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url-https%3A%2F%2Fraw.githubusercontent.com%2Fjkrgr0%2Fha-blueprints%2Fmain%2Ftodo_chores%2Ftodo_chores.yaml)

## Roadmap

TBA
