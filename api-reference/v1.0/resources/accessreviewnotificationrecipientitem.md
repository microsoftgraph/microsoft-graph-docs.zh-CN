---
title: accessReviewNotificationRecipientItem 资源类型
description: 定义将接收通知的访问评审通知的用户或组。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 34b6f56f166fa972171467f89c06ac0090523fc1
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698378"
---
# <a name="accessreviewnotificationrecipientitem-resource-type"></a>accessReviewNotificationRecipientItem 资源类型

命名空间：microsoft.graph

表示审阅实例上的 Azure AD [访问评审](accessreviewsv2-overview.md) 通知事件。 此项包含电子邮件模板类型和收件人属性，用于为给定 [的访问评审实例](accessreviewinstance.md)发送特定类型的通知。

## <a name="properties"></a>属性

| 属性                     | 类型     | 说明                          |
| :--------------------------- | :------  | :----------                          |
| notificationTemplateType  |String  | 指示要发送的访问评审电子邮件的类型。 支持的模板类型是 `CompletedAdditionalRecipients`向收件人发送审阅完成通知。|
| notificationRecipientScope |[accessReviewNotificationRecipientScope](../resources/accessreviewnotificationrecipientscope.md)  | 确定通知电子邮件的收件人。|

## <a name="relationships"></a>关系
无。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewNotificationRecipientItem",
  "openType": true
}
-->

```json
{
  "@odata.type":"#microsoft.graph.accessReviewNotificationRecipientItem",
  "notificationRecipientScope": {
      "@odata.type":"#microsoft.graph.accessReviewNotificationRecipientQueryScope"                
    },
  "notificationTemplateType": "String"
}
```
