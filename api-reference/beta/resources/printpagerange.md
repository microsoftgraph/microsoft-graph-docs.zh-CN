---
title: printPageRange 资源类型
description: 指定要打印的页面范围。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 65e2455438dbdb8c7bef3ef3439f846e737ebba0
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895598"
---
# <a name="printpagerange-resource-type"></a><span data-ttu-id="28823-103">printPageRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="28823-103">printPageRange resource type</span></span>

<span data-ttu-id="28823-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28823-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28823-105">指定要打印的页面范围。</span><span class="sxs-lookup"><span data-stu-id="28823-105">Specifies the range of pages to be printed.</span></span>

## <a name="properties"></a><span data-ttu-id="28823-106">属性</span><span class="sxs-lookup"><span data-stu-id="28823-106">Properties</span></span>
| <span data-ttu-id="28823-107">属性</span><span class="sxs-lookup"><span data-stu-id="28823-107">Property</span></span>     | <span data-ttu-id="28823-108">类型</span><span class="sxs-lookup"><span data-stu-id="28823-108">Type</span></span>        | <span data-ttu-id="28823-109">说明</span><span class="sxs-lookup"><span data-stu-id="28823-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="28823-110">startPage</span><span class="sxs-lookup"><span data-stu-id="28823-110">startPage</span></span>|<span data-ttu-id="28823-111">Int32</span><span class="sxs-lookup"><span data-stu-id="28823-111">Int32</span></span>|<span data-ttu-id="28823-112">区域的起始页（包含）。</span><span class="sxs-lookup"><span data-stu-id="28823-112">The start page (inclusive) for the range.</span></span> <span data-ttu-id="28823-113">只读。</span><span class="sxs-lookup"><span data-stu-id="28823-113">Read-only.</span></span>|
|<span data-ttu-id="28823-114">endPage</span><span class="sxs-lookup"><span data-stu-id="28823-114">endPage</span></span>|<span data-ttu-id="28823-115">Int32</span><span class="sxs-lookup"><span data-stu-id="28823-115">Int32</span></span>|<span data-ttu-id="28823-116">区域的结束页面（包含）。</span><span class="sxs-lookup"><span data-stu-id="28823-116">The end page (inclusive) for the range.</span></span> <span data-ttu-id="28823-117">只读。</span><span class="sxs-lookup"><span data-stu-id="28823-117">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="28823-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28823-118">JSON representation</span></span>

<span data-ttu-id="28823-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28823-119">The following is a JSON representation of the resource.</span></span>

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
