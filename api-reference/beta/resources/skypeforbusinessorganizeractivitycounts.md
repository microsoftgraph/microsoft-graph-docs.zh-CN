---
title: skypeForBusinessOrganizerActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 0729aef6367ebcb0a5edfaa461d80ffd8cb0775c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049494"
---
# <a name="skypeforbusinessorganizeractivitycounts-resource-type"></a><span data-ttu-id="7564c-103">skypeForBusinessOrganizerActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="7564c-103">skypeForBusinessOrganizerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7564c-104">属性</span><span class="sxs-lookup"><span data-stu-id="7564c-104">Properties</span></span>

| <span data-ttu-id="7564c-105">属性</span><span class="sxs-lookup"><span data-stu-id="7564c-105">Property</span></span>           | <span data-ttu-id="7564c-106">类型</span><span class="sxs-lookup"><span data-stu-id="7564c-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="7564c-107">im</span><span class="sxs-lookup"><span data-stu-id="7564c-107">im</span></span>                 | <span data-ttu-id="7564c-108">Int64</span><span class="sxs-lookup"><span data-stu-id="7564c-108">Int64</span></span>  |
| <span data-ttu-id="7564c-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="7564c-109">audioVideo</span></span>         | <span data-ttu-id="7564c-110">Int64</span><span class="sxs-lookup"><span data-stu-id="7564c-110">Int64</span></span>  |
| <span data-ttu-id="7564c-111">的</span><span class="sxs-lookup"><span data-stu-id="7564c-111">appSharing</span></span>         | <span data-ttu-id="7564c-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7564c-112">Int64</span></span>  |
| <span data-ttu-id="7564c-113">web</span><span class="sxs-lookup"><span data-stu-id="7564c-113">web</span></span>                | <span data-ttu-id="7564c-114">Int64</span><span class="sxs-lookup"><span data-stu-id="7564c-114">Int64</span></span>  |
| <span data-ttu-id="7564c-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="7564c-115">dialInOut3rdParty</span></span>  | <span data-ttu-id="7564c-116">Int64</span><span class="sxs-lookup"><span data-stu-id="7564c-116">Int64</span></span>  |
| <span data-ttu-id="7564c-117">dialInOutMicrosoft</span><span class="sxs-lookup"><span data-stu-id="7564c-117">dialInOutMicrosoft</span></span> | <span data-ttu-id="7564c-118">Int64</span><span class="sxs-lookup"><span data-stu-id="7564c-118">Int64</span></span>  |
| <span data-ttu-id="7564c-119">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7564c-119">reportRefreshDate</span></span>  | <span data-ttu-id="7564c-120">日期</span><span class="sxs-lookup"><span data-stu-id="7564c-120">Date</span></span>   |
| <span data-ttu-id="7564c-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="7564c-121">reportDate</span></span>         | <span data-ttu-id="7564c-122">日期</span><span class="sxs-lookup"><span data-stu-id="7564c-122">Date</span></span>   |
| <span data-ttu-id="7564c-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7564c-123">reportPeriod</span></span>       | <span data-ttu-id="7564c-124">String</span><span class="sxs-lookup"><span data-stu-id="7564c-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7564c-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7564c-125">JSON representation</span></span>

<span data-ttu-id="7564c-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7564c-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 1024, 
  "appSharing": 1024, 
  "web": 1024, 
  "dialInOut3rdParty": 1024, 
  "dialInOutMicrosoft": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
