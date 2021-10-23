---
title: mailAssessmentRequest 资源类型
description: 用于创建和检索邮件威胁评估。
ms.localizationpriority: medium
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 83a2fb0fa5a309d880830a11f9806a729383b1d7
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60560826"
---
# <a name="mailassessmentrequest-resource-type"></a>mailAssessmentRequest 资源类型

用于创建和检索邮件威胁评估，派生自 [threatAssessmentRequest](threatAssessmentRequest.md)。

创建邮件威胁评估请求时，邮件应由 中指定的用户接收 `recipientEmail` 。 [Mail.Read](/graph/permissions-reference#mail-permissions) (Mail.Read 或 Mail.Read.Shared) 的委派邮件权限将重新进行quried，以访问用户接收或其他人共享的邮件。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建 threatAssessmentRequest](../api/informationprotection-post-threatassessmentrequests.md) | [mailAssessmentRequest](mailAssessmentRequest.md) | 通过发布 **mailAssessmentRequest** 对象创建新的邮件评估请求。 |
| [获取 threatAssessmentRequest](../api/threatassessmentrequest-get.md) | [mailAssessmentRequest](mailassessmentrequest.md) | 读取 **mailAssessmentRequest** 对象的属性和关系。 |


## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|destinationRoutingReason|[mailDestinationRoutingReason](enums.md#maildestinationroutingreason-values)|邮件路由到目标的原因。 可能的值是 `none` `mailFlowRule` `safeSender` ：、、、、、、、、、、 `blockedSender` `advancedSpamFiltering` `domainAllowList` `domainBlockList` `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` `junk` 。|
|messageUri|String|要评估的邮件的资源 URI。|
|recipientEmail|String|其策略用于评估邮件的邮件收件人。|
|“类别”|[threatCategory](enums.md#threatcategory-values)|威胁类别。 可取值为：`spam`、`phishing`、`malware`。|
|contentType|[threatAssessmentContentType](enums.md#threatassessmentcontenttype-values)|威胁评估的内容类型。 可取值为：`mail`、`url`、`file`。|
|createdBy|[identitySet](identityset.md)|威胁评估请求创建者。|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|expectedAssessment|[threatExpectedAssessment](enums.md#threatexpectedassessment-values)|提交者的预期评估。 可能的值是：`block`、`unblock`。|
|id|String|威胁评估请求 ID 是 GUID (全局唯) 。|
|requestSource|[threatAssessmentRequestSource](enums.md#threatassessmentrequestsource-values)|威胁评估请求的来源。 可能的值是 `administrator` ：。|
|status|[threatAssessmentStatus](enums.md#threatassessmentstatus-values)|评估流程状态。 可取值为：`pending`、`completed`。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|results|[threatAssessmentResult](threatassessmentresult.md) 集合|威胁评估结果的集合。 只读。 默认情况下， `GET /threatAssessmentRequests/{id}` 除非对该属性应用 ，否则 不会返回 `$expand` 此属性。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailAssessmentRequest",
  "keyProperty": "id"
}-->

```json
{
  "destinationRoutingReason": "String",
  "messageUri": "String",
  "recipientEmail": "String",
  "category": "String",
  "contentType": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "expectedAssessment": "String",
  "id": "String (identifier)",
  "requestSource": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

