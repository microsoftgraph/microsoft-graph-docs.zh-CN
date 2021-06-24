---
title: userSettings 资源类型
description: '内容发现的当前用户设置。 '
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: a16ab96bb04f6d7dfc4f9ceff29f49dc7d348d23
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108871"
---
# <a name="usersettings-resource-type"></a>userSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

设置表示用户对区域设置和语言、排班、排[](../resources/regionalandlanguagesettings.md)班和项目Delve[首选项](../resources/officegraphinsights.md)的首选项[](../resources/shiftpreferences.md)。

管理用户基于区域设置首选项： 
  - 确定用户首选使用哪些语言和区域格式查看应用程序。
  - 更新用户的语言和区域格式首选项。

管理用户的工作班次首选项： 
  - 检查是否可以在日程安排中为用户分配班次。
  - 更新用户的班次首选项。
  
管理Delve辅助功能：
  - 检查用户及其组织是否有权访问Office Delve。
  - 为特定用户禁用或Office Delve文档。 

配置 [itemInsights 的可见性](../resources/iteminsights.md) 和 [会议时间见解](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1)。 ItemInsight 在用户和其他项目之间派生 (如文档中的文档) 网站Microsoft 365：
  - 检查是否已启用用户的项目和会议时间见解。
  - 为特定用户禁用或启用项和会议时间见解。

若要了解如何获取或更新用户设置，请参阅[获取设置](../api/usersettings-get.md)和[更新设置](../api/usersettings-update.md)。

> [!NOTE]
> 此终结点仅适用于用户。 无法将此终结点用于联系人。

## <a name="methods"></a>方法
| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取用户设置](../api/usersettings-get.md) |[userSettings](../resources/usersettings.md)| 获取用户和组织设置。 |
|[更新用户设置](../api/usersettings-update.md) |[userSettings](../resources/usersettings.md)| 更新用户当前的设置。 |

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|布尔值|如果设为 true，则用户的 Office Delve 中的文档将禁用。 用户可以在 [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout) 中控制此设置。 |
|contributionToContentDiscoveryAsOrganizationDisabled|布尔值|反映Office Delve[级别设置](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)。 如果设为 true，则组织没有 Office Delve 的访问权限。 此设置为只读，并且仅可由管理员在 [SharePoint 管理中心](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)更改。|

## <a name="relationships"></a>关系

| 关系 | 类型 | 说明 |
|:---------------|:--------|:----------|
|shiftPreferences|[shiftPreferences](shiftpreferences.md)| 用户的班次首选项。 |
|regionalAndLanguageSettings|[regionalAndLanguageSettings](regionalandlanguagesettings.md)| 用户的语言、区域设置和日期/时间格式的首选项。 |
|itemInsights|[userInsightsSettings](userinsightssettings.md)| 用户设置，用于查看会议时间见解，以及从用户与 Microsoft 365（如文档或网站）中派生的见解。 [通过此导航属性获取 userInsightsSettings。](../api/userinsightssettings-get.md) |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userSettings",
  "baseType": "microsoft.graph.entity"
}-->
```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```


