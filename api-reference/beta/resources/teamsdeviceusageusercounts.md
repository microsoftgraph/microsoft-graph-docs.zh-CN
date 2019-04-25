---
title: teamsDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 671dfada02b9c16d3392d0a97023b82020fd1218
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553594"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="f1b5e-103">teamsDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1b5e-103">teamsDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f1b5e-104">属性</span><span class="sxs-lookup"><span data-stu-id="f1b5e-104">Properties</span></span>

| <span data-ttu-id="f1b5e-105">属性</span><span class="sxs-lookup"><span data-stu-id="f1b5e-105">Property</span></span>          | <span data-ttu-id="f1b5e-106">类型</span><span class="sxs-lookup"><span data-stu-id="f1b5e-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f1b5e-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f1b5e-107">reportRefreshDate</span></span> | <span data-ttu-id="f1b5e-108">Date</span><span class="sxs-lookup"><span data-stu-id="f1b5e-108">Date</span></span>   |
| <span data-ttu-id="f1b5e-109">web</span><span class="sxs-lookup"><span data-stu-id="f1b5e-109">web</span></span>               | <span data-ttu-id="f1b5e-110">Int64</span><span class="sxs-lookup"><span data-stu-id="f1b5e-110">Int64</span></span>  |
| <span data-ttu-id="f1b5e-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="f1b5e-111">windowsPhone</span></span>      | <span data-ttu-id="f1b5e-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f1b5e-112">Int64</span></span>  |
| <span data-ttu-id="f1b5e-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="f1b5e-113">androidPhone</span></span>      | <span data-ttu-id="f1b5e-114">Int64</span><span class="sxs-lookup"><span data-stu-id="f1b5e-114">Int64</span></span>  |
| <span data-ttu-id="f1b5e-115">ios</span><span class="sxs-lookup"><span data-stu-id="f1b5e-115">ios</span></span>               | <span data-ttu-id="f1b5e-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f1b5e-116">Int64</span></span>  |
| <span data-ttu-id="f1b5e-117">mac</span><span class="sxs-lookup"><span data-stu-id="f1b5e-117">mac</span></span>               | <span data-ttu-id="f1b5e-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f1b5e-118">Int64</span></span>  |
| <span data-ttu-id="f1b5e-119">时间</span><span class="sxs-lookup"><span data-stu-id="f1b5e-119">windows</span></span>           | <span data-ttu-id="f1b5e-120">Int64</span><span class="sxs-lookup"><span data-stu-id="f1b5e-120">Int64</span></span>  |
| <span data-ttu-id="f1b5e-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="f1b5e-121">reportDate</span></span>        | <span data-ttu-id="f1b5e-122">Date</span><span class="sxs-lookup"><span data-stu-id="f1b5e-122">Date</span></span>   |
| <span data-ttu-id="f1b5e-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f1b5e-123">reportPeriod</span></span>      | <span data-ttu-id="f1b5e-124">String</span><span class="sxs-lookup"><span data-stu-id="f1b5e-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f1b5e-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1b5e-125">JSON representation</span></span>

<span data-ttu-id="f1b5e-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1b5e-126">The following is a JSON representation of the resource.</span></span>

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
