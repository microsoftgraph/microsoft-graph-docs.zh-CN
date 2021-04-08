---
title: teamsAppDefinition 资源类型
description: teamsApp 的一个版本的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 205c656e81ed9dfc75e97cbe0734eeb36c5c0127
ms.sourcegitcommit: aa18eb8a9965f99cc97680808abba8df46f31ba5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "51638905"
---
# <a name="teamsappdefinition-resource-type"></a>teamsAppDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

teamsApp [版本的详细信息](teamsapp.md)。

## <a name="properties"></a>属性

| 属性            | 类型     | 说明 |
|:------------------- |:-------- |:----------- |
| id                  | string   | 唯一 id (不是 teams appid) 。 |
| teamsAppId          | 字符串   | Teams 应用清单中的 ID。 |
| publishingState| 字符串|Teams 应用特定版本的已发布状态。 可能的值是：</br>`submitted` — Teams 应用的特定版本已提交，正在审查中。 </br>`published`  — 发布特定版本的 Teams 应用的请求已由管理员批准，并且该应用已发布。 </br> `rejected` — 管理员拒绝了发布 Teams 应用的特定版本的请求。 |
| azureADAppId        | 字符串   | The WebApplicationInfo.id from the Teams App manifest. |
| displayName         | string   | 应用开发人员提供的应用的名称。 |
| version             | 字符串   | 应用程序的版本号。 |
| allowedInstallationScopes | teamsAppInstallationScope 集合 | 可在其中安装 Teams 应用的范围集合。 可能的值是：</br>`team` — 指示 Teams 应用可以安装在团队中，并有权访问该团队的数据。 </br>`groupChat`  — 指示 Teams 应用可以安装在群聊中，并有权访问该群聊的数据。 </br> `personal` — 指示 Teams 应用可以安装在用户的个人范围内，并有权访问该用户的数据。 | 

## <a name="relationships"></a>关系

| 关系 | 类型   | 说明 |
|:---------------|:--------|:----------|
|bot|[teamworkBot](teamworkbot.md) | Teams 应用清单中指定的自动程序的详细信息。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "Test App",
  "version": "1.0.0"
}
```

## <a name="see-also"></a>另请参阅

- [teamsApp](teamsapp.md)
- [teamsAppInstallation](teamsappinstallation.md)
- [teamsTab](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


