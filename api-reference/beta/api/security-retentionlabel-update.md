---
title: 更新 retentionLabel
description: 更新 retentionLabel 对象的属性。
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 717457b49b98074e72cffe4cec5b8fe5b36f54db
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447575"
---
# <a name="update-retentionlabel"></a>更新 retentionLabel
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [retentionLabel](../resources/security-retentionlabel.md) 对象的属性。

若要更新 [处置评审阶段](../resources/security-dispositionreviewstage.md)，请将 **actionAfterRetentionPeriod** 属性包含在请求正文中，其中指定了一个可能的值。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|RecordsManagement.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|RecordsManagement.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /security/labels/retentionLabels/{retentionLabelId}

```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|属性|类型|说明|
|:---|:---|:---|
|actionAfterRetentionPeriod|microsoft.graph.security.actionAfterRetentionPeriod| 指定要在保留期后对具有此标签的文档应用的操作。 可能的值包括 `none`、`delete`、`startDispositionReview`、`unknownFutureValue`。|
|behaviorDuringRetentionPeriod|microsoft.graph.security.behaviorDuringRetentionPeriod|指定在保留期内使用此标签的文档的行为。 可能的值包括 `doNotRetain`、`retain`、`retainAsRecord`、`retainAsRegulatoryRecord`、`unknownFutureValue`。|
|createdBy|[microsoft.graph.identitySet](/graph/api/resources/identityset)|表示创建 retentionLabel 的用户。|
|createdDateTime|DateTimeOffset|表示创建 retentionLabel 的日期和时间。|
|descriptionForAdmins|String|这是为管理员提供标签信息的可选属性。|
|descriptionForUsers|String|这是为用户提供标签信息的可选属性。|
|displayName|String|定义标签名称的唯一字符串。|
|dispositionReviewStages|[microsoft.graph.security.dispositionReviewStage](../resources/security-dispositionreviewstage.md) 集合|在审查阶段，审阅者将收到通知，以确定是必须删除还是保留文档。|
|id|String|retentionLabel 的唯一 ID。 [entity](/graph/api/resources/entity).|
|isInUse|Boolean|指定当前是否正在使用标签。|
|lastModifiedBy|[microsoft.graph.identitySet](/graph/api/resources/identityset)|上次修改 retentionLabel 的用户。|
|lastModifiedDateTime|DateTimeOffset|修改 retentionLabel 的最新日期时间。|
|retentionDuration|[microsoft.graph.security.retentionduration](../resources/security-retentionduration.md)|指定保留内容的天数。|
|retentionTrigger|microsoft.graph.security.retentionTrigger|指定保留期是从内容创建日期、标记日期还是上次修改日期计算的。 可能的值包括 `dateLabeled`、`dateCreated`、`dateModified`、`dateOfEvent`、`unknownFutureValue`。|
|defaultRecordBehavior|microsoft.graph.security.defaultRecordBehavior|指定创建记录标签时记录标签的锁定或解锁状态。可能的值为： `startLocked`， ， `startUnlocked`。 `unknownFutureValue`|
|labelToBeApplied|String|指定要在当前标签的保留期结束后自动应用的替换标签。 |



## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "update_retentionlabel"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/security/labels/retentionLabels/{retentionLabelId}
Content-Type: application/json
Content-length: 555

{
  "@odata.type": "#microsoft.graph.security.retentionLabel",
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
  "labelToBeApplied": "String",
  "defaultRecordBehavior": "String"
}
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.retentionLabel"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.security.retentionLabel",
  "id": "64a99fb4-07be-0481-8746-44c15c0eef1f",
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

