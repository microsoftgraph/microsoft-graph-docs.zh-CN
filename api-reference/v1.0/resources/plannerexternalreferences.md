---
title: plannerExternalReferences 资源类型
description: '**plannerExternalReferences** 资源表示对任务的引用的集合。 这是"打开类型"。 它是任务详细信息对象的一部分。 属性值对中的值是 externalReference 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d4580d2e54b1f9b913b7dab5c283e9af7391b964
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473393"
---
# <a name="plannerexternalreferences-resource-type"></a><span data-ttu-id="743db-106">plannerExternalReferences 资源类型</span><span class="sxs-lookup"><span data-stu-id="743db-106">plannerExternalReferences resource type</span></span>

<span data-ttu-id="743db-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="743db-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="743db-108">**plannerExternalReferences** 资源表示对任务的引用的集合。</span><span class="sxs-lookup"><span data-stu-id="743db-108">The **plannerExternalReferences** resource represents the collection of references on a task.</span></span> <span data-ttu-id="743db-109">这是"打开类型"。</span><span class="sxs-lookup"><span data-stu-id="743db-109">This is an Open Type.</span></span> <span data-ttu-id="743db-110">它是任务详细信息 [对象的一](plannertaskdetails.md) 部分。</span><span class="sxs-lookup"><span data-stu-id="743db-110">It is part of the [task details](plannertaskdetails.md) object.</span></span> <span data-ttu-id="743db-111">属性值对中的值是 [externalReference](plannerexternalreference.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="743db-111">The value in the property-value pair is the [externalReference](plannerexternalreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="743db-112">属性</span><span class="sxs-lookup"><span data-stu-id="743db-112">Properties</span></span>
<span data-ttu-id="743db-113">开放类型的属性可以通过客户端定义。</span><span class="sxs-lookup"><span data-stu-id="743db-113">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="743db-114">在这种情况下，客户端必须提供基于 **HTTP/HTTPS** 协议的有效 **URL** 作为属性，并且其值必须是 [externalReference](plannerexternalreference.md)对象。</span><span class="sxs-lookup"><span data-stu-id="743db-114">In this case, the client must provide **valid URLs** based on the **HTTP/HTTPS** protocols as properties and their values must be the [externalReference](plannerexternalreference.md) objects.</span></span> <span data-ttu-id="743db-115">基于 OData，Open Types 中的属性名称不能包含下列字符 `.` `:` `%` `@` `#` ：、，因此需要编码它们。</span><span class="sxs-lookup"><span data-stu-id="743db-115">Based on OData, property names in Open Types cannot contain the following characters: `.`, `:`, `%`, `@`, `#` so they need to be encoded.</span></span> <span data-ttu-id="743db-116">示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="743db-116">Example is shown below.</span></span> <span data-ttu-id="743db-117">若要删除引用，将 属性的值设置为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="743db-117">To remove a reference, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="743db-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="743db-118">JSON representation</span></span>

<span data-ttu-id="743db-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="743db-119">Here is a JSON representation of the resource</span></span>

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

## <a name="example"></a><span data-ttu-id="743db-120">示例</span><span class="sxs-lookup"><span data-stu-id="743db-120">Example</span></span>

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

