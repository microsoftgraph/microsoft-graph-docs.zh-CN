---
title: retentionLabel 资源类型
description: 表示客户如何管理其数据，无论保留还是删除数据的时间。
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 8e74f494b56c2a622510648953f1a021a32140c7
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447571"
---
# <a name="retentionlabel-resource-type"></a>retentionLabel 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示客户如何管理其数据，包括是否以及保留或删除数据的时间。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 retentionLabels](../api/security-retentionlabel-list.md)|[microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md) 集合|获取 [retentionLabel](../resources/security-retentionlabel.md) 对象及其属性的列表。|
|[创建 retentionLabel](../api/security-retentionlabel-post.md)|[microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md)|创建新的 [retentionLabel](../resources/security-retentionlabel.md) 对象。|
|[获取 retentionLabel](../api/security-retentionlabel-get.md)|[microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md)|读取 [retentionLabel](../resources/security-retentionlabel.md) 对象的属性和关系。|
|[更新 retentionLabel](../api/security-retentionlabel-update.md)|[microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md)|更新 [retentionLabel](../resources/security-retentionlabel.md) 对象的属性。|
|[删除 retentionLabel](../api/security-retentionlabel-delete.md)|无|删除 [retentionLabel](../resources/security-retentionlabel.md) 对象。|
|[列出 retentionEventType](../api/security-retentioneventtype-list.md)|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md) 集合|从 exapnd eventType 导航属性获取 retentionEventType 资源。|
|[添加 retentionEventType](../api/security-retentioneventtype-post.md)|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|通过在创建标签时添加相关的 odata 属性来添加 eventType。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|actionAfterRetentionPeriod|microsoft.graph.security.actionAfterRetentionPeriod| 指定在保留期内应用此标签的文档要执行的操作。 可能的值包括 `none`、`delete`、`startDispositionReview`、`unknownFutureValue`。|
|behaviorDuringRetentionPeriod|microsoft.graph.security.behaviorDuringRetentionPeriod|指定在保留期内使用此标签的文档的行为。 可能的值包括 `doNotRetain`、`retain`、`retainAsRecord`、`retainAsRegulatoryRecord`、`unknownFutureValue`。|
|createdBy|[microsoft.graph.identitySet](/graph/api/resources/identityset)|表示创建 retentionLabel 的用户。|
|createdDateTime|DateTimeOffset|表示创建 retentionLabel 的日期和时间。|
|descriptionForAdmins|String|为管理员提供标签信息。可选。|
|descriptionForUsers|String|为用户提供标签信息。 可选。|
|displayName|String|定义标签名称的唯一字符串。|
|dispositionReviewStages|[microsoft.graph.security.dispositionReviewStage](../resources/security-dispositionreviewstage.md) 集合|在审查阶段，审阅者将收到通知，以确定是必须删除还是保留文档。|
|id|String|retentionLabel 的唯一 ID。 [entity](/graph/api/resources/entity).|
|isInUse|Boolean|指定当前是否正在使用标签。|
|lastModifiedBy|[microsoft.graph.identitySet](/graph/api/resources/identityset)|上次修改 retentionLabel 的用户。|
|lastModifiedDateTime|DateTimeOffset|修改 retentionLabel 的最新日期时间。|
|retentionDuration|[microsoft.graph.security.retentionDuration](../resources/security-retentionduration.md)|指定保留内容的天数。|
|retentionTrigger|microsoft.graph.security.retentionTrigger|指定保留期是从内容创建日期、标记日期还是上次修改日期计算的。 可能的值包括 `dateLabeled`、`dateCreated`、`dateModified`、`dateOfEvent`、`unknownFutureValue`。|
|defaultRecordBehavior|microsoft.graph.security.defaultRecordBehavior|指定创建记录标签时记录标签的锁定或解锁状态。可能的值为： `startLocked`， ， `startUnlocked`。 `unknownFutureValue`|
|labelToBeApplied|String|指定要在当前标签的保留期结束后自动应用的替换标签。 |


## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|dispositionReviewStages|[microsoft.graph.security.dispositionReviewStage](../resources/security-dispositionreviewstage.md) 集合|当保留期末的操作选择为“dispositionReview”时，dispositionReviewStages 指定一组顺序阶段，每个阶段至少有一个审阅者。|
|eventType|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|表示与保留事件关联的类型。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.retentionLabel",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.retentionLabel",
  "id": "String (identifier)",
  "displayName": "String",
  "behaviorDuringRetentionPeriod": "String",
  "actionAfterRetentionPeriod": "String",
  "retentionTrigger": "String",
  "retentionDuration": {
    "@odata.type": "microsoft.graph.security.retentionDuration"
  },
  "isInUse": "Boolean",
  "descriptionForAdmins": "String",
  "descriptionForUsers": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "labelToBeApplied": "String",
  "defaultRecordBehavior": "String"
}
```
