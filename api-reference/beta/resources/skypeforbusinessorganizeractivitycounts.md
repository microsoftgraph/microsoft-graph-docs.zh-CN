---
title: skypeForBusinessOrganizerActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 9f6c77e86f76ac2e34fb87cf8ca5b6bded35a2a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866617"
---
# <a name="skypeforbusinessorganizeractivitycounts-resource-type"></a><span data-ttu-id="ec0b0-103">skypeForBusinessOrganizerActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="ec0b0-103">skypeForBusinessOrganizerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ec0b0-104">属性</span><span class="sxs-lookup"><span data-stu-id="ec0b0-104">Properties</span></span>

| <span data-ttu-id="ec0b0-105">属性</span><span class="sxs-lookup"><span data-stu-id="ec0b0-105">Property</span></span>           | <span data-ttu-id="ec0b0-106">类型</span><span class="sxs-lookup"><span data-stu-id="ec0b0-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="ec0b0-107">im</span><span class="sxs-lookup"><span data-stu-id="ec0b0-107">im</span></span>                 | <span data-ttu-id="ec0b0-108">Int64</span><span class="sxs-lookup"><span data-stu-id="ec0b0-108">Int64</span></span>  |
| <span data-ttu-id="ec0b0-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="ec0b0-109">audioVideo</span></span>         | <span data-ttu-id="ec0b0-110">Int64</span><span class="sxs-lookup"><span data-stu-id="ec0b0-110">Int64</span></span>  |
| <span data-ttu-id="ec0b0-111">的</span><span class="sxs-lookup"><span data-stu-id="ec0b0-111">appSharing</span></span>         | <span data-ttu-id="ec0b0-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ec0b0-112">Int64</span></span>  |
| <span data-ttu-id="ec0b0-113">web</span><span class="sxs-lookup"><span data-stu-id="ec0b0-113">web</span></span>                | <span data-ttu-id="ec0b0-114">Int64</span><span class="sxs-lookup"><span data-stu-id="ec0b0-114">Int64</span></span>  |
| <span data-ttu-id="ec0b0-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="ec0b0-115">dialInOut3rdParty</span></span>  | <span data-ttu-id="ec0b0-116">Int64</span><span class="sxs-lookup"><span data-stu-id="ec0b0-116">Int64</span></span>  |
| <span data-ttu-id="ec0b0-117">dialInOutMicrosoft</span><span class="sxs-lookup"><span data-stu-id="ec0b0-117">dialInOutMicrosoft</span></span> | <span data-ttu-id="ec0b0-118">Int64</span><span class="sxs-lookup"><span data-stu-id="ec0b0-118">Int64</span></span>  |
| <span data-ttu-id="ec0b0-119">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ec0b0-119">reportRefreshDate</span></span>  | <span data-ttu-id="ec0b0-120">日期</span><span class="sxs-lookup"><span data-stu-id="ec0b0-120">Date</span></span>   |
| <span data-ttu-id="ec0b0-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="ec0b0-121">reportDate</span></span>         | <span data-ttu-id="ec0b0-122">日期</span><span class="sxs-lookup"><span data-stu-id="ec0b0-122">Date</span></span>   |
| <span data-ttu-id="ec0b0-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ec0b0-123">reportPeriod</span></span>       | <span data-ttu-id="ec0b0-124">String</span><span class="sxs-lookup"><span data-stu-id="ec0b0-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ec0b0-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ec0b0-125">JSON representation</span></span>

<span data-ttu-id="ec0b0-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec0b0-126">The following is a JSON representation of the resource.</span></span>

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
