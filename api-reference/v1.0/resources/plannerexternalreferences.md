---
title: plannerExternalReferences 资源类型
description: '**PlannerExternalReferences**资源表示任务的引用集合。 这是开放类型。 它是任务详细信息对象的一部分。 属性-值对中的值是 externalReference 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 08e8a19db315846357feebb00a21f9572eea7fff
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2020
ms.locfileid: "48329988"
---
# <a name="plannerexternalreferences-resource-type"></a>plannerExternalReferences 资源类型

命名空间：microsoft.graph

**PlannerExternalReferences**资源表示任务的引用集合。 这是开放类型。 它是 [任务详细信息](plannertaskdetails.md) 对象的一部分。 属性-值对中的值是 [externalReference](plannerexternalreference.md) 对象。


## <a name="properties"></a>属性
可由客户端定义打开类型的属性。 在这种情况下，客户端必须提供基于**HTTP/HTTPS**协议的**有效 url**作为属性，并且它们的值必须是[externalReference](plannerexternalreference.md)对象。 根据 OData，开放式类型中的属性名称不能包含以下字符： `.` ， `:` ， `%`  因此需要对它们进行编码。 示例如下所示。 若要删除引用，请将属性的值设置为 `null` 。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
  "@odata.type": "microsoft.graph.plannerExternalReferences"
}-->


```json
{
  "String-value":
  {
    "alias": "String-value",
    "lastModifiedBy": "String-value",
    "lastModifiedDateTime": "String(timestamp)",
    "previewPriority": "String-value",
    "type": "String-value"
  }
}
```

## <a name="example"></a>示例

```json
{
  "https%3A//contoso%2Esharepoint%2Ecom/teams/agile/documents/AnnualReport%2Epptx":
  {
    "@odata.type": "microsoft.graph.externalReference", // required in PATCH requests to edit the references on a task
    "alias": "Agile Team Annual Report",
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedDateTime": "2015-09-21T17:45:12.039Z",
    "previewPriority": "0009005756397228702",
    "type": "PowerPoint"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

