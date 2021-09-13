---
title: 'teamsTabConfiguration 资源类型 (开放类型) '
description: 确定选项卡内容的设置。
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 90d9d51cffec818a601e8b7efddb4b77b1c2dc3d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59052858"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a>teamsTabConfiguration 资源类型 (开放类型) 

命名空间：microsoft.graph



确定选项卡内容的 [设置](teamstab.md)。当以交互方式配置选项卡时，此信息由选项卡提供程序应用程序设置。
除了下面的属性之外，某些选项卡提供程序应用程序还指定了其他自定义属性。

## <a name="properties"></a>属性

|属性|类型|说明|
|-|-|-|
|  entityId   |   string |  选项卡提供程序托管的实体的标识符。     |
|  contentUrl |   string |  用于在网站中呈现选项卡内容的Teams。 必需。    |
|  removeUrl  |   string |  当使用 Teams 客户端删除 Tab 时，由 Teams 调用的 URL。     |
|  websiteUrl |   string |  用于显示选项卡内容在外部的Teams。     |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

