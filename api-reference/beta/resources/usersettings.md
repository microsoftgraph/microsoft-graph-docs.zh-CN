---
title: userSettings 资源类型
description: '内容发现的当前用户设置。 '
author: jpettere
ms.localizationpriority: medium
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 4af8059856172ab15a44e20aa1b8dbc5374c195e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336345"
---
# <a name="usersettings-resource-type"></a>userSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

设置表示用户对以下内容的首选项的首选项：
- 访问 Delve
- [项目见解](../resources/officegraphinsights.md)
- [区域设置和语言](../resources/regionalandlanguagesettings.md)
- [排班](../resources/shiftpreferences.md)
- [合并重复联系人的建议](../resources/contactmergesuggestions.md)。

管理Delve辅助功能：
  - 检查用户和用户的组织是否有权访问Office Delve。
  - 为特定用户禁用或Office Delve文档。 

配置 [itemInsights 的可见性](../resources/iteminsights.md) 和 [会议时间见解](https://support.microsoft.com/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1)。 ItemInsight 在用户和其他项目之间派生 (如文档中的文档) 网站Microsoft 365：
  - 检查是否已启用用户的项目和会议时间见解。
  - 为特定用户禁用或启用项和会议时间见解。

管理用户基于区域设置首选项： 
  - 确定用户首选使用哪些语言和区域格式来查看应用程序。
  - 更新用户的语言和区域格式首选项。

管理用户的工作班次首选项： 
  - 检查是否可以在日程安排中为用户分配班次。
  - 更新用户的班次首选项。
  
配置 [contactMergeSuggestions](../resources/contactmergesuggestions.md)：
  - 确定是否启用合并用户重复联系人的建议。
  - 禁用或启用为用户合并重复联系人的建议。

若要了解如何获取或更新用户设置，请参阅[获取设置](../api/usersettings-get.md)和[更新设置](../api/usersettings-update.md)。

> [!NOTE]
> 此终结点仅适用于 [用户](user.md) 资源。 

## <a name="methods"></a>方法
| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取用户设置](../api/usersettings-get.md) |[userSettings](../resources/usersettings.md)| 获取用户和组织设置。 |
|[更新用户设置](../api/usersettings-update.md) |[userSettings](../resources/usersettings.md)| 更新用户当前的设置。 |

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|布尔值|如果设为 true，则用户的 Office Delve 中的文档将禁用。 用户可以在 [Office Delve](https://support.office.com/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout) 中控制此设置。 |
|contributionToContentDiscoveryAsOrganizationDisabled|布尔值|反映Office Delve[级别设置](https://support.office.com/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)。 如果设为 true，则组织没有 Office Delve 的访问权限。 此设置为只读，并且仅可由管理员在 [SharePoint 管理中心](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)更改。|

## <a name="relationships"></a>关系

| 关系 | 类型 | 说明 |
|:---------------|:--------|:----------|
|contactMergeSuggestions|[contactMergeSuggestions](contactmergesuggestions.md)| 用户的设置，用于查看用户联系人列表中重复联系人的合并建议。|
|itemInsights|[userInsightsSettings](userinsightssettings.md)| 用户设置，用于查看在用户与 Microsoft 365（如文档或网站）之间派生的每小时见解和见解。 [通过此导航属性获取 userInsightsSettings](../api/userinsightssettings-get.md) 。 |
|regionalAndLanguageSettings|[regionalAndLanguageSettings](regionalandlanguagesettings.md)| 用户的语言、区域设置和日期/时间格式的首选项。 |
|shiftPreferences|[shiftPreferences](shiftpreferences.md)| 用户的班次首选项。 |



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


