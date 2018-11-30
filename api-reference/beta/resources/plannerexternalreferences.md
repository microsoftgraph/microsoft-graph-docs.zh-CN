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
# <a name="plannerexternalreferences-resource-type"></a><span data-ttu-id="ca241-106">plannerExternalReferences 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca241-106">plannerExternalReferences resource type</span></span>

> <span data-ttu-id="ca241-107">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ca241-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca241-108">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ca241-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca241-p103">**plannerExternalReferences** 资源表示任务上的引用集合。它是开放类型。它是[任务详细信息](plannertaskdetails.md)对象的组成部分。该属性-值对中的值是 [externalReference](plannerexternalreference.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ca241-p103">The **plannerExternalReferences** resource represents the collection of references on a task. This is an Open Type. It is part of the [task details](plannertaskdetails.md) object. The value in the property-value pair is the [externalReference](plannerexternalreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="ca241-113">属性</span><span class="sxs-lookup"><span data-stu-id="ca241-113">Properties</span></span>
<span data-ttu-id="ca241-p104">开放类型的属性可以由客户端定义。在这种情况下，客户端必须根据 **HTTP/HTTPS** 协议提供**有效 URL** 来作为属性并且其值必须为 [externalReference](plannerexternalreference.md) 对象。根据 OData，开放类型的属性名称不能包含以下字符：`.`、`:`、`%`，因此需要将其编码。下面是一个示例。若要删除引用，请将该属性值设置为 `null`。</span><span class="sxs-lookup"><span data-stu-id="ca241-p104">Properties of an Open Type can be defined by the client. In this case, the client must provide **valid URLs** based on the **HTTP/HTTPS** protocols as properties and their values must be the [externalReference](plannerexternalreference.md) objects. Based on OData, property names in Open Types cannot contain the following characters: `.`, `:`, `%`  so they need to be encoded. Example is shown below. To remove a reference, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca241-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca241-119">JSON representation</span></span>

<span data-ttu-id="ca241-120">下面是资源的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca241-120">Here is a JSON representation of the resource</span></span>

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

<span data-ttu-id="ca241-121">// 示例</span><span class="sxs-lookup"><span data-stu-id="ca241-121">// Example</span></span>

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