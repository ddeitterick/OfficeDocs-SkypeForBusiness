--- 
title: Manage reactions in Teams meetings and webinars
ms.author: wlibebe
author: wlibebe
manager: pamgreen
ms.topic: article
ms.service: msteams
ms.reviewer: defnea
ms.date: 10/12/2023
audience: admin
ms.localizationpriority: medium
search.appverid: MET150
ms.collection: 
  - M365-collaboration
  - Tier2
  - m365initiative-meetings
appliesto: 
  - Microsoft Teams
f1.keywords:
- NOCSH
ms.custom: 
  - ms.teamsadmincenter.meetingpolicies.participantandguests
description: Learn to manage meeting reactions in Teams meetings.
---

# Manage reactions in Teams meetings and webinars

**APPLIES TO:** ✔️Meetings ✔️Webinars ✖️Town halls

As an admin, you can manage whether organizers can include reactions in their meetings and webinars through the Teams admin center or using PowerShell. Reactions are enabled by default.

This setting sets the default for new meetings. Meeting organizers can change the setting for each meeting that they create.

To set the default for meeting reactions in new meetings:

1. In the Teams admin center, expand **Meetings** and select **Meeting policies**.
1. Select the policy that you want to edit.
1. Scroll to the **Meeting engagement** section.
1. Toggle the **Reactions** setting **On** or **Off**.
1. Select **Save**.

To configure the setting in PowerShell, use the **`-AllowMeetingReactions`** parameter within the PowerShell [Set-CsTeamsMeetingPolicy](/powershell/module/teams/set-csteamsmeetingpolicy) cmdlet.

To turn off meeting reactions, use the following script:

```powershell
Set-CsTeamsMeetingPolicy -Identity <policy name> -AllowMeetingReactions Disabled
```

## Related topics

[Teams policy reference](settings-policies-reference.md)

[Assign policies to your users in Teams](policy-assignment-overview.md)

[Teams PowerShell overview](teams-powershell-overview.md)

[Express yourself in Teams meetings with live reactions](https://support.microsoft.com/office/a8323a40-3d07-4129-934b-305370a36e21)
