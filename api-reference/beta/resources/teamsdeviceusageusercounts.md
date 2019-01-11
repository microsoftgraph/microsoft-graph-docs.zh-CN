---
title: teamsDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 07a43b024d133e5ac1d8eb8a2665fd3027001edb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857349"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="e3c8e-103">teamsDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="e3c8e-103">teamsDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e3c8e-104">属性</span><span class="sxs-lookup"><span data-stu-id="e3c8e-104">Properties</span></span>

| <span data-ttu-id="e3c8e-105">属性</span><span class="sxs-lookup"><span data-stu-id="e3c8e-105">Property</span></span>          | <span data-ttu-id="e3c8e-106">类型</span><span class="sxs-lookup"><span data-stu-id="e3c8e-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="e3c8e-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e3c8e-107">reportRefreshDate</span></span> | <span data-ttu-id="e3c8e-108">日期</span><span class="sxs-lookup"><span data-stu-id="e3c8e-108">Date</span></span>   |
| <span data-ttu-id="e3c8e-109">web</span><span class="sxs-lookup"><span data-stu-id="e3c8e-109">web</span></span>               | <span data-ttu-id="e3c8e-110">Int64</span><span class="sxs-lookup"><span data-stu-id="e3c8e-110">Int64</span></span>  |
| <span data-ttu-id="e3c8e-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="e3c8e-111">windowsPhone</span></span>      | <span data-ttu-id="e3c8e-112">Int64</span><span class="sxs-lookup"><span data-stu-id="e3c8e-112">Int64</span></span>  |
| <span data-ttu-id="e3c8e-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="e3c8e-113">androidPhone</span></span>      | <span data-ttu-id="e3c8e-114">Int64</span><span class="sxs-lookup"><span data-stu-id="e3c8e-114">Int64</span></span>  |
| <span data-ttu-id="e3c8e-115">ios</span><span class="sxs-lookup"><span data-stu-id="e3c8e-115">ios</span></span>               | <span data-ttu-id="e3c8e-116">Int64</span><span class="sxs-lookup"><span data-stu-id="e3c8e-116">Int64</span></span>  |
| <span data-ttu-id="e3c8e-117">mac</span><span class="sxs-lookup"><span data-stu-id="e3c8e-117">mac</span></span>               | <span data-ttu-id="e3c8e-118">Int64</span><span class="sxs-lookup"><span data-stu-id="e3c8e-118">Int64</span></span>  |
| <span data-ttu-id="e3c8e-119">windows</span><span class="sxs-lookup"><span data-stu-id="e3c8e-119">windows</span></span>           | <span data-ttu-id="e3c8e-120">Int64</span><span class="sxs-lookup"><span data-stu-id="e3c8e-120">Int64</span></span>  |
| <span data-ttu-id="e3c8e-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="e3c8e-121">reportDate</span></span>        | <span data-ttu-id="e3c8e-122">日期</span><span class="sxs-lookup"><span data-stu-id="e3c8e-122">Date</span></span>   |
| <span data-ttu-id="e3c8e-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e3c8e-123">reportPeriod</span></span>      | <span data-ttu-id="e3c8e-124">String</span><span class="sxs-lookup"><span data-stu-id="e3c8e-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e3c8e-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3c8e-125">JSON representation</span></span>

<span data-ttu-id="e3c8e-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3c8e-126">The following is a JSON representation of the resource.</span></span>

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
