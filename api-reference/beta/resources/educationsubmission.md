---
title: educationSubmission 资源类型
description: 表示单个 (或组) 为分配提交的资源，以及 (的结果，例如与提交关联的成绩或反馈) 。
author: cristobal-buenrostro
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 12618b5a852755f9c478896b6088aa1d6836a549
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685059"
---
# <a name="educationsubmission-resource-type"></a>educationSubmission 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示单个 (或组) 为 [分配](educationassignment.md) 而交 (的资源，以及与 **提交** 关联的成绩或反馈) 等结果。

提交归 **分配** 所有。 发布 **分配** 时会自动创建提交。 该 **提交** 拥有两个资源列表。 资源表示用户/组工作区，而提交的资源表示学生主动上交的资源。  

**状态** 属性为只读属性，对象通过操作在工作流中移动。 

如果未对 **educationSubmission** 资源调用 [setUpResourcesFolder](../api/educationsubmission-setupResourcesFolder.md)，则 **resourcesFolderUrl** 属性为 `null`。

## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 educationSubmission](../api/educationsubmission-get.md) | [educationSubmission](educationsubmission.md) |读取 **educationSubmission** 对象的属性和关系。|
|[列出资源](../api/educationsubmission-list-resources.md) |[educationSubmissionResource](educationsubmissionresource.md) 集合| 获取 **educationSubmissionResource** 对象集合。|
|[列出 submittedResources](../api/educationsubmission-list-submittedresources.md) |[educationSubmissionResource](educationsubmissionresource.md) 集合| 获取 **educationSubmissionResource** 对象集合。|
|[列出结果](../api/educationsubmission-list-outcomes.md) |[educationOutcome](educationoutcome.md) 集合| 获取 **educationOutcome** 对象集合。|
|[返回](../api/educationsubmission-return.md)|[educationSubmission](educationsubmission.md)|教师使用返回来指示可以向学生显示成绩/反馈。|
|[分配](../api/educationsubmission-reassign.md)|[educationSubmission](educationsubmission.md)|将提交重新分配给学生，并提供反馈以供审阅。|
|[设置提交特定资源文件夹](../api/educationsubmission-setupResourcesFolder.md) |[educationSubmission](educationsubmission.md) | 在预定义的位置下创建SharePoint文件夹 () 上传文件作为提交资源。 |
|[提交](../api/educationsubmission-submit.md)|[educationSubmission](educationsubmission.md)|学生使用 submit 来提交 **作业**。 这会将资源复制到 **submittedResources** 文件夹中进行评分并更新状态。|
|[unsubmit](../api/educationsubmission-unsubmit.md)|[educationSubmission](educationsubmission.md)|学生使用取消提交将提交状态从提交移回工作状态。 这会将资源复制到 **workingResources** 文件夹中进行评分并更新状态。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String|提交的唯一标识符。|
|recipient|[educationSubmissionRecipient](educationsubmissionrecipient.md)|Who此提交被分配到。|
|returnedBy|[identitySet](identityset.md)|将此提交状态移动到返回的用户。|
|returnedDateTime|DateTimeOffset|返回提交的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|resourcesFolderUrl|String|需要存储此提交的所有文件资源的文件夹。|
|状态|educationSubmissionStatus| 只读。 可能的值为：`working`、`submitted`、`released`和 `unknownFutureValue` `returned``reassigned`。 请注意，必须使用`Prefer: include-unknown-enum-members`请求标头获取以下值 (此[可旋转枚举](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)中的) ： `reassigned`|
|submittedBy|[identitySet](identityset.md)|将资源移动到提交状态的用户。|
|submittedDateTime|DateTimeOffset|提交进入提交状态的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|unsubmittedBy|[identitySet](identityset.md)|将资源从提交迁移到工作状态的用户。|
|unsubmittedDateTime|DateTimeOffset|提交从提交移动到工作状态的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|reassignedBy|[identitySet](identityset.md)|将此提交状态移动到重新分配的用户。|
|reassignedDateTime|DateTimeOffset|重新分配提交的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|resources|[educationSubmissionResource](educationsubmissionresource.md) 集合| 可为 NULL。|
|submittedResources|[educationSubmissionResource](educationsubmissionresource.md) 集合| 只读。可为空。|
|结果|[educationOutcome](educationOutcome.md) 集合。 保存教师为此提交分配的分数、反馈和/或标准信息|读写。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmission"
}-->

```json
{
    "id":"String (identifier)",
    "recipient":{"@odata.type":"microsoft.graph.educationSubmissionRecipient"},
    "returnedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "returnedDateTime":"String (timestamp)",
    "resourcesFolderUrl":"String",
    "status":"string",
    "submittedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "submittedDateTime":"String (timestamp)",
    "unsubmittedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "unsubmittedDateTime":"String (timestamp)",
    "reassignedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "reassignedDateTime":"String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


