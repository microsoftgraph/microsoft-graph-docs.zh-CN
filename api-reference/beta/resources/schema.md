---
title: 架构资源类型
description: 介绍内容的类型，以及如何在 Microsoft Search 连接中对项目中的每个属性编制索引。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c7780cd7c31da98a618053febba1b75c5e318931
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990263"
---
# <a name="schema-resource-type"></a><span data-ttu-id="12391-103">架构资源类型</span><span class="sxs-lookup"><span data-stu-id="12391-103">schema resource type</span></span>

<span data-ttu-id="12391-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12391-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12391-105">介绍内容的类型，以及如何在 Microsoft Search[连接](externalconnection.md)中对项目中的每个属性编制索引。</span><span class="sxs-lookup"><span data-stu-id="12391-105">Describes the type of content and how to index each property in items in a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="12391-106">方法</span><span class="sxs-lookup"><span data-stu-id="12391-106">Methods</span></span>

| <span data-ttu-id="12391-107">方法</span><span class="sxs-lookup"><span data-stu-id="12391-107">Method</span></span>                                                    | <span data-ttu-id="12391-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="12391-108">Return Type</span></span>                   | <span data-ttu-id="12391-109">说明</span><span class="sxs-lookup"><span data-stu-id="12391-109">Description</span></span> |
|:----------------------------------------------------------|:------------------------------|:--|
| [<span data-ttu-id="12391-110">创建架构</span><span class="sxs-lookup"><span data-stu-id="12391-110">Create schema</span></span>](../api/externalconnection-post-schema.md) | <span data-ttu-id="12391-111">无*或*[架构](schema.md)</span><span class="sxs-lookup"><span data-stu-id="12391-111">None *or* [schema](schema.md)</span></span> | <span data-ttu-id="12391-112">注册连接架构。</span><span class="sxs-lookup"><span data-stu-id="12391-112">Register connection schema.</span></span> |
| [<span data-ttu-id="12391-113">获取架构</span><span class="sxs-lookup"><span data-stu-id="12391-113">Get schema</span></span>](../api/schema-get.md)                        | [<span data-ttu-id="12391-114">schema</span><span class="sxs-lookup"><span data-stu-id="12391-114">schema</span></span>](schema.md)           | <span data-ttu-id="12391-115">读取架构对象的属性。</span><span class="sxs-lookup"><span data-stu-id="12391-115">Read properties of a schema object.</span></span> |

## <a name="properties"></a><span data-ttu-id="12391-116">属性</span><span class="sxs-lookup"><span data-stu-id="12391-116">Properties</span></span>

| <span data-ttu-id="12391-117">属性</span><span class="sxs-lookup"><span data-stu-id="12391-117">Property</span></span>   | <span data-ttu-id="12391-118">类型</span><span class="sxs-lookup"><span data-stu-id="12391-118">Type</span></span>                               | <span data-ttu-id="12391-119">说明</span><span class="sxs-lookup"><span data-stu-id="12391-119">Description</span></span>                |
|:-----------|:-----------------------------------|:---------------------------|
| <span data-ttu-id="12391-120">#c1</span><span class="sxs-lookup"><span data-stu-id="12391-120">baseType</span></span>   | <span data-ttu-id="12391-121">String</span><span class="sxs-lookup"><span data-stu-id="12391-121">String</span></span>                             | <span data-ttu-id="12391-122">必须设置为 `microsoft.graph.externalItem`。</span><span class="sxs-lookup"><span data-stu-id="12391-122">Must be set to `microsoft.graph.externalItem`.</span></span> <span data-ttu-id="12391-123">必需。</span><span class="sxs-lookup"><span data-stu-id="12391-123">Required.</span></span> |
| <span data-ttu-id="12391-124">properties</span><span class="sxs-lookup"><span data-stu-id="12391-124">properties</span></span> | <span data-ttu-id="12391-125">[属性](property.md)集合</span><span class="sxs-lookup"><span data-stu-id="12391-125">[property](property.md) collection</span></span> | <span data-ttu-id="12391-126">为连接中的项目定义的属性。</span><span class="sxs-lookup"><span data-stu-id="12391-126">The properties defined for the items in the connection.</span></span> <span data-ttu-id="12391-127">最小属性数为1，最大值为128。</span><span class="sxs-lookup"><span data-stu-id="12391-127">The minimum number of properties is one, the maximum is 128.</span></span> |

## <a name="relationships"></a><span data-ttu-id="12391-128">关系</span><span class="sxs-lookup"><span data-stu-id="12391-128">Relationships</span></span>

<span data-ttu-id="12391-129">无</span><span class="sxs-lookup"><span data-stu-id="12391-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="12391-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12391-130">JSON representation</span></span>

<span data-ttu-id="12391-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12391-131">The following is a JSON representation of the resource.</span></span>

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
