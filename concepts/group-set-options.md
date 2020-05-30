---
title: 设置 Microsoft 365 组行为和设置选项
description: 在 Microsoft Graph 中使用组资源，您可以设置特定的组行为和资源，以便在创建 Microsoft 365 组时进行设置。
author: yyuank
localization_priority: Priority
ms.openlocfilehash: fd276dcdc42b70f6ed3aeb2e43095e6b5d76e2d4
ms.sourcegitcommit: a1a57e803c334e11316dd571ad1b54c95406740e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2020
ms.locfileid: "44413495"
---
# <a name="set-microsoft-365-group-behaviors-and-provisioning-options-preview"></a>设置 Microsoft 365 组行为和设置选项（预览）

在 Microsoft Graph 中使用[组](/graph/api/resources/group?view=graph-rest-beta)资源，您可以设置特定的组行为和资源，以便在创建 Microsoft 365 组时进行设置。 根据资源的不同，还可以在组更新中进行设置。

### <a name="configuring-and-provisioning-groups"></a>配置和设置组

**Group**资源公开两个属性（ **resourceBehaviorOptions**和**resourceProvisioningOptions**），以自定义要在创建组时设置的行为和资源。 

> [!NOTE]
> **ResourceBehaviorOptions**和**resourceProvisioningOptions**属性当前仅在 Microsoft Graph beta 终结点中可用。 请勿在生产应用程序中使用它们，因为它们可能会更改，恕不另行通知。

**resourceBehaviorOptions**是一个字符串集合，用于指定 Microsoft 365 组的组行为。 只能在 "[创建组](/graph/api/group-post-groups?view=graph-rest-beta)" （）中设置这些 bahaviors `POST` 。

| ResourceBehaviorOptions 支持的值   |说明|如果未设置，则为默认值|
|:---------------|:--------|:-----------|
| AllowOnlyMembersToPost|只有组*成员*可以向组发布对话。|组织中的任何用户都可以向组发布对话。|
| HideGroupInOutlook|此组在 Outlook 体验中处于隐藏状态。|在 Outlook 体验中，所有组都是可见且可发现的。|
| SubscribeNewGroupMembers|成员可以订阅接收组对话。 |组成员不接收组对话。|
| WelcomeEmailDisabled|欢迎电子邮件不会发送给新成员。|加入组时，会将欢迎电子邮件发送到新成员。|

**resourceProvisioningOptions**是一个字符串集合，用于指定要作为创建 Microsoft 365 组的一部分进行设置的组资源，这些资源通常不是默认组创建的一部分。

| ResourceProvisioningOptions 支持的值   |说明| 如果未设置，则为默认值 |
|:---------------|:--------|:------------|
| Teams|将此组设置为 Microsoft 团队中的团队。 此外，还可以通过操作将此值添加到[组更新](/graph/api/group-update?view=graph-rest-beta)中的**resourceProvisioningOptions**字符串集合 `PATCH` ，以便将现有的 Microsoft 365 组转换为团队。| 该组是不带团队功能的常规 Microsoft 365 组。|


## <a name="see-also"></a>另请参阅

- [Microsoft Graph 中的 Microsoft 365 组概述](office365-groups-concept-overview.md)
- [Microsoft Teams API 概述](teams-concept-overview.md)
