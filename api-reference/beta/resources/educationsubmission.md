---
title: educationSubmission 资源类型
description: 提交归工作分配所有。 提交表示单个用户或 (组) 为作业启用的资源以及返回的成绩/反馈。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 550e8329374865ce22954f1d25c977f877faf415
ms.sourcegitcommit: 40a8e4b9e344811267025e23c372a6e60e31a1b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/01/2021
ms.locfileid: "52119017"
---
# <a name="educationsubmission-resource-type"></a>educationSubmission 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提交归工作分配所有。 提交表示单个 (或组) 为作业启用的资源，以及 (与提交关联的成绩或) 反馈等结果。
发布作业时将自动创建提交。 提交拥有两个资源列表。 资源表示用户/组工作区，而提交的资源表示学生已主动启用的资源。  

>**注意：** 状态为只读，并且对象通过操作在工作流中移动。 

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 educationSubmission](../api/educationsubmission-get.md) | [educationSubmission](educationsubmission.md) |读取 **educationSubmission** 对象的属性和关系。|
|[列出资源](../api/educationsubmission-list-resources.md) |[educationSubmissionResource](educationsubmissionresource.md) 集合| 获取 **educationSubmissionResource** 对象集合。|
|[列出 submittedResources](../api/educationsubmission-list-submittedresources.md) |[educationSubmissionResource](educationsubmissionresource.md) 集合| 获取 **educationSubmissionResource** 对象集合。|
|[列出结果](../api/educationsubmission-list-outcomes.md) |[educationOutcome](educationoutcome.md) 集合| 获取 **educationOutcome** 对象集合。|
|[Return](../api/educationsubmission-return.md)|[educationSubmission](educationsubmission.md)|教师使用返回来指示可以向学生显示成绩/反馈。|
|[Submit](../api/educationsubmission-submit.md)|[educationSubmission](educationsubmission.md)|学生使用 submit 提交提交作业。 这会将资源复制到 **submittedResources** 文件夹中进行评分并更新状态。|
|[Unsubmit](../api/educationsubmission-unsubmit.md)|[educationSubmission](educationsubmission.md)|学生使用取消提交将提交状态从提交后移回工作。 这会将资源复制到 **workingResources** 文件夹中进行评分并更新状态。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|recipient|[educationSubmissionRecipient](educationsubmissionrecipient.md)|Who分配此提交。|
|releasedBy (已弃) |[identitySet](identityset.md)|将此提交的状态移至已发布的用户。|
|releasedDateTime (弃用) |DateTimeOffset|发布提交的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|returnedBy|[identitySet](identityset.md)|将此提交的状态移至已返回的用户。|
|returnedDateTime|DateTimeOffset|提交返回的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|resourcesFolderUrl|字符串|需要存储此提交的所有文件资源的文件夹。|
|状态|string| 只读。 可取值为：`working`、`submitted`、`released`、`returned`。|
|submittedBy|[identitySet](identityset.md)|将资源移动到已提交状态的用户。|
|submittedDateTime|DateTimeOffset|提交移动到提交状态的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|unsubmittedBy|[identitySet](identityset.md)|将资源从提交移动到工作状态的用户。|
|unsubmittedDateTime|DateTimeOffset|将提交从提交移动到工作状态的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|resources|[educationSubmissionResource](educationsubmissionresource.md) 集合| 可为 NULL。|
|submittedResources|[educationSubmissionResource](educationsubmissionresource.md) 集合| 只读。可为 NULL。|
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
    "unsubmittedDateTime":"String (timestamp)"
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


