---
title: offerShiftRequest 资源类型
description: 表示向团队中的其他用户提供班次的 shift 请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e7c41461848fab45f3d291b175e6c584f98326fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021271"
---
# <a name="offershiftrequest-resource-type"></a>offerShiftRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示向团队中的其他用户提供班次的 shift 请求的类型。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建](../api/offershiftrequest-post.md) | [offerShiftRequest](offershiftrequest.md) | 创建 offerShiftRequest 对象的实例。 |
| [获取](../api/offershiftrequest-get.md) | [offerShiftRequest](offershiftrequest.md) | 读取 offerShiftRequest 对象的属性和关系。 |
| [List](../api/offershiftrequest-list.md) | [OfferShiftRequest](offershiftrequest.md)的集合 | 读取团队中所有 offerShiftRequest 对象的属性和关系。 |
|[批准](../api/offershiftrequest-approve.md)|无|批准 offerShiftRequest。 |
|[拒绝](../api/offershiftrequest-decline.md)|无|拒绝 offerShiftRequest。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|recipientActionDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|recipientActionMessage|String| 由服务移动请求的收件人发送的自定义消息。 |
|recipientUserId|String| 提供班次请求的收件人的用户 id。|
|senderShiftId|String| 提供班次请求的发件人的用户 id。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.offerShiftRequest",
  "baseType": ""
}-->

```json
{
  "recipientActionDateTime": "String (timestamp)",
  "recipientActionMessage": "String",
  "recipientUserId": "String",
  "senderShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "offerShiftRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


