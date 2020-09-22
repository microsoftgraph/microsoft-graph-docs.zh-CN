---
title: teamsDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6b5a4a09c96c5b3691c4cbcc285ac947c903ce50
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046480"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="94f83-103">teamsDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="94f83-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

<span data-ttu-id="94f83-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94f83-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="94f83-105">属性</span><span class="sxs-lookup"><span data-stu-id="94f83-105">Properties</span></span>

| <span data-ttu-id="94f83-106">属性</span><span class="sxs-lookup"><span data-stu-id="94f83-106">Property</span></span>          | <span data-ttu-id="94f83-107">类型</span><span class="sxs-lookup"><span data-stu-id="94f83-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="94f83-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="94f83-108">reportRefreshDate</span></span> | <span data-ttu-id="94f83-109">日期</span><span class="sxs-lookup"><span data-stu-id="94f83-109">Date</span></span>   |
| <span data-ttu-id="94f83-110">web</span><span class="sxs-lookup"><span data-stu-id="94f83-110">web</span></span>               | <span data-ttu-id="94f83-111">Int64</span><span class="sxs-lookup"><span data-stu-id="94f83-111">Int64</span></span>  |
| <span data-ttu-id="94f83-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="94f83-112">windowsPhone</span></span>      | <span data-ttu-id="94f83-113">Int64</span><span class="sxs-lookup"><span data-stu-id="94f83-113">Int64</span></span>  |
| <span data-ttu-id="94f83-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="94f83-114">androidPhone</span></span>      | <span data-ttu-id="94f83-115">Int64</span><span class="sxs-lookup"><span data-stu-id="94f83-115">Int64</span></span>  |
| <span data-ttu-id="94f83-116">ios</span><span class="sxs-lookup"><span data-stu-id="94f83-116">ios</span></span>               | <span data-ttu-id="94f83-117">Int64</span><span class="sxs-lookup"><span data-stu-id="94f83-117">Int64</span></span>  |
| <span data-ttu-id="94f83-118">mac</span><span class="sxs-lookup"><span data-stu-id="94f83-118">mac</span></span>               | <span data-ttu-id="94f83-119">Int64</span><span class="sxs-lookup"><span data-stu-id="94f83-119">Int64</span></span>  |
| <span data-ttu-id="94f83-120">时间</span><span class="sxs-lookup"><span data-stu-id="94f83-120">windows</span></span>           | <span data-ttu-id="94f83-121">Int64</span><span class="sxs-lookup"><span data-stu-id="94f83-121">Int64</span></span>  |
| <span data-ttu-id="94f83-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="94f83-122">reportPeriod</span></span>      | <span data-ttu-id="94f83-123">String</span><span class="sxs-lookup"><span data-stu-id="94f83-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="94f83-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94f83-124">JSON representation</span></span>

<span data-ttu-id="94f83-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94f83-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
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
  "reportPeriod": "String"
}
```


