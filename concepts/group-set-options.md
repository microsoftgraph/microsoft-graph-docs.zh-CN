---
title: 设置 Microsoft 365 组行为与预配选项
description: 在 Microsoft Graph 使用组资源，你可以设置创建 Microsoft 365 组时要预配的特定组行为和资源。
author: Jordanndahl
ms.localizationpriority: high
ms.openlocfilehash: d8e902c0b2cd43c870d29fcf00b4e28e1e17fca8
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225929"
---
# <a name="set-microsoft-365-group-behaviors-and-provisioning-options-preview"></a>设置 Microsoft 365 组行为与预配选项（预览）

使用 Microsoft Graph 中的 [组](/graph/api/resources/group) ，可设置创建 Microsoft 365 组时要预配的特定组行为和资源。 根据资源，还可在组更新时预配某些内容。

### <a name="configuring-and-provisioning-groups"></a>配置和预配组

**组** 资源公开两个属性，即 **resourceBehaviorOptions** 和 **resourceProvisioningOptions**，用于自定义创建组时要预配的行为和资源。 

**resourceBehaviorOptions** 是一个字符串集合，用于为 Microsoft 365 组指定组行为。 这些行为只能在 [组创建](/graph/api/group-post-groups)时设置 (`POST`)。

| resourceBehaviorOptions 支持的值   |说明|如果未设置，则为默认值|
|:---------------|:--------|:-----------|
| AllowOnlyMembersToPost|只有组 *成员* 可以向组发布对话。|组织中的任何用户都可以向组发布对话。|
| HideGroupInOutlook|此组在 Outlook 体验中是隐藏的。|所有组在 Outlook 体验中都是可见的，也是可发现的。|
| SubscribeNewGroupMembers|成员可以订阅接收组对话。 |组成员不接收组对话。|
| WelcomeEmailDisabled|欢迎电子邮件不会发送给新成员。|加入组时，会将欢迎电子邮件发送到新成员。|

**resourceProvisioningOptions** 是一个字符串集合，指定要预配为 Microsoft 365 组的一部分的组资源。 可以在组创建或更新期间指定这些资源。

| resourceProvisioningOptions 支持的值   |说明| 如果未设置，则为默认值 |
|:---------------|:--------|:------------|
| 团队|在 Microsoft Teams 中将此组预配为团队。此外，还可以通过 `PATCH` 操作将此值添加在 [组更新](/graph/api/group-update) 上，以便从现有 Microsoft 365 组中预配团队。| 此组是没有 Teams 功能的常规 Microsoft 365 组。|


## <a name="see-also"></a>另请参阅

- [Microsoft Graph 中的 Microsoft 365 组概述](office365-groups-concept-overview.md)
- [Microsoft Teams API 概述](teams-concept-overview.md)
