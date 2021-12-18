---
title: educationSubmission 资源类型
description: 表示单个用户或 (组) 提交作业的资源，以及 (提交的结果（如成绩) 反馈）。
author: cristobal-buenrostro
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 64d5de98447327f67e659452cc58009e89320bed
ms.sourcegitcommit: 15dd0e98e69f872ed5a709600608b244759b0967
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2021
ms.locfileid: "61567403"
---
# <a name="educationsubmission-resource-type"></a>educationSubmission 资源类型

命名空间：microsoft.graph

表示单个用户或 (组) 为作业启用的资源，以及 (提交关联的成绩或) 反馈 [](educationassignment.md)等 **结果。**

提交归工作分配 **所有**。 发布作业时将自动 **创建** 提交。 **提交** 拥有两个资源列表。 资源表示用户/组工作区，而提交的资源表示学生已主动启用的资源。  

**status** 属性是只读的，并且对象通过操作在工作流中移动。 

如果尚未对 **educationSubmission** 资源调用 [setUpResourcesFolder，](../api/educationsubmission-setupResourcesFolder.md)**则 resourcesFolderUrl** 属性为 `null` 。

## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 educationSubmission](../api/educationsubmission-get.md) | [educationSubmission](educationsubmission.md) |读取 **educationSubmission** 对象的属性和关系。|
|[列出资源](../api/educationsubmission-list-resources.md) |[educationSubmissionResource](educationsubmissionresource.md) 集合| 获取 **educationSubmissionResource** 对象集合。|
|[列出 submittedResources](../api/educationsubmission-list-submittedresources.md) |[educationSubmissionResource](educationsubmissionresource.md) 集合| 获取 **educationSubmissionResource** 对象集合。|
|[列出结果](../api/educationsubmission-list-outcomes.md) |[educationOutcome](educationoutcome.md) 集合| 获取 **educationOutcome** 对象集合。|
|[return](../api/educationsubmission-return.md)|[educationSubmission](educationsubmission.md)|教师使用返回来指示可以向学生显示成绩/反馈。|
|[reassign](../api/educationsubmission-reassign.md)|[educationSubmission](educationsubmission.md)|将提交重新分配给学生并反馈评价。|
|[设置提交特定资源文件夹](../api/educationsubmission-setupResourcesFolder.md) |[educationSubmission](educationsubmission.md) | 在预定义SharePoint位置 (创建一个) 文件夹，以将文件作为提交资源上载。 |
|[提交](../api/educationsubmission-submit.md)|[educationSubmission](educationsubmission.md)|学生使用 submit 提交来提交 **作业**。 这会将资源复制到 **submittedResources** 文件夹中进行评分并更新状态。|
|[unsubmit](../api/educationsubmission-unsubmit.md)|[educationSubmission](educationsubmission.md)|学生使用取消提交将提交状态从提交后移回工作。 这会将资源复制到 **workingResources** 文件夹中进行评分并更新状态。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|recipient|[educationSubmissionRecipient](educationsubmissionrecipient.md)|Who分配此提交。|
|returnedBy|[identitySet](identityset.md)|将此提交的状态移至已返回的用户。|
|returnedDateTime|DateTimeOffset|提交返回的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|resourcesFolderUrl|String|需要存储此提交的所有文件资源的文件夹。|
|状态|string| 只读。 可能的值是 `working` `submitted` `released` ：、、、 `returned` 和 `reassigned` 。 请注意，必须使用此可变化枚举 (请求) 获取以下 `Prefer: include-unknown-enum-members` [值](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `reassigned` ： 。|
|submittedBy|[identitySet](identityset.md)|将资源移动到已提交状态的用户。|
|submittedDateTime|DateTimeOffset|提交移动到提交状态的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|unsubmittedBy|[identitySet](identityset.md)|将资源从提交移动到工作状态的用户。|
|unsubmittedDateTime|DateTimeOffset|将提交从提交移动到工作状态的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|reassignedBy|[identitySet](identityset.md)|移动了此提交状态以重新分配的用户。|
|reassignedDateTime|DateTimeOffset|重新分配提交的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|resources|[educationSubmissionResource](educationsubmissionresource.md) 集合| 可为 NULL。|
|submittedResources|[educationSubmissionResource](educationsubmissionresource.md) 集合| 只读。可为空。|
|outcomes|[educationOutcome](educationOutcome.md) 集合。 保留教师分配给此提交的成绩、反馈和/或评分标准信息|读写。 可为 Null。|

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


