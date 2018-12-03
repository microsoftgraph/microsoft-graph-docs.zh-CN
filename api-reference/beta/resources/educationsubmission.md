---
title: educationSubmission 资源类型
description: 提交归工作分配。 提交表示的资源的个人 （或组） 打开中的工作分配和返回薪等级/反馈。
ms.openlocfilehash: f0b1cc9ccd169d29c31eb96bb6305f6d7cdcd6b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042145"
---
# <a name="educationsubmission-resource-type"></a>educationSubmission 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

提交归工作分配。 提交表示的资源的个人 （或组） 打开中的工作分配和返回薪等级/反馈。
发布工作分配时，会自动创建提交。 提交拥有资源的两个的列表。 资源表示工作区域时的提交的资源表示主动已打开学生的资源的用户/组。  

>**注意：** 状态是只读的并通过操作在工作流移动对象。 

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 educationSubmission](../api/educationsubmission-get.md) | [educationSubmission](educationsubmission.md) |读取属性和**educationSubmission**对象的关系。|
|[列表资源](../api/educationsubmission-list-resources.md) |[educationSubmissionResource](educationsubmissionresource.md)集合| 获取**educationSubmissionResource**对象集合。|
|[列表 submittedResources](../api/educationsubmission-list-submittedresources.md) |[educationSubmissionResource](educationsubmissionresource.md)集合| 获取**educationSubmissionResource**对象集合。|
|[Update](../api/educationsubmission-update.md) | [educationSubmission](educationsubmission.md) |更新**educationSubmission**对象。 |
|[Return](../api/educationsubmission-return.md)|[educationSubmission](educationsubmission.md)|教师使用返回指示可以向学生显示薪等级/反馈。|
|[Submit](../api/educationsubmission-submit.md)|[educationSubmission](educationsubmission.md)|使用提交以分配中启用的学生。 这会将资源复制到评分的**submittedResources**文件夹，并更新状态。|
|[Unsubmit](../api/educationsubmission-unsubmit.md)|[educationSubmission](educationsubmission.md)|学生使用 unsubmit 将提交的状态从提交后移至工作。 这会将资源复制到评分的**workingResources**文件夹，并更新状态。|

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|反馈|[educationFeedback](educationfeedback.md)|保留反馈属性存储回学生教师的注释。|
|grade|[educationAssignmentGrade](educationassignmentgrade.md)|包含教师将分配给此提交的薪等级信息。|
|id|String| 只读。|
|收件人|[educationSubmissionRecipient](educationsubmissionrecipient.md)|此提交被分配到。|
|releasedBy|[identitySet](identityset.md)|移动此提交释放的状态的用户。|
|releasedDateTime|DateTimeOffset|发布提交时时刻。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|returnedBy|[identitySet](identityset.md)|移动此提交返回的状态的用户。|
|returnedDateTime|DateTimeOffset|返回提交了时刻。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|resourcesFolderUrl|字符串|此提交的所有文件资源都需要存储的文件夹。|
|status|string| 只读。 可取值为：`working`、`submitted`、`released`、`returned`。|
|submittedBy|[identitySet](identityset.md)|移至提交状态的资源的用户。|
|submittedDateTime|DateTimeOffset|当提交已移至提交状态时刻。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|unsubmittedBy|[identitySet](identityset.md)|移动资源的用户从提交到运行状态。|
|unsubmittedDateTime|DateTimeOffset|当提交已移动从提交到工作状态时刻。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |Description|
|:---------------|:--------|:----------|
|resources|[educationSubmissionResource](educationsubmissionresource.md)集合| 可为 Null。|
|submittedResources|[educationSubmissionResource](educationsubmissionresource.md)集合| 只读。可为 NULL。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmission"
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.educationFeedback"},
  "grade": {"@odata.type": "microsoft.graph.educationAssignmentGrade"},
  "id": "String (identifier)",
  "recipient": {"@odata.type": "microsoft.graph.educationSubmissionRecipient"},
  "returnedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "returnedDateTime": "String (timestamp)",
  "resourcesFolderUrl": "String",
  "status": "string",
  "submittedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "submittedDateTime": "String (timestamp)",
  "unsubmittedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "unsubmittedDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->