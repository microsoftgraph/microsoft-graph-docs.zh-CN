---
title: teamsAppDefinition 资源类型
description: 表示一个版本的 teamsApp 的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 08a652c5b4ad4b9555eb7c09e33398f140ed97b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036931"
---
# <a name="teamsappdefinition-resource-type"></a>teamsAppDefinition 资源类型

命名空间：microsoft.graph

表示一个版本的 [teamsApp](teamsapp.md)的详细信息。

## <a name="properties"></a>属性

| 属性            | 类型     | 说明 |
|:------------------- |:-------- |:----------- |
| id                  | string   | 唯一 ID (团队应用程序 ID) 。 |
| teamsAppId          | 字符串   | 团队应用程序清单中的 ID。 |
| publishingState| 字符串|特定版本的团队应用程序的已发布状态。 可能的值是：</br>`submitted` —团队应用程序的特定版本已提交，正在进行审阅。 </br>`published`  —发布特定版本的团队应用程序的请求已由管理员批准，并且应用已发布。 </br> `rejected` —管理员拒绝了发布特定版本的团队应用程序的请求。 |
| displayName         | string   | 应用程序开发人员提供的应用程序的名称。 |
| version             | 字符串   | 应用程序的版本号。 |

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
  "displayName": "string",
  "version": "string"
}
```

## <a name="see-also"></a>另请参阅

- [teamsApp](teamsapp.md)
- [teamsAppInstallation](teamsappinstallation.md)
- [teamsTab](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

