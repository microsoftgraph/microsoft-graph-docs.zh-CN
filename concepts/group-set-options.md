---
title: 设置 Microsoft 365 组行为与预配选项
description: 在 Microsoft Graph 使用组资源，你可以设置创建 Microsoft 365 组时要预配的特定组行为和资源。
author: Jordanndahl
localization_priority: Priority
ms.openlocfilehash: 54e4622a69f33980494962882ac1aa06d07eaec5
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682178"
---
# <a name="set-microsoft-365-group-behaviors-and-provisioning-options-preview"></a>设置 Microsoft 365 组行为与预配选项（预览）

使用 Microsoft Graph 中的 [组](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) ，可设置创建 Microsoft 365 组时要预配的特定组行为和资源。 根据资源，还可在组更新时预配某些内容。

### <a name="configuring-and-provisioning-groups"></a>配置和预配组

**组** 资源公开两个属性，即 **resourceBehaviorOptions** 和 **resourceProvisioningOptions**，用于自定义创建组时要预配的行为和资源。 

> [!NOTE]
> **resourceBehaviortions** 和 **resourceProvisioningOptions** 属性目前仅可用于 Microsoft Graph beta 版终结点。  请勿在生产应用中使用它们，因为它们可能在没有通知的情况下随时更改。

**resourceBehaviorOptions** 是一个字符串集合，用于为 Microsoft 365 组指定组行为。 这些行为只能在 [组创建](/graph/api/group-post-groups?view=graph-rest-beta&preserve-view=true)时设置 (`POST`)。

| resourceBehaviorOptions 支持的值   |说明|如果未设置，则为默认值|
|:---------------|:--------|:-----------|
| AllowOnlyMembersToPost|只有组 *成员* 可以向组发布对话。|组织中的任何用户都可以向组发布对话。|
| HideGroupInOutlook|此组在 Outlook 体验中是隐藏的。|所有组在 Outlook 体验中都是可见的，也是可发现的。|
| SubscribeNewGroupMembers|成员可以订阅接收组对话。 |组成员不接收组对话。|
| WelcomeEmailDisabled|欢迎电子邮件不会发送给新成员。|加入组时，会将欢迎电子邮件发送到新成员。|

**resourceProvisioningOptions** 是一个字符串集合，用于指定作为创建 Microsoft 365 组的一部分进行预配的组资源，但这些组资源通常不是默认组创建的组成部分。

| resourceProvisioningOptions 支持的值   |说明| 如果未设置，则为默认值 |
|:---------------|:--------|:------------|
| Teams|将此组预配为 Microsoft Teams 中的团队。此外，此值可通过 `PATCH` 操作添加到 [组更新](/graph/api/group-update?view=graph-rest-beta&preserve-view=true) 上的 **resourceProvisioningOptions** 字符串集合，以便将现有的 Microsoft 365 组转换为团队。| 此组是没有 Teams 功能的常规 Microsoft 365 组。|


## <a name="see-also"></a>另请参阅

- [Microsoft Graph 中的 Microsoft 365 组概述](office365-groups-concept-overview.md)
- [Microsoft Teams API 概述](teams-concept-overview.md)
