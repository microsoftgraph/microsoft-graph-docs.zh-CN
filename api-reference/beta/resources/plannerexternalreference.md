---
title: plannerExternalReference 资源类型
description: '**PlannerExternalReference**资源表示 （例如文件，URL 附件） 的引用的元数据。 它是 externalReferences 对象中的属性值对的值。'
ms.openlocfilehash: ad892b5e9f9a741e7a4994c509ac704ad1ca62a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042399"
---
# <a name="plannerexternalreference-resource-type"></a>plannerExternalReference 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

**plannerExternalReference** 资源表示引用（文件、URL 等附件）的元数据。它是 [externalReferences 对象](plannerexternalreferences.md)的属性-值对的值。



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|alias|String|描述引用的别名。|
|lastModifiedBy|[identitySet](identityset.md)|只读。上一次修改它的用户 ID。|
|lastModifiedDateTime|DateTimeOffset|只读。上一次修改它的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|previewPriority|String|用于设置在任务上以预览形式显示引用的相对优先级顺序。|
|type|String|用于描述引用的类型。类型包括：`PowerPoint`、`Word`、`Excel`、`Other`。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReference"
}-->

```json
{
  "alias": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "previewPriority": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->