---
title: changeNotification 资源类型
description: 表示发送给订阅者更改通知。
localization_priority: Normal
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: b5654e2b010b5cacd2f5a0ddfa2d95256abb1b02
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082319"
---
# <a name="changenotification-resource-type"></a>changeNotification 资源类型

命名空间：microsoft.graph

表示发送给订阅者的通知。

有关详细信息，请参阅 [Microsoft Graph API 通过更改通知](webhooks.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| changeType | changeType | 指示将引发更改通知的更改类型。 支持的值是：`created`、`updated`、`deleted`。 必填。 |
| clientState | string | 订阅请求请求中发送的 **clientState** (（如果有) ）。 最大长度为 255 个字符。 客户端可以通过比较 **clientState** 属性的值来检查更改通知是否来自服务。 与订阅一起发送的 **clientState** 属性的值与每次更改通知时收到的 **clientState** 属性的值进行比较。 可选。 |
| encryptedContent | [changeNotificationEncryptedContent](changenotificationencryptedcontent.md) |  (预览) 更改通知附加的加密内容。 仅在订阅 **请求期间定义了 encryptionCertificate** 和 **includeResourceData** 且资源支持它时提供。 可选。 |
| id | string | 通知的唯一 ID。 可选。 |
| lifecycleEvent | lifecycleEventType| 如果当前通知是生命周期通知，则生命周期通知的类型。 可选。 支持的值是 `missed` `removed` `reauthorizationRequired` 、、。 |
| resource | string | 发出更改通知的资源相对于 的 `https://graph.microsoft.com` URI。 必填。 |
| resourceData | [resourceData](resourcedata.md) | 此属性的内容取决于要订阅资源的类型。 必填。 |
| subscriptionExpirationDateTime | DateTimeOffset | 订阅的过期时间。 必填。 |
| subscriptionId | GUID | 生成通知的订阅的唯一标识符。 |
| tenantId | GUID | 源自更改通知的租户的唯一标识符。 |

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

