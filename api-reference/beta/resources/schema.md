---
title: 架构资源类型
description: 介绍内容的类型，以及如何在 Microsoft Search 连接中对项目中的每个属性编制索引。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 2a13d797ff3b695250f7dd5cfef3bc077afe505b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870115"
---
# <a name="schema-resource-type"></a><span data-ttu-id="83a28-103">架构资源类型</span><span class="sxs-lookup"><span data-stu-id="83a28-103">schema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83a28-104">介绍内容的类型，以及如何在 Microsoft Search[连接](externalconnection.md)中对项目中的每个属性编制索引。</span><span class="sxs-lookup"><span data-stu-id="83a28-104">Describes the type of content and how to index each property in items in a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="83a28-105">方法</span><span class="sxs-lookup"><span data-stu-id="83a28-105">Methods</span></span>

| <span data-ttu-id="83a28-106">方法</span><span class="sxs-lookup"><span data-stu-id="83a28-106">Method</span></span>                                                    | <span data-ttu-id="83a28-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="83a28-107">Return Type</span></span>                   | <span data-ttu-id="83a28-108">说明</span><span class="sxs-lookup"><span data-stu-id="83a28-108">Description</span></span> |
|:----------------------------------------------------------|:------------------------------|:--|
| [<span data-ttu-id="83a28-109">创建架构</span><span class="sxs-lookup"><span data-stu-id="83a28-109">Create schema</span></span>](../api/externalconnection-post-schema.md) | <span data-ttu-id="83a28-110">无*或*[架构](schema.md)</span><span class="sxs-lookup"><span data-stu-id="83a28-110">None *or* [schema](schema.md)</span></span> | <span data-ttu-id="83a28-111">注册连接架构。</span><span class="sxs-lookup"><span data-stu-id="83a28-111">Register connection schema.</span></span> |
| [<span data-ttu-id="83a28-112">获取架构</span><span class="sxs-lookup"><span data-stu-id="83a28-112">Get schema</span></span>](../api/schema-get.md)                        | [<span data-ttu-id="83a28-113">schema</span><span class="sxs-lookup"><span data-stu-id="83a28-113">schema</span></span>](schema.md)           | <span data-ttu-id="83a28-114">读取架构对象的属性。</span><span class="sxs-lookup"><span data-stu-id="83a28-114">Read properties of a schema object.</span></span> |

## <a name="properties"></a><span data-ttu-id="83a28-115">属性</span><span class="sxs-lookup"><span data-stu-id="83a28-115">Properties</span></span>

| <span data-ttu-id="83a28-116">属性</span><span class="sxs-lookup"><span data-stu-id="83a28-116">Property</span></span>   | <span data-ttu-id="83a28-117">类型</span><span class="sxs-lookup"><span data-stu-id="83a28-117">Type</span></span>                               | <span data-ttu-id="83a28-118">说明</span><span class="sxs-lookup"><span data-stu-id="83a28-118">Description</span></span>                |
|:-----------|:-----------------------------------|:---------------------------|
| <span data-ttu-id="83a28-119">#c1</span><span class="sxs-lookup"><span data-stu-id="83a28-119">baseType</span></span>   | <span data-ttu-id="83a28-120">String</span><span class="sxs-lookup"><span data-stu-id="83a28-120">String</span></span>                             | <span data-ttu-id="83a28-121">可能的值为 `microsoft.graph.externalItem` 和 `microsoft.graph.externalFile`。</span><span class="sxs-lookup"><span data-stu-id="83a28-121">Possible values are `microsoft.graph.externalItem` and `microsoft.graph.externalFile`.</span></span> <span data-ttu-id="83a28-122">必需。</span><span class="sxs-lookup"><span data-stu-id="83a28-122">Required.</span></span> |
| <span data-ttu-id="83a28-123">properties</span><span class="sxs-lookup"><span data-stu-id="83a28-123">properties</span></span> | <span data-ttu-id="83a28-124">[属性](property.md)集合</span><span class="sxs-lookup"><span data-stu-id="83a28-124">[property](property.md) collection</span></span> | <span data-ttu-id="83a28-125">为连接中的项目定义的属性。</span><span class="sxs-lookup"><span data-stu-id="83a28-125">The properties defined for the items in the connection.</span></span> <span data-ttu-id="83a28-126">最小属性数为1，最大值为64。</span><span class="sxs-lookup"><span data-stu-id="83a28-126">The minimum number of properties is one, the maximum is 64.</span></span> <span data-ttu-id="83a28-127">在设置`baseType`为`microsoft.graph.externalItem`时所需的。</span><span class="sxs-lookup"><span data-stu-id="83a28-127">Required when `baseType` is set to `microsoft.graph.externalItem`.</span></span> <span data-ttu-id="83a28-128">当设置`baseType`为时， `microsoft.graph.externalFile`将忽略。</span><span class="sxs-lookup"><span data-stu-id="83a28-128">Ignored when `baseType` is set to `microsoft.graph.externalFile`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="83a28-129">关系</span><span class="sxs-lookup"><span data-stu-id="83a28-129">Relationships</span></span>

<span data-ttu-id="83a28-130">无</span><span class="sxs-lookup"><span data-stu-id="83a28-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83a28-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83a28-131">JSON representation</span></span>

<span data-ttu-id="83a28-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83a28-132">The following is a JSON representation of the resource.</span></span>

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
