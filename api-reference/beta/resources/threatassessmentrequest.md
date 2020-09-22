---
title: threatAssessmentRequest 资源类型
description: 用于表示威胁评估请求项目的抽象资源类型。
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2435d1eef85dcdedc58b5e4e2be590759b779227
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988784"
---
# <a name="threatassessmentrequest-resource-type"></a>threatAssessmentRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于表示威胁评估请求项目的抽象资源类型。

威胁评估请求可以是以下类型之一：

* 邮件 ([mailAssessmentRequest](mailAssessmentRequest.md) 资源) 
* 电子邮件文件 ([emailFileAssessmentRequest](emailFileAssessmentRequest.md) 资源) 
* 文件 ([fileAssessmentRequest](fileAssessmentRequest.md) 资源) 
* [UrlAssessmentRequest](urlAssessmentRequest.md)资源的 URL () 

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 threatAssessmentRequest](../api/informationprotection-list-threatassessmentrequests.md) | [threatAssessmentRequest](threatassessmentrequest.md) 集合 | 列出租户下的所有威胁评估请求。 |
| [创建 threatAssessmentRequest](../api/informationprotection-post-threatassessmentrequests.md) | [threatAssessmentRequest](threatassessmentrequest.md) | 通过发布派生的资源类型创建新的威胁评估请求： [mailAssessmentRequest](../resources/mailAssessmentRequest.md)、 [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md)、 [fileAssessmentRequest](../resources/fileAssessmentRequest.md)、 [urlAssessmentRequest](../resources/urlAssessmentRequest.md)。 |
| [获取 threatAssessmentRequest](../api/threatassessmentrequest-get.md) | [threatAssessmentRequest](threatassessmentrequest.md) | 检索指定的 **threatAssessmentRequest** 资源的属性和关系。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
| :-------------|:------------|:------------|
|category|[threatCategory](enums.md#threatcategory-values)|威胁类别。 可取值为：`spam`、`phishing`、`malware`。|
|contentType|[threatAssessmentContentType](enums.md#threatassessmentcontenttype-values)|威胁评估的内容类型。 可取值为：`mail`、`url`、`file`。|
|createdBy|[identitySet](identityset.md)|威胁评估请求创建程序。|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|expectedAssessment|[threatExpectedAssessment](enums.md#threatexpectedassessment-values)|来自提交者的预期评估。 可能的值是：`block`、`unblock`。|
|id|String|威胁评估请求 ID 是 GUID)  (全局唯一标识符。|
|requestSource|[threatAssessmentRequestSource](enums.md#threatassessmentrequestsource-values)|威胁评估请求的来源。 可取值为：`user`、`administrator`。|
|状态|[threatAssessmentStatus](enums.md#threatassessmentstatus-values)|评估过程状态。 可取值为：`pending`、`completed`。|

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
  "@odata.type": "microsoft.graph.threatAssessmentRequest",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
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
  "description": "threatAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


