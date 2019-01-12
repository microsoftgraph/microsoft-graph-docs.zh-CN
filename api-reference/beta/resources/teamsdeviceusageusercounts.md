---
title: teamsDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 671dfada02b9c16d3392d0a97023b82020fd1218
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987396"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="5be38-103">teamsDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="5be38-103">teamsDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5be38-104">属性</span><span class="sxs-lookup"><span data-stu-id="5be38-104">Properties</span></span>

| <span data-ttu-id="5be38-105">属性</span><span class="sxs-lookup"><span data-stu-id="5be38-105">Property</span></span>          | <span data-ttu-id="5be38-106">类型</span><span class="sxs-lookup"><span data-stu-id="5be38-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5be38-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5be38-107">reportRefreshDate</span></span> | <span data-ttu-id="5be38-108">日期</span><span class="sxs-lookup"><span data-stu-id="5be38-108">Date</span></span>   |
| <span data-ttu-id="5be38-109">web</span><span class="sxs-lookup"><span data-stu-id="5be38-109">web</span></span>               | <span data-ttu-id="5be38-110">Int64</span><span class="sxs-lookup"><span data-stu-id="5be38-110">Int64</span></span>  |
| <span data-ttu-id="5be38-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="5be38-111">windowsPhone</span></span>      | <span data-ttu-id="5be38-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5be38-112">Int64</span></span>  |
| <span data-ttu-id="5be38-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="5be38-113">androidPhone</span></span>      | <span data-ttu-id="5be38-114">Int64</span><span class="sxs-lookup"><span data-stu-id="5be38-114">Int64</span></span>  |
| <span data-ttu-id="5be38-115">ios</span><span class="sxs-lookup"><span data-stu-id="5be38-115">ios</span></span>               | <span data-ttu-id="5be38-116">Int64</span><span class="sxs-lookup"><span data-stu-id="5be38-116">Int64</span></span>  |
| <span data-ttu-id="5be38-117">mac</span><span class="sxs-lookup"><span data-stu-id="5be38-117">mac</span></span>               | <span data-ttu-id="5be38-118">Int64</span><span class="sxs-lookup"><span data-stu-id="5be38-118">Int64</span></span>  |
| <span data-ttu-id="5be38-119">windows</span><span class="sxs-lookup"><span data-stu-id="5be38-119">windows</span></span>           | <span data-ttu-id="5be38-120">Int64</span><span class="sxs-lookup"><span data-stu-id="5be38-120">Int64</span></span>  |
| <span data-ttu-id="5be38-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="5be38-121">reportDate</span></span>        | <span data-ttu-id="5be38-122">日期</span><span class="sxs-lookup"><span data-stu-id="5be38-122">Date</span></span>   |
| <span data-ttu-id="5be38-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5be38-123">reportPeriod</span></span>      | <span data-ttu-id="5be38-124">String</span><span class="sxs-lookup"><span data-stu-id="5be38-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5be38-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5be38-125">JSON representation</span></span>

<span data-ttu-id="5be38-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5be38-126">The following is a JSON representation of the resource.</span></span>

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
