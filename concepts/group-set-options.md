---
title: 设置 Microsoft 365 组行为与预配选项
description: 使用Microsoft Graph中的组资源来设置创建Microsoft 365组时要预配的特定组行为和资源。
author: psaffaie
ms.localizationpriority: high
ms.openlocfilehash: 82349bfa47d0df9ed81384bf4af4108f18726f40
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096201"
---
# <a name="set-microsoft-365-group-behaviors-and-provisioning-options"></a>设置 Microsoft 365 组行为与预配选项

使用 Microsoft Graph 中的 [组](/graph/api/resources/group) ，可设置创建 Microsoft 365 组时要预配的特定组行为和资源。 根据资源，还可在组更新时预配某些内容。

**组** 资源公开两个属性，即 **resourceBehaviorOptions** 和 **resourceProvisioningOptions**，用于自定义创建组时要预配的行为和资源。

## <a name="configure-groups"></a>配置组

**resourceBehaviorOptions** 是一个字符串集合，用于为 Microsoft 365 组指定组行为。 这些行为只能在 [组创建](/graph/api/group-post-groups)时设置 (`POST`)。

| resourceBehaviorOptions 支持的值 | 说明                                                  | 如果未设置，则为默认值                                                |
| :------------------------------------------- | :----------------------------------------------------------- | :---------------------------------------------------------------- |
| AllowOnlyMembersToPost                       | 只有组 _成员_ 可以向组发布对话。    | 组织中的任何用户都可以向组发布对话。 |
| HideGroupInOutlook                           | 此组在 Outlook 体验中是隐藏的。                 | 所有组在 Outlook 体验中都是可见的，也是可发现的。   |
| SubscribeNewGroupMembers                     | 成员可以订阅接收组对话。 | 组成员不接收组对话。                 |
| WelcomeEmailDisabled                         | 欢迎电子邮件不会发送给新成员。                  | 加入组时，会将欢迎电子邮件发送到新成员。     |

## <a name="provision-groups"></a>预配组

**resourceProvisioningOptions** 是一个字符串集合，指定要预配为 Microsoft 365 组的一部分的组资源。 可以在组创建或更新期间指定这些资源。

| resourceProvisioningOptions 支持的值 | 说明                                              | 如果未设置，则为默认值                                                |
| :----------------------------------------------- | :------------------------------------------------------- | :---------------------------------------------------------------- |
| 团队                                             | 在 Microsoft Teams 中将此组预配为团队。此外，还可以通过 `PATCH` 操作将此值添加在 [组更新](/graph/api/group-update) 上，以便从现有 Microsoft 365 组中预配团队。 | 此组是没有 Teams 功能的常规 Microsoft 365 组。 |

## <a name="see-also"></a>另请参阅

- [Microsoft Graph 中的 Microsoft 365 组概述](office365-groups-concept-overview.md)
- [Microsoft Teams API 概述](teams-concept-overview.md)
