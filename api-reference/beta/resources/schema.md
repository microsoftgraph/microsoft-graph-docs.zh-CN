---
title: 架构资源类型
description: 介绍内容的类型，以及如何在 Microsoft Search 连接中对项目中的每个属性编制索引。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 77c17345a6a9408a8208f73f03dd98033f2b6a36
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704134"
---
# <a name="schema-resource-type"></a><span data-ttu-id="fc492-103">架构资源类型</span><span class="sxs-lookup"><span data-stu-id="fc492-103">schema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc492-104">介绍内容的类型，以及如何在 Microsoft Search[连接](externalconnection.md)中对项目中的每个属性编制索引。</span><span class="sxs-lookup"><span data-stu-id="fc492-104">Describes the type of content and how to index each property in items in a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="fc492-105">方法</span><span class="sxs-lookup"><span data-stu-id="fc492-105">Methods</span></span>

| <span data-ttu-id="fc492-106">方法</span><span class="sxs-lookup"><span data-stu-id="fc492-106">Method</span></span>                                                    | <span data-ttu-id="fc492-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="fc492-107">Return Type</span></span>                   | <span data-ttu-id="fc492-108">说明</span><span class="sxs-lookup"><span data-stu-id="fc492-108">Description</span></span> |
|:----------------------------------------------------------|:------------------------------|:--|
| [<span data-ttu-id="fc492-109">创建架构</span><span class="sxs-lookup"><span data-stu-id="fc492-109">Create schema</span></span>](../api/externalconnection-post-schema.md) | <span data-ttu-id="fc492-110">无*或*[架构](schema.md)</span><span class="sxs-lookup"><span data-stu-id="fc492-110">None *or* [schema](schema.md)</span></span> | <span data-ttu-id="fc492-111">注册连接架构。</span><span class="sxs-lookup"><span data-stu-id="fc492-111">Register connection schema.</span></span> |
| [<span data-ttu-id="fc492-112">获取架构</span><span class="sxs-lookup"><span data-stu-id="fc492-112">Get schema</span></span>](../api/schema-get.md)                        | [<span data-ttu-id="fc492-113">schema</span><span class="sxs-lookup"><span data-stu-id="fc492-113">schema</span></span>](schema.md)           | <span data-ttu-id="fc492-114">读取架构对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fc492-114">Read properties of a schema object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fc492-115">属性</span><span class="sxs-lookup"><span data-stu-id="fc492-115">Properties</span></span>

| <span data-ttu-id="fc492-116">属性</span><span class="sxs-lookup"><span data-stu-id="fc492-116">Property</span></span>   | <span data-ttu-id="fc492-117">类型</span><span class="sxs-lookup"><span data-stu-id="fc492-117">Type</span></span>                               | <span data-ttu-id="fc492-118">说明</span><span class="sxs-lookup"><span data-stu-id="fc492-118">Description</span></span>                |
|:-----------|:-----------------------------------|:---------------------------|
| <span data-ttu-id="fc492-119">#c1</span><span class="sxs-lookup"><span data-stu-id="fc492-119">baseType</span></span>   | <span data-ttu-id="fc492-120">String</span><span class="sxs-lookup"><span data-stu-id="fc492-120">String</span></span>                             | <span data-ttu-id="fc492-121">可能的值为 `microsoft.graph.externalItem` 和 `microsoft.graph.externalFile`。</span><span class="sxs-lookup"><span data-stu-id="fc492-121">Possible values are `microsoft.graph.externalItem` and `microsoft.graph.externalFile`.</span></span> <span data-ttu-id="fc492-122">必需。</span><span class="sxs-lookup"><span data-stu-id="fc492-122">Required.</span></span> |
| <span data-ttu-id="fc492-123">properties</span><span class="sxs-lookup"><span data-stu-id="fc492-123">properties</span></span> | <span data-ttu-id="fc492-124">[属性](property.md)集合</span><span class="sxs-lookup"><span data-stu-id="fc492-124">[property](property.md) collection</span></span> | <span data-ttu-id="fc492-125">为连接中的项目定义的属性。</span><span class="sxs-lookup"><span data-stu-id="fc492-125">The properties defined for the items in the connection.</span></span> <span data-ttu-id="fc492-126">最小属性数为1，最大值为64。</span><span class="sxs-lookup"><span data-stu-id="fc492-126">The minimum number of properties is one, the maximum is 64.</span></span> <span data-ttu-id="fc492-127">在设置`baseType`为`microsoft.graph.externalItem`时所需的。</span><span class="sxs-lookup"><span data-stu-id="fc492-127">Required when `baseType` is set to `microsoft.graph.externalItem`.</span></span> <span data-ttu-id="fc492-128">当设置`baseType`为时， `microsoft.graph.externalFile`将忽略。</span><span class="sxs-lookup"><span data-stu-id="fc492-128">Ignored when `baseType` is set to `microsoft.graph.externalFile`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fc492-129">关系</span><span class="sxs-lookup"><span data-stu-id="fc492-129">Relationships</span></span>

<span data-ttu-id="fc492-130">无</span><span class="sxs-lookup"><span data-stu-id="fc492-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc492-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc492-131">JSON representation</span></span>

<span data-ttu-id="fc492-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc492-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schema",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "baseType": "String",
  "id": "String (identifier)",
  "properties": [{"@odata.type": "microsoft.graph.property"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "schema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
