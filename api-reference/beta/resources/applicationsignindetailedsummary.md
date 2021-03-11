---
title: applicationSignInDetailedSummary 资源类型 - Microsoft Graph API
description: 表示应用程序登录的详细摘要。
localization_priority: Normal
author: sureshja
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 8f53d1ebce8a7a578c067354ba7f89c6c27ea947
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720828"
---
# <a name="applicationsignindetailedsummary-resource-type"></a>applicationSignInDetailedSummary 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示应用程序登录的详细摘要。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-get.md) | [applicationSignInDetailedSummary](applicationsignindetailedsummary.md) | 读取 **applicationSignInDetailedSummary** 对象的属性和关系。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|aggregatedEventDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|appDisplayName|String|用户登录的应用程序的名称。|
|appId|String|用户登录的应用程序的 ID。|
|id|String| 表示登录活动的唯一 ID。|
|signInCount|Int64|应用程序进行登录的计数。|
|status|[signInStatus](signinstatus.md)|登录状态的详细信息。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationSignInDetailedSummary"
}-->

```json
{
  "aggregatedEventDateTime": "String (timestamp)",
  "appDisplayName": "String",
  "appId": "String",
  "id": "String (identifier)",
  "signInCount": 1024,
  "status": {"@odata.type": "microsoft.graph.signInStatus"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationSignInDetailedSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


