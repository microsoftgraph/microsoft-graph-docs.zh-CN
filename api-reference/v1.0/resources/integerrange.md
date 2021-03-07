---
title: integerRange 资源类型
description: 表示由两个 Int64 边界描述的整数的包含范围。
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: aee4ebfab164e6abbbecde083ba028c4c5a98723
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516969"
---
# <a name="integerrange-resource-type"></a><span data-ttu-id="f187b-103">integerRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="f187b-103">integerRange resource type</span></span>

<span data-ttu-id="f187b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f187b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f187b-105">表示由两个 Int64 边界描述的整数的包含范围。</span><span class="sxs-lookup"><span data-stu-id="f187b-105">Represents an inclusive range of integers described by two Int64 boundaries.</span></span>

## <a name="properties"></a><span data-ttu-id="f187b-106">属性</span><span class="sxs-lookup"><span data-stu-id="f187b-106">Properties</span></span>
| <span data-ttu-id="f187b-107">属性</span><span class="sxs-lookup"><span data-stu-id="f187b-107">Property</span></span>     | <span data-ttu-id="f187b-108">类型</span><span class="sxs-lookup"><span data-stu-id="f187b-108">Type</span></span>        | <span data-ttu-id="f187b-109">Description</span><span class="sxs-lookup"><span data-stu-id="f187b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f187b-110">start</span><span class="sxs-lookup"><span data-stu-id="f187b-110">start</span></span>|<span data-ttu-id="f187b-111">Int64</span><span class="sxs-lookup"><span data-stu-id="f187b-111">Int64</span></span>|<span data-ttu-id="f187b-112">整数范围的包含下限。</span><span class="sxs-lookup"><span data-stu-id="f187b-112">The inclusive lower bound of the integer range.</span></span>|
|<span data-ttu-id="f187b-113">end</span><span class="sxs-lookup"><span data-stu-id="f187b-113">end</span></span>|<span data-ttu-id="f187b-114">Int64</span><span class="sxs-lookup"><span data-stu-id="f187b-114">Int64</span></span>|<span data-ttu-id="f187b-115">整数范围的包含上限。</span><span class="sxs-lookup"><span data-stu-id="f187b-115">The inclusive upper bound of the integer range.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f187b-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f187b-116">JSON representation</span></span>

<span data-ttu-id="f187b-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f187b-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.integerRange"
}
-->
```json
{
    "start": 12345,
    "end": 12345
}
```