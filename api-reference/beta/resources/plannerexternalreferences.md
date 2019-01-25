---
title: plannerExternalReferences 资源类型
description: '**plannerExternalReferences** 资源表示任务上的引用集合。它是开放类型。它是任务详细信息对象的组成部分。该属性-值对中的值是 externalReference 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 23ebd270bd97455ad09d67870c5fbb8fc37cd051
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516285"
---
# <a name="plannerexternalreferences-resource-type"></a><span data-ttu-id="dc556-106">plannerExternalReferences 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc556-106">plannerExternalReferences resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc556-p102">**plannerExternalReferences** 资源表示任务上的引用集合。它是开放类型。它是[任务详细信息](plannertaskdetails.md)对象的组成部分。该属性-值对中的值是 [externalReference](plannerexternalreference.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dc556-p102">The **plannerExternalReferences** resource represents the collection of references on a task. This is an Open Type. It is part of the [task details](plannertaskdetails.md) object. The value in the property-value pair is the [externalReference](plannerexternalreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="dc556-111">属性</span><span class="sxs-lookup"><span data-stu-id="dc556-111">Properties</span></span>
<span data-ttu-id="dc556-p103">开放类型的属性可以由客户端定义。在这种情况下，客户端必须根据 **HTTP/HTTPS** 协议提供**有效 URL** 来作为属性并且其值必须为 [externalReference](plannerexternalreference.md) 对象。根据 OData，开放类型的属性名称不能包含以下字符：`.`、`:`、`%`，因此需要将其编码。下面是一个示例。若要删除引用，请将该属性值设置为 `null`。</span><span class="sxs-lookup"><span data-stu-id="dc556-p103">Properties of an Open Type can be defined by the client. In this case, the client must provide **valid URLs** based on the **HTTP/HTTPS** protocols as properties and their values must be the [externalReference](plannerexternalreference.md) objects. Based on OData, property names in Open Types cannot contain the following characters: `.`, `:`, `%`  so they need to be encoded. Example is shown below. To remove a reference, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc556-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc556-117">JSON representation</span></span>

<span data-ttu-id="dc556-118">下面是资源的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc556-118">Here is a JSON representation of the resource</span></span>

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

<span data-ttu-id="dc556-119">// 示例</span><span class="sxs-lookup"><span data-stu-id="dc556-119">// Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerExternalReferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerexternalreferences.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
