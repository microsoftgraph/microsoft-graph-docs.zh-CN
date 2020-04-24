---
title: externalItemContent 资源类型
description: 通过 Microsoft Search 连接编制索引的项目的内容。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: db0276307e824faa0c5606a8fb1212a0ad25e654
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805659"
---
# <a name="externalitemcontent-resource-type"></a><span data-ttu-id="d3612-103">externalItemContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3612-103">externalItemContent resource type</span></span>

<span data-ttu-id="d3612-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3612-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3612-105">通过 Microsoft Search[连接](externalconnection.md)编制索引的[externalItem](externalitem.md)的内容。</span><span class="sxs-lookup"><span data-stu-id="d3612-105">The content of an [externalItem](externalitem.md) indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="d3612-106">属性</span><span class="sxs-lookup"><span data-stu-id="d3612-106">Properties</span></span>

| <span data-ttu-id="d3612-107">属性</span><span class="sxs-lookup"><span data-stu-id="d3612-107">Property</span></span> | <span data-ttu-id="d3612-108">类型</span><span class="sxs-lookup"><span data-stu-id="d3612-108">Type</span></span>   | <span data-ttu-id="d3612-109">说明</span><span class="sxs-lookup"><span data-stu-id="d3612-109">Description</span></span>                                                                                 |
|:---------|:-------|:--------------------------------------------------------------------------------------------|
| <span data-ttu-id="d3612-110">值</span><span class="sxs-lookup"><span data-stu-id="d3612-110">value</span></span>    | <span data-ttu-id="d3612-111">String</span><span class="sxs-lookup"><span data-stu-id="d3612-111">String</span></span> | <span data-ttu-id="d3612-112">ExternalItem 的内容。</span><span class="sxs-lookup"><span data-stu-id="d3612-112">The content for the externalItem.</span></span> <span data-ttu-id="d3612-113">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="d3612-113">Required.</span></span>                                                 |
| <span data-ttu-id="d3612-114">type</span><span class="sxs-lookup"><span data-stu-id="d3612-114">type</span></span>     | <span data-ttu-id="d3612-115">字符串</span><span class="sxs-lookup"><span data-stu-id="d3612-115">String</span></span> | <span data-ttu-id="d3612-116">Value 属性中的内容类型。</span><span class="sxs-lookup"><span data-stu-id="d3612-116">The type of content in the value property.</span></span> <span data-ttu-id="d3612-117">可能的值为 `text` 和 `html`。</span><span class="sxs-lookup"><span data-stu-id="d3612-117">Possible values are `text` and `html`.</span></span> <span data-ttu-id="d3612-118">必需。</span><span class="sxs-lookup"><span data-stu-id="d3612-118">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d3612-119">关系</span><span class="sxs-lookup"><span data-stu-id="d3612-119">Relationships</span></span>

<span data-ttu-id="d3612-120">无</span><span class="sxs-lookup"><span data-stu-id="d3612-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3612-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3612-121">JSON representation</span></span>

<span data-ttu-id="d3612-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3612-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItemContent",
  "baseType": ""
}-->

```json
{
  "value": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalItemContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
