---
title: yammerActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 438cb55f4682d533876ef9a01561a3d69c4f1ea2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836650"
---
# <a name="yammeractivitysummary-resource-type"></a><span data-ttu-id="e9ba6-103">yammerActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="e9ba6-103">yammerActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e9ba6-104">属性</span><span class="sxs-lookup"><span data-stu-id="e9ba6-104">Properties</span></span>

| <span data-ttu-id="e9ba6-105">属性</span><span class="sxs-lookup"><span data-stu-id="e9ba6-105">Property</span></span>          | <span data-ttu-id="e9ba6-106">类型</span><span class="sxs-lookup"><span data-stu-id="e9ba6-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="e9ba6-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e9ba6-107">reportRefreshDate</span></span> | <span data-ttu-id="e9ba6-108">日期</span><span class="sxs-lookup"><span data-stu-id="e9ba6-108">Date</span></span>   |
| <span data-ttu-id="e9ba6-109">满意</span><span class="sxs-lookup"><span data-stu-id="e9ba6-109">liked</span></span>             | <span data-ttu-id="e9ba6-110">Int64</span><span class="sxs-lookup"><span data-stu-id="e9ba6-110">Int64</span></span>  |
| <span data-ttu-id="e9ba6-111">发布</span><span class="sxs-lookup"><span data-stu-id="e9ba6-111">posted</span></span>            | <span data-ttu-id="e9ba6-112">Int64</span><span class="sxs-lookup"><span data-stu-id="e9ba6-112">Int64</span></span>  |
| <span data-ttu-id="e9ba6-113">读取</span><span class="sxs-lookup"><span data-stu-id="e9ba6-113">read</span></span>              | <span data-ttu-id="e9ba6-114">Int64</span><span class="sxs-lookup"><span data-stu-id="e9ba6-114">Int64</span></span>  |
| <span data-ttu-id="e9ba6-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="e9ba6-115">reportDate</span></span>        | <span data-ttu-id="e9ba6-116">日期</span><span class="sxs-lookup"><span data-stu-id="e9ba6-116">Date</span></span>   |
| <span data-ttu-id="e9ba6-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e9ba6-117">reportPeriod</span></span>      | <span data-ttu-id="e9ba6-118">String</span><span class="sxs-lookup"><span data-stu-id="e9ba6-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e9ba6-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9ba6-119">JSON representation</span></span>

<span data-ttu-id="e9ba6-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9ba6-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "liked": 1024, 
  "posted": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
