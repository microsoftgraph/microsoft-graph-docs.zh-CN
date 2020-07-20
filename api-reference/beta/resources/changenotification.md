---
title: changeNotification 资源类型
description: 表示发送给订阅者的更改通知。
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 5aa207fba6293db3ca1d0de4879639a4ea1c1b76
ms.sourcegitcommit: 41a5bd5868685c10181f6285d5ac91c6dad556e2
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/04/2020
ms.locfileid: "45038521"
---
# <a name="changenotification-resource-type"></a>changeNotification 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示发送给订阅者的通知。

有关详细信息，请参阅[使用 Microsoft GRAPH API 获取更改通知](webhooks.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| changeType | string | 指示将引发更改通知的更改的类型。 支持的值是：`created`、`updated`、`deleted`。 必需。 |
| clientState | string | 在订阅请求中指定的**clientState**属性的值（如果有）。 最大长度为 255 个字符。 客户端可以通过比较**clientState**属性的值，来检查更改通知是否来自服务。 与订阅一起发送的**clientState**属性的值将与每个更改通知收到的**clientState**属性的值进行比较。 可选。 |
| encryptedContent | [changeNotificationEncryptedContent](changenotificationencryptedcontent.md) | 预览随更改通知附加的加密内容。 仅当**encryptionCertificate**和**includeResourceData**在订阅请求期间定义并且资源支持它时才提供。 可选 |
| lifecycleEvent | string | 如果当前通知是生命周期通知，则为生命周期通知的类型。 可选。 支持的值为 `missed` 、 `removed` 、 `reauthorizationRequired` 。 |
| id | 字符串 | 通知的唯一 ID。 可选。 |
| resource | string | 发出更改通知的资源的 URI （相对于） `https://graph.microsoft.com` 。 必需。 |
| resourceData | [resourceData](resourcedata.md) | 此属性的内容取决于要订阅资源的类型。 必需。 |
| subscriptionExpirationDateTime | [dateTime](https://tools.ietf.org/html/rfc3339) | 订阅的过期时间。 必需。 |
| subscriptionId | string | 生成通知的订阅的唯一标识符。 |
| tenantId | containerparentjob | 来自其发出更改通知的租户的唯一标识符。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeNotification"
}-->

```json
{
  "subscriptionId": "76222963-cc7b-42d2-882d-8aaa69cb2ba3",
  "changeType": "created",
  "clientState": "client state provided when creating subscription",
  "id": "15ee1d1f-af7b-42d9-885b-9d00db065dd9",
  "tenantId": "2c937fad-a8a7-496c-b0e4-bf77dcc7eb2a",
  "subscriptionExpirationDateTime": "2020-04-12T23:20:50.52Z",
  "resource": "teams('d29828b8-c04d-4e2a-b2f6-07da6982f0f0')/channels('19:f127a8c55ad949d1a238464d22f0f99e@thread.skype')/messages('1565045424600')/replies('1565047490246')",
  "resourceData": {
    "id": "1565293727947",
    "@odata.type": "#Microsoft.Graph.ChatMessage",
    "@odata.id": "teams('88cbc8fc-164b-44f0-b6a6-b59b4a1559d3')/channels('19:8d9da062ec7647d4bb1976126e788b47@thread.tacv2')/messages('1565293727947')/replies('1565293727947')"
  }
}
```

<!-- uuid: 15ee1d1f-af7b-42d9-885b-9d00db065dd9
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "change notification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
