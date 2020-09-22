---
title: plannerExternalReferences 资源类型
description: '**PlannerExternalReferences**资源表示任务的引用集合。 这是开放类型。 它是任务详细信息对象的一部分。 属性-值对中的值是 externalReference 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: fc961bff401a16d74881210aa28e9fcb115e8ae1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067256"
---
# <a name="plannerexternalreferences-resource-type"></a><span data-ttu-id="63b7d-106">plannerExternalReferences 资源类型</span><span class="sxs-lookup"><span data-stu-id="63b7d-106">plannerExternalReferences resource type</span></span>

<span data-ttu-id="63b7d-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63b7d-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63b7d-108">**PlannerExternalReferences**资源表示任务的引用集合。</span><span class="sxs-lookup"><span data-stu-id="63b7d-108">The **plannerExternalReferences** resource represents the collection of references on a task.</span></span> <span data-ttu-id="63b7d-109">这是开放类型。</span><span class="sxs-lookup"><span data-stu-id="63b7d-109">This is an Open Type.</span></span> <span data-ttu-id="63b7d-110">它是 [任务详细信息](plannertaskdetails.md) 对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="63b7d-110">It is part of the [task details](plannertaskdetails.md) object.</span></span> <span data-ttu-id="63b7d-111">属性-值对中的值是 [externalReference](plannerexternalreference.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="63b7d-111">The value in the property-value pair is the [externalReference](plannerexternalreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="63b7d-112">属性</span><span class="sxs-lookup"><span data-stu-id="63b7d-112">Properties</span></span>
<span data-ttu-id="63b7d-113">可由客户端定义打开类型的属性。</span><span class="sxs-lookup"><span data-stu-id="63b7d-113">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="63b7d-114">在这种情况下，客户端必须提供基于**HTTP/HTTPS**协议的**有效 url**作为属性，并且它们的值必须是[externalReference](plannerexternalreference.md)对象。</span><span class="sxs-lookup"><span data-stu-id="63b7d-114">In this case, the client must provide **valid URLs** based on the **HTTP/HTTPS** protocols as properties and their values must be the [externalReference](plannerexternalreference.md) objects.</span></span> <span data-ttu-id="63b7d-115">根据 OData，开放式类型中的属性名称不能包含以下字符： `.` ， `:` ， `%`  因此需要对它们进行编码。</span><span class="sxs-lookup"><span data-stu-id="63b7d-115">Based on OData, property names in Open Types cannot contain the following characters: `.`, `:`, `%`  so they need to be encoded.</span></span> <span data-ttu-id="63b7d-116">示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="63b7d-116">Example is shown below.</span></span> <span data-ttu-id="63b7d-117">若要删除引用，请将属性的值设置为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="63b7d-117">To remove a reference, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="63b7d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63b7d-118">JSON representation</span></span>

<span data-ttu-id="63b7d-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63b7d-119">Here is a JSON representation of the resource</span></span>

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

<span data-ttu-id="63b7d-120">示例</span><span class="sxs-lookup"><span data-stu-id="63b7d-120">// Example</span></span>

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
  "suppressions": []
}
-->


