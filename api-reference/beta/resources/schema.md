---
title: 架构资源类型
description: 介绍内容的类型，以及如何在 Microsoft Search 连接中对项目中的每个属性编制索引。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 40c31536f8d53c46563fda4205d34deee0501beb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520954"
---
# <a name="schema-resource-type"></a><span data-ttu-id="35e12-103">架构资源类型</span><span class="sxs-lookup"><span data-stu-id="35e12-103">schema resource type</span></span>

<span data-ttu-id="35e12-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="35e12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35e12-105">介绍内容的类型，以及如何在 Microsoft Search[连接](externalconnection.md)中对项目中的每个属性编制索引。</span><span class="sxs-lookup"><span data-stu-id="35e12-105">Describes the type of content and how to index each property in items in a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="35e12-106">方法</span><span class="sxs-lookup"><span data-stu-id="35e12-106">Methods</span></span>

| <span data-ttu-id="35e12-107">方法</span><span class="sxs-lookup"><span data-stu-id="35e12-107">Method</span></span>                                                    | <span data-ttu-id="35e12-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="35e12-108">Return Type</span></span>                   | <span data-ttu-id="35e12-109">说明</span><span class="sxs-lookup"><span data-stu-id="35e12-109">Description</span></span> |
|:----------------------------------------------------------|:------------------------------|:--|
| [<span data-ttu-id="35e12-110">创建架构</span><span class="sxs-lookup"><span data-stu-id="35e12-110">Create schema</span></span>](../api/externalconnection-post-schema.md) | <span data-ttu-id="35e12-111">无*或*[架构](schema.md)</span><span class="sxs-lookup"><span data-stu-id="35e12-111">None *or* [schema](schema.md)</span></span> | <span data-ttu-id="35e12-112">注册连接架构。</span><span class="sxs-lookup"><span data-stu-id="35e12-112">Register connection schema.</span></span> |
| [<span data-ttu-id="35e12-113">获取架构</span><span class="sxs-lookup"><span data-stu-id="35e12-113">Get schema</span></span>](../api/schema-get.md)                        | [<span data-ttu-id="35e12-114">schema</span><span class="sxs-lookup"><span data-stu-id="35e12-114">schema</span></span>](schema.md)           | <span data-ttu-id="35e12-115">读取架构对象的属性。</span><span class="sxs-lookup"><span data-stu-id="35e12-115">Read properties of a schema object.</span></span> |

## <a name="properties"></a><span data-ttu-id="35e12-116">属性</span><span class="sxs-lookup"><span data-stu-id="35e12-116">Properties</span></span>

| <span data-ttu-id="35e12-117">属性</span><span class="sxs-lookup"><span data-stu-id="35e12-117">Property</span></span>   | <span data-ttu-id="35e12-118">类型</span><span class="sxs-lookup"><span data-stu-id="35e12-118">Type</span></span>                               | <span data-ttu-id="35e12-119">说明</span><span class="sxs-lookup"><span data-stu-id="35e12-119">Description</span></span>                |
|:-----------|:-----------------------------------|:---------------------------|
| <span data-ttu-id="35e12-120">#c1</span><span class="sxs-lookup"><span data-stu-id="35e12-120">baseType</span></span>   | <span data-ttu-id="35e12-121">String</span><span class="sxs-lookup"><span data-stu-id="35e12-121">String</span></span>                             | <span data-ttu-id="35e12-122">可能的值为 `microsoft.graph.externalItem` 和 `microsoft.graph.externalFile`。</span><span class="sxs-lookup"><span data-stu-id="35e12-122">Possible values are `microsoft.graph.externalItem` and `microsoft.graph.externalFile`.</span></span> <span data-ttu-id="35e12-123">必填。</span><span class="sxs-lookup"><span data-stu-id="35e12-123">Required.</span></span> |
| <span data-ttu-id="35e12-124">properties</span><span class="sxs-lookup"><span data-stu-id="35e12-124">properties</span></span> | <span data-ttu-id="35e12-125">[属性](property.md)集合</span><span class="sxs-lookup"><span data-stu-id="35e12-125">[property](property.md) collection</span></span> | <span data-ttu-id="35e12-126">为连接中的项目定义的属性。</span><span class="sxs-lookup"><span data-stu-id="35e12-126">The properties defined for the items in the connection.</span></span> <span data-ttu-id="35e12-127">最小属性数为1，最大值为64。</span><span class="sxs-lookup"><span data-stu-id="35e12-127">The minimum number of properties is one, the maximum is 64.</span></span> <span data-ttu-id="35e12-128">在设置`baseType`为`microsoft.graph.externalItem`时所需的。</span><span class="sxs-lookup"><span data-stu-id="35e12-128">Required when `baseType` is set to `microsoft.graph.externalItem`.</span></span> <span data-ttu-id="35e12-129">当设置`baseType`为时， `microsoft.graph.externalFile`将忽略。</span><span class="sxs-lookup"><span data-stu-id="35e12-129">Ignored when `baseType` is set to `microsoft.graph.externalFile`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="35e12-130">关系</span><span class="sxs-lookup"><span data-stu-id="35e12-130">Relationships</span></span>

<span data-ttu-id="35e12-131">无</span><span class="sxs-lookup"><span data-stu-id="35e12-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35e12-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35e12-132">JSON representation</span></span>

<span data-ttu-id="35e12-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35e12-133">The following is a JSON representation of the resource.</span></span>

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
