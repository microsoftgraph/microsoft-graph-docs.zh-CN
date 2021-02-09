---
title: 架构资源类型
description: 连接架构确定添加到连接的内容如何用于各种 Microsoft Graph 体验。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 88509a885a528f9ef2d55cd84381db493e128003
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156355"
---
# <a name="schema-resource-type"></a><span data-ttu-id="d0065-103">架构资源类型</span><span class="sxs-lookup"><span data-stu-id="d0065-103">schema resource type</span></span>

<span data-ttu-id="d0065-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0065-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0065-105">连接 [架构](externalconnection.md) 确定外部内容在各种 Microsoft Graph 体验中的使用方式。</span><span class="sxs-lookup"><span data-stu-id="d0065-105">The [connection](externalconnection.md) schema determines how your external content will be used in various Microsoft Graph experiences.</span></span> <span data-ttu-id="d0065-106">架构是计划添加到连接中的所有属性的简单列表及其属性、标签和别名。</span><span class="sxs-lookup"><span data-stu-id="d0065-106">Schema is a flat list of all the properties that you plan to add to the connection along with their attributes, labels, and aliases.</span></span> <span data-ttu-id="d0065-107">向连接添加项目前，必须注册架构。</span><span class="sxs-lookup"><span data-stu-id="d0065-107">You must register the schema before adding items into the connection.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="d0065-108">方法</span><span class="sxs-lookup"><span data-stu-id="d0065-108">Methods</span></span>

| <span data-ttu-id="d0065-109">方法</span><span class="sxs-lookup"><span data-stu-id="d0065-109">Method</span></span>                                                    | <span data-ttu-id="d0065-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d0065-110">Return Type</span></span>                   | <span data-ttu-id="d0065-111">说明</span><span class="sxs-lookup"><span data-stu-id="d0065-111">Description</span></span> |
|:----------------------------------------------------------|:------------------------------|:--|
| [<span data-ttu-id="d0065-112">创建架构</span><span class="sxs-lookup"><span data-stu-id="d0065-112">Create schema</span></span>](../api/externalconnection-post-schema.md) | <span data-ttu-id="d0065-113">无 *或*[架构](schema.md)</span><span class="sxs-lookup"><span data-stu-id="d0065-113">None *or* [schema](schema.md)</span></span> | <span data-ttu-id="d0065-114">注册连接架构。</span><span class="sxs-lookup"><span data-stu-id="d0065-114">Register connection schema.</span></span> |
| [<span data-ttu-id="d0065-115">获取架构</span><span class="sxs-lookup"><span data-stu-id="d0065-115">Get schema</span></span>](../api/schema-get.md)                        | [<span data-ttu-id="d0065-116">schema</span><span class="sxs-lookup"><span data-stu-id="d0065-116">schema</span></span>](schema.md)           | <span data-ttu-id="d0065-117">读取架构对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d0065-117">Read properties of a schema object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d0065-118">属性</span><span class="sxs-lookup"><span data-stu-id="d0065-118">Properties</span></span>

| <span data-ttu-id="d0065-119">属性</span><span class="sxs-lookup"><span data-stu-id="d0065-119">Property</span></span>   | <span data-ttu-id="d0065-120">类型</span><span class="sxs-lookup"><span data-stu-id="d0065-120">Type</span></span>                               | <span data-ttu-id="d0065-121">说明</span><span class="sxs-lookup"><span data-stu-id="d0065-121">Description</span></span>                |
|:-----------|:-----------------------------------|:---------------------------|
| <span data-ttu-id="d0065-122">baseType</span><span class="sxs-lookup"><span data-stu-id="d0065-122">baseType</span></span>   | <span data-ttu-id="d0065-123">String</span><span class="sxs-lookup"><span data-stu-id="d0065-123">String</span></span>                             | <span data-ttu-id="d0065-124">必须设置为 `microsoft.graph.externalItem`。</span><span class="sxs-lookup"><span data-stu-id="d0065-124">Must be set to `microsoft.graph.externalItem`.</span></span> <span data-ttu-id="d0065-125">必需。</span><span class="sxs-lookup"><span data-stu-id="d0065-125">Required.</span></span> |
| <span data-ttu-id="d0065-126">properties</span><span class="sxs-lookup"><span data-stu-id="d0065-126">properties</span></span> | <span data-ttu-id="d0065-127">[property](property.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d0065-127">[property](property.md) collection</span></span> | <span data-ttu-id="d0065-128">为连接中的项目定义的属性。</span><span class="sxs-lookup"><span data-stu-id="d0065-128">The properties defined for the items in the connection.</span></span> <span data-ttu-id="d0065-129">最小属性数为 1，最大值为 128。</span><span class="sxs-lookup"><span data-stu-id="d0065-129">The minimum number of properties is one, the maximum is 128.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d0065-130">关系</span><span class="sxs-lookup"><span data-stu-id="d0065-130">Relationships</span></span>

<span data-ttu-id="d0065-131">无</span><span class="sxs-lookup"><span data-stu-id="d0065-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0065-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0065-132">JSON representation</span></span>

<span data-ttu-id="d0065-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0065-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schema",
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


