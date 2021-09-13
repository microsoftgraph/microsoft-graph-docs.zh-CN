---
title: plannerExternalReferences 资源类型
description: '**plannerExternalReferences** 资源表示对任务的引用的集合。 这是"打开类型"。 它是任务详细信息对象的一部分。 属性值对中的值是 externalReference 对象。'
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: e1284f07b7efc1b43465b0f7e9e4c6d5de078698
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019263"
---
# <a name="plannerexternalreferences-resource-type"></a>plannerExternalReferences 资源类型

命名空间：microsoft.graph

**plannerExternalReferences** 资源表示对任务的引用的集合。 这是"打开类型"。 它是任务详细信息 [对象的一](plannertaskdetails.md) 部分。 属性值对中的值是 [externalReference](plannerexternalreference.md) 对象。


## <a name="properties"></a>属性
开放类型的属性可通过客户端定义。 在这种情况下，客户端必须提供基于 **HTTP/HTTPS** 协议的有效 **URL** 作为属性，并且其值必须是 [externalReference](plannerexternalreference.md)对象。 基于 OData，Open Types 中的属性名称不能包含下列字符 `.` `:` `%` `@` `#` ：、，因此需要对它们进行编码。 示例如下所示。 若要删除引用，将 属性的值设置为 `null` 。

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

