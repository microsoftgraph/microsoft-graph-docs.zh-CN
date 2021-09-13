---
title: offerShiftRequest 资源类型
description: 表示向团队中的其他用户转移的请求。
ms.localizationpriority: medium
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 10e96e9260f1027db87884bc8b01582fb7743a75
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094224"
---
# <a name="offershiftrequest-resource-type"></a>offerShiftRequest 资源类型

命名空间：microsoft.graph

表示向团队中的其他用户转移的请求。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [List](../api/offershiftrequest-list.md) | [offerShiftRequest 集合](offershiftrequest.md) | 读取团队中 **所有 offerShiftRequest** 对象的属性和关系。 |
| [Create](../api/offershiftrequest-post.md) | [offerShiftRequest](offershiftrequest.md) | 创建 **offerShiftRequest 对象** 的实例。 |
| [Get](../api/offershiftrequest-get.md) | [offerShiftRequest](offershiftrequest.md) | 读取 **offerShiftRequest** 对象的属性和关系。 |
|[批准](../api/offershiftrequest-approve.md)|无|批准 **offerShiftRequest**。 |
|[拒绝](../api/offershiftrequest-decline.md)|无|拒绝 **offerShiftRequest**。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|recipientActionDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z`|
|recipientActionMessage|String| 产品/服务班次请求的收件人发送的自定义邮件。 |
|recipientUserId|String| 产品/服务班次请求的收件人的用户 ID。|
|senderShiftId|String| 产品/服务班次请求发件人的用户 ID。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.offerShiftRequest"
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

