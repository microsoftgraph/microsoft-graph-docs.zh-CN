---
title: yammerGroupsActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: f8a205c2ecd74e8543a220508e7d4110a90317cc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806788"
---
# <a name="yammergroupsactivitycounts-resource-type"></a><span data-ttu-id="7ef35-103">yammerGroupsActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ef35-103">yammerGroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7ef35-104">属性</span><span class="sxs-lookup"><span data-stu-id="7ef35-104">Properties</span></span>

| <span data-ttu-id="7ef35-105">属性</span><span class="sxs-lookup"><span data-stu-id="7ef35-105">Property</span></span>          | <span data-ttu-id="7ef35-106">类型</span><span class="sxs-lookup"><span data-stu-id="7ef35-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="7ef35-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7ef35-107">reportRefreshDate</span></span> | <span data-ttu-id="7ef35-108">日期</span><span class="sxs-lookup"><span data-stu-id="7ef35-108">Date</span></span>   |
| <span data-ttu-id="7ef35-109">满意</span><span class="sxs-lookup"><span data-stu-id="7ef35-109">liked</span></span>             | <span data-ttu-id="7ef35-110">Int64</span><span class="sxs-lookup"><span data-stu-id="7ef35-110">Int64</span></span>  |
| <span data-ttu-id="7ef35-111">发布</span><span class="sxs-lookup"><span data-stu-id="7ef35-111">posted</span></span>            | <span data-ttu-id="7ef35-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7ef35-112">Int64</span></span>  |
| <span data-ttu-id="7ef35-113">读取</span><span class="sxs-lookup"><span data-stu-id="7ef35-113">read</span></span>              | <span data-ttu-id="7ef35-114">Int64</span><span class="sxs-lookup"><span data-stu-id="7ef35-114">Int64</span></span>  |
| <span data-ttu-id="7ef35-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="7ef35-115">reportDate</span></span>        | <span data-ttu-id="7ef35-116">日期</span><span class="sxs-lookup"><span data-stu-id="7ef35-116">Date</span></span>   |
| <span data-ttu-id="7ef35-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7ef35-117">reportPeriod</span></span>      | <span data-ttu-id="7ef35-118">String</span><span class="sxs-lookup"><span data-stu-id="7ef35-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7ef35-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ef35-119">JSON representation</span></span>

<span data-ttu-id="7ef35-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ef35-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityCounts"
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
