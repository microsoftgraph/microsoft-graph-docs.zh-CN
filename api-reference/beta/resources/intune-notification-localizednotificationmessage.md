---
title: localizedNotificationMessage 资源类型
description: 指定区域设置的通知消息模板的文本内容。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 53a33c5d83821ff5131b601bd5687e7d98634c00
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825786"
---
# <a name="localizednotificationmessage-resource-type"></a>localizedNotificationMessage 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

指定区域设置的通知消息模板的文本内容。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 localizedNotificationMessages](../api/intune-notification-localizednotificationmessage-list.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 集合|列出 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性和关系。|
|[获取 localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-get.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|读取 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性和关系。|
|[创建 localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-create.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|创建新的 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。|
|[删除 localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-delete.md)|无|删除 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)。|
|[更新 localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-update.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|更新 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。|
|locale|String|此消息的目标区域设置。|
|subject|String|消息模板主题。|
|messageTemplate|String|消息模板内容。|
|isDefault|Boolean|用于指示这是否是语言回退的默认区域设置的标记。 此标志只能设置。 若要取消设置，请在其他本地化通知消息中将该属性设置为 true。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.localizedNotificationMessage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "locale": "String",
  "subject": "String",
  "messageTemplate": "String",
  "isDefault": true
}
```





