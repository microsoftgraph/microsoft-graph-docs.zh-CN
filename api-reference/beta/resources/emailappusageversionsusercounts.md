---
title: emailAppUsageVersionsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 2aff22c0ae1d3042859f3457f398ef5d0a5ffbe7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884845"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="159c3-103">emailAppUsageVersionsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="159c3-103">emailAppUsageVersionsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="159c3-104">属性</span><span class="sxs-lookup"><span data-stu-id="159c3-104">Properties</span></span>

| <span data-ttu-id="159c3-105">属性</span><span class="sxs-lookup"><span data-stu-id="159c3-105">Property</span></span>          | <span data-ttu-id="159c3-106">类型</span><span class="sxs-lookup"><span data-stu-id="159c3-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="159c3-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="159c3-107">reportRefreshDate</span></span> | <span data-ttu-id="159c3-108">日期</span><span class="sxs-lookup"><span data-stu-id="159c3-108">Date</span></span>   |
| <span data-ttu-id="159c3-109">outlook2016</span><span class="sxs-lookup"><span data-stu-id="159c3-109">outlook2016</span></span>       | <span data-ttu-id="159c3-110">Int64</span><span class="sxs-lookup"><span data-stu-id="159c3-110">Int64</span></span>  |
| <span data-ttu-id="159c3-111">outlook2013</span><span class="sxs-lookup"><span data-stu-id="159c3-111">outlook2013</span></span>       | <span data-ttu-id="159c3-112">Int64</span><span class="sxs-lookup"><span data-stu-id="159c3-112">Int64</span></span>  |
| <span data-ttu-id="159c3-113">outlook2010</span><span class="sxs-lookup"><span data-stu-id="159c3-113">outlook2010</span></span>       | <span data-ttu-id="159c3-114">Int64</span><span class="sxs-lookup"><span data-stu-id="159c3-114">Int64</span></span>  |
| <span data-ttu-id="159c3-115">outlook2007</span><span class="sxs-lookup"><span data-stu-id="159c3-115">outlook2007</span></span>       | <span data-ttu-id="159c3-116">Int64</span><span class="sxs-lookup"><span data-stu-id="159c3-116">Int64</span></span>  |
| <span data-ttu-id="159c3-117">无法确定</span><span class="sxs-lookup"><span data-stu-id="159c3-117">undetermined</span></span>      | <span data-ttu-id="159c3-118">Int64</span><span class="sxs-lookup"><span data-stu-id="159c3-118">Int64</span></span>  |
| <span data-ttu-id="159c3-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="159c3-119">reportPeriod</span></span>      | <span data-ttu-id="159c3-120">String</span><span class="sxs-lookup"><span data-stu-id="159c3-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="159c3-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="159c3-121">JSON representation</span></span>

<span data-ttu-id="159c3-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="159c3-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "outlook2016": 1024, 
  "outlook2013": 1024, 
  "outlook2010": 1024, 
  "outlook2007": 1024, 
  "undetermined": 1024, 
  "reportPeriod": "String"
}
```
