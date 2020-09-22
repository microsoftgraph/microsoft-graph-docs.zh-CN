---
title: printPageRange 资源类型
description: 指定要打印的页面范围。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: a8bbf452c337cb5c2ade7302eb29cff4bdb73d23
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052536"
---
# <a name="printpagerange-resource-type"></a><span data-ttu-id="42d31-103">printPageRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="42d31-103">printPageRange resource type</span></span>

<span data-ttu-id="42d31-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42d31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42d31-105">指定要打印的页面范围。</span><span class="sxs-lookup"><span data-stu-id="42d31-105">Specifies the range of pages to be printed.</span></span>

## <a name="properties"></a><span data-ttu-id="42d31-106">属性</span><span class="sxs-lookup"><span data-stu-id="42d31-106">Properties</span></span>
| <span data-ttu-id="42d31-107">属性</span><span class="sxs-lookup"><span data-stu-id="42d31-107">Property</span></span>     | <span data-ttu-id="42d31-108">类型</span><span class="sxs-lookup"><span data-stu-id="42d31-108">Type</span></span>        | <span data-ttu-id="42d31-109">说明</span><span class="sxs-lookup"><span data-stu-id="42d31-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="42d31-110">startPage</span><span class="sxs-lookup"><span data-stu-id="42d31-110">startPage</span></span>|<span data-ttu-id="42d31-111">Int32</span><span class="sxs-lookup"><span data-stu-id="42d31-111">Int32</span></span>|<span data-ttu-id="42d31-112">范围 (包含) 的起始页。</span><span class="sxs-lookup"><span data-stu-id="42d31-112">The start page (inclusive) for the range.</span></span> <span data-ttu-id="42d31-113">只读。</span><span class="sxs-lookup"><span data-stu-id="42d31-113">Read-only.</span></span>|
|<span data-ttu-id="42d31-114">endPage</span><span class="sxs-lookup"><span data-stu-id="42d31-114">endPage</span></span>|<span data-ttu-id="42d31-115">Int32</span><span class="sxs-lookup"><span data-stu-id="42d31-115">Int32</span></span>|<span data-ttu-id="42d31-116">区域 (包含) 的最后一页。</span><span class="sxs-lookup"><span data-stu-id="42d31-116">The end page (inclusive) for the range.</span></span> <span data-ttu-id="42d31-117">只读。</span><span class="sxs-lookup"><span data-stu-id="42d31-117">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42d31-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42d31-118">JSON representation</span></span>

<span data-ttu-id="42d31-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42d31-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printPageRange"
}-->

```json
{
  "startPage": 123456,
  "endPage": 123456
}
```


