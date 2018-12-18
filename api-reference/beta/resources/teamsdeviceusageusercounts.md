---
title: teamsDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
ms.openlocfilehash: 1255a8e1e92bb461d5c100c72e9030f57db5f8fa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306508"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="aef45-103">teamsDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="aef45-103">teamsDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="aef45-104">属性</span><span class="sxs-lookup"><span data-stu-id="aef45-104">Properties</span></span>

| <span data-ttu-id="aef45-105">属性</span><span class="sxs-lookup"><span data-stu-id="aef45-105">Property</span></span>          | <span data-ttu-id="aef45-106">类型</span><span class="sxs-lookup"><span data-stu-id="aef45-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="aef45-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="aef45-107">reportRefreshDate</span></span> | <span data-ttu-id="aef45-108">日期</span><span class="sxs-lookup"><span data-stu-id="aef45-108">Date</span></span>   |
| <span data-ttu-id="aef45-109">web</span><span class="sxs-lookup"><span data-stu-id="aef45-109">web</span></span>               | <span data-ttu-id="aef45-110">Int64</span><span class="sxs-lookup"><span data-stu-id="aef45-110">Int64</span></span>  |
| <span data-ttu-id="aef45-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="aef45-111">windowsPhone</span></span>      | <span data-ttu-id="aef45-112">Int64</span><span class="sxs-lookup"><span data-stu-id="aef45-112">Int64</span></span>  |
| <span data-ttu-id="aef45-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="aef45-113">androidPhone</span></span>      | <span data-ttu-id="aef45-114">Int64</span><span class="sxs-lookup"><span data-stu-id="aef45-114">Int64</span></span>  |
| <span data-ttu-id="aef45-115">ios</span><span class="sxs-lookup"><span data-stu-id="aef45-115">ios</span></span>               | <span data-ttu-id="aef45-116">Int64</span><span class="sxs-lookup"><span data-stu-id="aef45-116">Int64</span></span>  |
| <span data-ttu-id="aef45-117">mac</span><span class="sxs-lookup"><span data-stu-id="aef45-117">mac</span></span>               | <span data-ttu-id="aef45-118">Int64</span><span class="sxs-lookup"><span data-stu-id="aef45-118">Int64</span></span>  |
| <span data-ttu-id="aef45-119">windows</span><span class="sxs-lookup"><span data-stu-id="aef45-119">windows</span></span>           | <span data-ttu-id="aef45-120">Int64</span><span class="sxs-lookup"><span data-stu-id="aef45-120">Int64</span></span>  |
| <span data-ttu-id="aef45-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="aef45-121">reportDate</span></span>        | <span data-ttu-id="aef45-122">日期</span><span class="sxs-lookup"><span data-stu-id="aef45-122">Date</span></span>   |
| <span data-ttu-id="aef45-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="aef45-123">reportPeriod</span></span>      | <span data-ttu-id="aef45-124">String</span><span class="sxs-lookup"><span data-stu-id="aef45-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aef45-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aef45-125">JSON representation</span></span>

<span data-ttu-id="aef45-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aef45-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
