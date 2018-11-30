---
title: teamsTabConfiguration 资源类型 （打开类型）
description: 确定内容的选项卡的设置。
ms.openlocfilehash: b9a638692302dc8d301c3b14e50096b08891d821
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042709"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a>teamsTabConfiguration 资源类型 （打开类型）

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

确定内容的[选项卡上](teamstab.md)的设置。选项卡以交互方式配置时，此信息由选项卡提供程序应用程序设置。
除了下面的属性中，某些选项卡提供程序应用程序指定其他自定义属性。

## <a name="properties"></a>属性

|属性|类型|说明|
|-|-|-|
|  entityId   |   string |  选项卡上的服务提供商托管实体的标识符。     |
|  contentUrl |   string |  用于呈现团队中的选项卡内容的 Url。 必需。    |
|  removeUrl  |   string |  使用团队客户端中移除一个选项卡时调用团队客户端的 Url。     |
|  websiteUrl |   string |  显示选项卡团队之外的内容的 Url。     |

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
