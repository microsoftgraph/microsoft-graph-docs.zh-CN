---
title: accessReviewNotificationRecipientItem 资源类型
description: 定义将接收通知的用户或组访问审阅通知。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7f63f9cfe3e1233407d0aaf966d9e2c0d933da26
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61649688"
---
# <a name="accessreviewnotificationrecipientitem-resource-type"></a>accessReviewNotificationRecipientItem 资源类型

命名空间：microsoft.graph

表示[Azure AD实例上的](accessreviewsv2-overview.md)访问评审通知事件。 此项目包含电子邮件模板类型和收件人属性，以允许发送给定访问评审实例的某些类型的 [通知](accessreviewinstance.md)。

## <a name="properties"></a>属性

| 属性                     | 类型     | 说明                          |
| :--------------------------- | :------  | :----------                          |
| notificationTemplateType  |String  | 指示要发送的访问评审电子邮件的类型。 支持的模板类型为 `CompletedAdditionalRecipients` ，用于向收件人发送审阅完成通知。|
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
