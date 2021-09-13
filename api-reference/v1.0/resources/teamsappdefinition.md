---
title: teamsAppDefinition 资源类型
description: 表示 teamsApp 的一个版本的详细信息。
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 923cba82d9def93b619545cf4184180ef220f247
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021426"
---
# <a name="teamsappdefinition-resource-type"></a>teamsAppDefinition 资源类型

命名空间：microsoft.graph

表示 [teamsApp 版本的详细信息](teamsapp.md)。

## <a name="properties"></a>属性

| 属性            | 类型     | 说明 |
|:------------------- |:-------- |:----------- |
| id                  | string   | 唯一 ID (应用Teams ID) 。 |
| teamsAppId          | string   | 应用清单Teams ID。 |
| publishingState| string|应用程序特定版本的已发布Teams状态。 可能的值是：</br>`submitted`— 应用程序的特定版本Teams已提交并且正在审查中。 </br>`published`— 发布特定版本的 Teams 请求已由管理员批准，并且应用已发布。 </br> `rejected`— 管理员拒绝了发布特定版本的 Teams 应用的请求。 |
| displayName         | string   | 应用开发人员提供的应用的名称。 |
| version             | string   | 应用程序的版本号。 |
| shortDescription    | 字符串   | 应用程序的简短说明。 |
| 说明         | string   | 应用程序详细说明。 |

## <a name="relationships"></a>关系

| 关系 | 类型   | 说明 |
|:---------------|:--------|:----------|
|bot|[teamworkBot](teamworkbot.md) | 在应用清单中指定的自动程序Teams详细信息。 |

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

