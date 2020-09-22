---
title: teamsDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: af62b0bf6d11c256252b2c6c6f16f4e3b5ba2354
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046466"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="de43a-103">teamsDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="de43a-103">teamsDeviceUsageUserCounts resource type</span></span>

<span data-ttu-id="de43a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de43a-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="de43a-105">属性</span><span class="sxs-lookup"><span data-stu-id="de43a-105">Properties</span></span>

| <span data-ttu-id="de43a-106">属性</span><span class="sxs-lookup"><span data-stu-id="de43a-106">Property</span></span>          | <span data-ttu-id="de43a-107">类型</span><span class="sxs-lookup"><span data-stu-id="de43a-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="de43a-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="de43a-108">reportRefreshDate</span></span> | <span data-ttu-id="de43a-109">日期</span><span class="sxs-lookup"><span data-stu-id="de43a-109">Date</span></span>   |
| <span data-ttu-id="de43a-110">web</span><span class="sxs-lookup"><span data-stu-id="de43a-110">web</span></span>               | <span data-ttu-id="de43a-111">Int64</span><span class="sxs-lookup"><span data-stu-id="de43a-111">Int64</span></span>  |
| <span data-ttu-id="de43a-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="de43a-112">windowsPhone</span></span>      | <span data-ttu-id="de43a-113">Int64</span><span class="sxs-lookup"><span data-stu-id="de43a-113">Int64</span></span>  |
| <span data-ttu-id="de43a-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="de43a-114">androidPhone</span></span>      | <span data-ttu-id="de43a-115">Int64</span><span class="sxs-lookup"><span data-stu-id="de43a-115">Int64</span></span>  |
| <span data-ttu-id="de43a-116">ios</span><span class="sxs-lookup"><span data-stu-id="de43a-116">ios</span></span>               | <span data-ttu-id="de43a-117">Int64</span><span class="sxs-lookup"><span data-stu-id="de43a-117">Int64</span></span>  |
| <span data-ttu-id="de43a-118">mac</span><span class="sxs-lookup"><span data-stu-id="de43a-118">mac</span></span>               | <span data-ttu-id="de43a-119">Int64</span><span class="sxs-lookup"><span data-stu-id="de43a-119">Int64</span></span>  |
| <span data-ttu-id="de43a-120">时间</span><span class="sxs-lookup"><span data-stu-id="de43a-120">windows</span></span>           | <span data-ttu-id="de43a-121">Int64</span><span class="sxs-lookup"><span data-stu-id="de43a-121">Int64</span></span>  |
| <span data-ttu-id="de43a-122">reportDate</span><span class="sxs-lookup"><span data-stu-id="de43a-122">reportDate</span></span>        | <span data-ttu-id="de43a-123">日期</span><span class="sxs-lookup"><span data-stu-id="de43a-123">Date</span></span>   |
| <span data-ttu-id="de43a-124">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="de43a-124">reportPeriod</span></span>      | <span data-ttu-id="de43a-125">String</span><span class="sxs-lookup"><span data-stu-id="de43a-125">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="de43a-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de43a-126">JSON representation</span></span>

<span data-ttu-id="de43a-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de43a-127">The following is a JSON representation of the resource.</span></span>

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


