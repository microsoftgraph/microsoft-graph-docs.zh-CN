---
title: plannerExternalReferences 资源类型
description: '**plannerExternalReferences** 资源表示任务上的引用集合。它是开放类型。它是任务详细信息对象的组成部分。该属性-值对中的值是 externalReference 对象。'
ms.openlocfilehash: cfd50c11956e421bd54bf29ad68a9c258f69cf20
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044759"
---
# <a name="plannerexternalreferences-resource-type"></a>plannerExternalReferences 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

**plannerExternalReferences** 资源表示任务上的引用集合。它是开放类型。它是[任务详细信息](plannertaskdetails.md)对象的组成部分。该属性-值对中的值是 [externalReference](plannerexternalreference.md) 对象。


## <a name="properties"></a>属性
开放类型的属性可以由客户端定义。在这种情况下，客户端必须根据 **HTTP/HTTPS** 协议提供**有效 URL** 来作为属性并且其值必须为 [externalReference](plannerexternalreference.md) 对象。根据 OData，开放类型的属性名称不能包含以下字符：`.`、`:`、`%`，因此需要将其编码。下面是一个示例。若要删除引用，请将该属性值设置为 `null`。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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

// 示例

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