---
title: 请求资源类型
description: 一个抽象实体类型，用于对初始化的请求工作流进行建模以创建、更新和删除对象。
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fad1d480fbb792ca63b05ddfe8507b2ede9d54e8
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695249"
---
# <a name="request-resource-type"></a>请求资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一个抽象实体类型，用于对初始化的请求工作流进行建模以创建、更新和删除对象。

继承自 [实体](entity.md)。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|approvalId|String|请求审批的标识符。|
|completedDateTime|DateTimeOffset|请求完成日期时间。|
|createdBy|[identitySet](identityset.md)|创建此请求的用户。|
|createdDateTime|DateTimeOffset|请求创建日期时间。|
|customData|String|用于定义请求的任何自定义数据的免费文本字段。 未使用。|
|status|字符串|请求的状态。 不可为 null。 可能的值包括 `Canceled` `Denied` `Failed` `Granted` `PendingAdminDecision` `PendingApproval` ：、、、、、和 `PendingProvisioning` `PendingScheduleCreation` `Provisioned` `Revoked` `ScheduleCreated` 。 不可为空。|
|id|String|请求的标识符。 只读。 不可为 null。 继承自 [实体](entity.md)。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|审批|[审批](../resources/approval.md)|表示请求链接到的审批对象。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.request",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.request",
  "id": "String (identifier)",
  "approvalId": "String (identifier)",
  "completedDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "customData": "String",
  "status": "String",
}
```

