---
title: mailAssessmentRequest 资源类型
description: 用于创建和检索邮件威胁评估。
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c684694ac2af189698c74935ca58f70aa4a8cf9f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083076"
---
# <a name="mailassessmentrequest-resource-type"></a>mailAssessmentRequest 资源类型

用于创建和检索从 [threatAssessmentRequest](threatAssessmentRequest.md)派生的邮件威胁评估。

当您创建邮件威胁评估请求时，邮件应由中指定的用户接收 `recipientEmail` 。 委派的 [邮件权限](/graph/permissions-reference#mail-permissions) (mail. Read 或 Mail. Shared) 是 requried，用于访问用户接收的邮件或由其他人共享的邮件。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建 threatAssessmentRequest](../api/informationprotection-post-threatassessmentrequests.md) | [mailAssessmentRequest](mailAssessmentRequest.md) | 通过发布 **mailAssessmentRequest** 对象创建新的邮件评估请求。 |
| [获取 threatAssessmentRequest](../api/threatassessmentrequest-get.md) | [mailAssessmentRequest](mailassessmentrequest.md) | 读取 **mailAssessmentRequest** 对象的属性和关系。 |


## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|destinationRoutingReason|[mailDestinationRoutingReason](enums.md#maildestinationroutingreason-values)|邮件路由到其目标的原因。 可能的值为：、、、、、、、、、、、、、、 `none` `mailFlowRule` `safeSender` `blockedSender` `advancedSpamFiltering` `domainAllowList` `domainBlockList` `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` `junk` 。|
|messageUri|String|要进行评估的邮件邮件的资源 URI。|
|recipientEmail|String|其策略用于评估邮件的邮件收件人。|
|“类别”|[threatCategory](enums.md#threatcategory-values)|威胁类别。 可取值为：`spam`、`phishing`、`malware`。|
|contentType|[threatAssessmentContentType](enums.md#threatassessmentcontenttype-values)|威胁评估的内容类型。 可取值为：`mail`、`url`、`file`。|
|createdBy|[identitySet](identityset.md)|威胁评估请求创建程序。|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|expectedAssessment|[threatExpectedAssessment](enums.md#threatexpectedassessment-values)|来自提交者的预期评估。 可能的值是：`block`、`unblock`。|
|id|String|威胁评估请求 ID 是 GUID)  (全局唯一标识符。|
|requestSource|[threatAssessmentRequestSource](enums.md#threatassessmentrequestsource-values)|威胁评估请求的来源。 可取值为：`user`、`administrator`。|
|status|[threatAssessmentStatus](enums.md#threatassessmentstatus-values)|评估过程状态。 可取值为：`pending`、`completed`。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|results|[threatAssessmentResult](threatassessmentresult.md) 集合|威胁评估结果的集合。 只读。 默认情况下，a 不 `GET /threatAssessmentRequests/{id}` 会返回此属性，除非您应用于该属性 `$expand` 。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailAssessmentRequest",
  "baseType": "",
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

