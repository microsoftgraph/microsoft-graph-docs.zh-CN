---
title: educationSubmission 资源类型
description: 提交由工作分配拥有。 提交表示个人 (或组) 在工作分配和返回的评分/反馈中打开的资源。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 27467548339dc01f7c95fe55bda159c0569c38ba
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173039"
---
# <a name="educationsubmission-resource-type"></a>educationSubmission 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提交由工作分配拥有。 提交表示个人 (或组) 在工作分配和返回的评分/反馈中打开的资源。
发布工作分配时, 将自动创建提交。 提交内容拥有两个资源列表。 资源表示用户/组工作区, 而提交的资源代表学生已处于活动状态的资源。  

>**注意:** 状态为只读, 该对象通过操作在工作流中移动。 

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 educationSubmission](../api/educationsubmission-get.md) | [educationSubmission](educationsubmission.md) |读取**educationSubmission**对象的属性和关系。|
|[列出资源](../api/educationsubmission-list-resources.md) |[educationSubmissionResource](educationsubmissionresource.md)集合| 获取**educationSubmissionResource**对象集合。|
|[列出 submittedResources](../api/educationsubmission-list-submittedresources.md) |[educationSubmissionResource](educationsubmissionresource.md)集合| 获取**educationSubmissionResource**对象集合。|
|[列表结果](../api/educationsubmission-list-outcomes.md) |[educationOutcome](educationoutcome.md)集合| 获取**educationOutcome**对象集合。|
|[更新](../api/educationsubmission-update.md) | [educationSubmission](educationsubmission.md) |更新**educationSubmission**对象。 |
|[Return](../api/educationsubmission-return.md)|[educationSubmission](educationsubmission.md)|教师使用 return 来表示可以向学生显示成绩/反馈。|
|[Submit](../api/educationsubmission-submit.md)|[educationSubmission](educationsubmission.md)|学生使用提交来打开工作分配。 这将把资源复制到**submittedResources**文件夹进行评分并更新状态。|
|[Unsubmit](../api/educationsubmission-unsubmit.md)|[educationSubmission](educationsubmission.md)|学生使用 unsubmit 将提交状态移动回 "正在运行"。 这将把资源复制到**workingResources**文件夹进行评分并更新状态。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|反馈|[educationFeedback](educationfeedback.md)|保留反馈属性, 该属性将教师的备注存储回学生。|
|grade|[educationAssignmentGrade](educationassignmentgrade.md)|保留教师为此提交分配的年级信息。|
|id|String| 只读。|
|recipient|[educationSubmissionRecipient](educationsubmissionrecipient.md)|此提交被分配到的所有者。|
|releasedBy|[identitySet](identityset.md)|将此提交的状态移动到 "已发布" 的用户。|
|releasedDateTime|DateTimeOffset|提交发布的时间。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|returnedBy|[identitySet](identityset.md)|将此提交的状态移动到 "已返回" 的用户。|
|returnedDateTime|DateTimeOffset|返回提交的时间点。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|resourcesFolderUrl|String|需要存储此提交的所有文件资源的文件夹。|
|状态|string| 只读。 可取值为：`working`、`submitted`、`released`、`returned`。|
|submittedBy|[identitySet](identityset.md)|将资源移动到已提交状态的用户。|
|submittedDateTime|DateTimeOffset|将提交状态移至提交状态的时间点。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|unsubmittedBy|[identitySet](identityset.md)|移动资源的用户被提交到工作状态。|
|unsubmittedDateTime|DateTimeOffset|将提交的提交时间从提交到工作状态的时刻。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|resources|[educationSubmissionResource](educationsubmissionresource.md)集合| 可为 Null。|
|submittedResources|[educationSubmissionResource](educationsubmissionresource.md)集合| 只读。 可为 Null。|
|成果|[educationOutcome](educationOutcome.md)集合|只读。可为空。|

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
    "feedback":{"@odata.type":"microsoft.graph.educationFeedback"},
    "grade":{"@odata.type":"microsoft.graph.educationAssignmentGrade"},
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
    "releasedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "releasedDateTime":"String (timestamp)"
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
