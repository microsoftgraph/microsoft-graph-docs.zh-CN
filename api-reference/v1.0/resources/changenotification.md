---
title: changeNotification 资源类型
description: 表示发送给订阅者更改通知。
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 7ce05497382eb23d3137dd1e1bf2867b38e0095a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337150"
---
# <a name="changenotification-resource-type"></a>changeNotification 资源类型

命名空间：microsoft.graph

表示发送给订阅者的通知。 此资源的所有属性都是只读的。

有关详细信息，请参阅 [Microsoft Graph API 通过更改通知](webhooks.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| changeType | changeType | 指示将引发更改通知的更改类型。 支持的值是：`created`、`updated`、`deleted`。 必需项。 |
| clientState | string | 订阅请求请求中发送的 **clientState** (（如果有) ）。 最大长度为 255 个字符。 客户端可以通过比较 **clientState** 属性的值来检查更改通知是否来自服务。 与订阅一起发送的 **clientState** 属性的值与每次更改通知时收到的 **clientState** 属性的值进行比较。 可选。 |
| encryptedContent | [changeNotificationEncryptedContent](changenotificationencryptedcontent.md) |  (预览) 更改通知附加的加密内容。 仅在订阅 **请求期间定义了 encryptionCertificate** 和 **includeResourceData** 且资源支持它时提供。 可选。 |
| id | string | 通知的唯一 ID。 可选。 |
| lifecycleEvent | lifecycleEventType| 如果当前通知是生命周期通知，则生命周期通知的类型。 可选。 支持的值是 、`missed``subscriptionRemoved`、`reauthorizationRequired`。 可选。|
| resource | 字符串 | 发出更改通知的资源 `https://graph.microsoft.com`相对于 的 URI。 必需项。 |
| resourceData | [resourceData](resourcedata.md) | 此属性的内容取决于要订阅资源的类型。 可选。 |
| subscriptionExpirationDateTime | DateTimeOffset | 订阅的过期时间。 必需项。 |
| subscriptionId | Guid | 生成通知的订阅的唯一标识符。必填。 |
| tenantId | Guid | 发出更改通知的租户的唯一标识符。 必填。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.changeNotification"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.changeNotification",
  "id": "String (identifier)",
  "subscriptionId": "Guid",
  "subscriptionExpirationDateTime": "String (timestamp)",
  "clientState": "String",
  "changeType": "String",
  "resource": "String",
  "tenantId": "Guid",
  "encryptedContent": {
    "@odata.type": "microsoft.graph.changeNotificationEncryptedContent"
  },
  "lifecycleEvent": "String",
  "resourceData": {
    "@odata.type": "microsoft.graph.resourceData"
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

