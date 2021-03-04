---
author: swapnil1993
title: termColumn 资源类型
description: termColumn 资源指示列的值包含分类数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 6d29ec570d7f3fad798fb1e2ba213b5a998643dc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446614"
---
# <a name="termcolumn-resource-type"></a><span data-ttu-id="1bd1b-103">termColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="1bd1b-103">termColumn resource type</span></span>

<span data-ttu-id="1bd1b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bd1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="1bd1b-105">指示列的值包含分类数据。</span><span class="sxs-lookup"><span data-stu-id="1bd1b-105">Indicates that the column's values contains taxonomy data.</span></span>

## <a name="properties"></a><span data-ttu-id="1bd1b-106">属性</span><span class="sxs-lookup"><span data-stu-id="1bd1b-106">Properties</span></span>

| <span data-ttu-id="1bd1b-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="1bd1b-107">Property name</span></span> | <span data-ttu-id="1bd1b-108">类型</span><span class="sxs-lookup"><span data-stu-id="1bd1b-108">Type</span></span>   | <span data-ttu-id="1bd1b-109">说明</span><span class="sxs-lookup"><span data-stu-id="1bd1b-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="1bd1b-110">allowMultipleValues</span><span class="sxs-lookup"><span data-stu-id="1bd1b-110">allowMultipleValues</span></span> | <span data-ttu-id="1bd1b-111">布尔</span><span class="sxs-lookup"><span data-stu-id="1bd1b-111">Boolean</span></span> | <span data-ttu-id="1bd1b-112">指定列是否允许多个值</span><span class="sxs-lookup"><span data-stu-id="1bd1b-112">Specifies whether the column will allow more than one value</span></span>   
| <span data-ttu-id="1bd1b-113">parentTerm</span><span class="sxs-lookup"><span data-stu-id="1bd1b-113">parentTerm</span></span>     | <span data-ttu-id="1bd1b-114">microsoft.graph.termStore.term</span><span class="sxs-lookup"><span data-stu-id="1bd1b-114">microsoft.graph.termStore.term</span></span> | <span data-ttu-id="1bd1b-115">指定可选择其子项作为列值的术语 guid。</span><span class="sxs-lookup"><span data-stu-id="1bd1b-115">Specifies the term guid whose children can be selected as column's value.</span></span>  
| <span data-ttu-id="1bd1b-116">showFullyQualifiedName</span><span class="sxs-lookup"><span data-stu-id="1bd1b-116">showFullyQualifiedName</span></span> | <span data-ttu-id="1bd1b-117">布尔</span><span class="sxs-lookup"><span data-stu-id="1bd1b-117">Boolean</span></span> | <span data-ttu-id="1bd1b-118">指定是显示整个术语路径还是仅显示术语标签。</span><span class="sxs-lookup"><span data-stu-id="1bd1b-118">Specifies whether to display the entire term path or only the term label.</span></span>  
| <span data-ttu-id="1bd1b-119">termSet</span><span class="sxs-lookup"><span data-stu-id="1bd1b-119">termSet</span></span>      | <span data-ttu-id="1bd1b-120">microsoft.graph.termStore.set</span><span class="sxs-lookup"><span data-stu-id="1bd1b-120">microsoft.graph.termStore.set</span></span> | <span data-ttu-id="1bd1b-121">可以选择其子项作为列值的术语集。</span><span class="sxs-lookup"><span data-stu-id="1bd1b-121">Termset whose children can be selected as column's value.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="1bd1b-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1bd1b-122">JSON representation</span></span>

<span data-ttu-id="1bd1b-123">下面是 **termColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1bd1b-123">Here is a JSON representation of a **termColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.termColumn" } -->

```json
{
    "allowMultipleValues": true,
    "parentTerm": { "@type": "microsoft.graph.termStore.term" },
    "showFullyQualifiedName": false,
    "termSet": { "@type": "microsoft.graph.termStore.set" }
}
```

