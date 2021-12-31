---
title: accessReviewNotificationRecipientItem 资源类型
description: 定义将接收通知的用户或组访问审阅通知。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 00904cf1ac474d418629a0bba19d925698d72cf8
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650487"
---
# <a name="accessreviewnotificationrecipientitem-resource-type"></a>accessReviewNotificationRecipientItem 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]


表示Azure AD[实例](accessreviewsv2-overview.md)上的访问评审通知事件。 此项目包含电子邮件模板类型和收件人属性，以允许发送给定访问评审实例的某些类型的 [通知](accessreviewinstance.md)。

## <a name="properties"></a>属性

| 属性                     | 类型     | 说明                          |
| :--------------------------- | :------  | :----------                          |
| notificationTemplateType  |String  | 指示要发送的访问评审电子邮件的类型。 支持的模板类型 `CompletedAdditionalRecipients` 是向收件人发送审阅完成通知的类型。|
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
