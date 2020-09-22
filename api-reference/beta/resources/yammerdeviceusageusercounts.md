---
title: yammerDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 137c69b4bc908e7706716fadcc6e6f9c619604ab
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979187"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a><span data-ttu-id="e1360-103">yammerDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1360-103">yammerDeviceUsageUserCounts resource type</span></span>

<span data-ttu-id="e1360-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1360-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="e1360-105">属性</span><span class="sxs-lookup"><span data-stu-id="e1360-105">Properties</span></span>

| <span data-ttu-id="e1360-106">属性</span><span class="sxs-lookup"><span data-stu-id="e1360-106">Property</span></span>          | <span data-ttu-id="e1360-107">类型</span><span class="sxs-lookup"><span data-stu-id="e1360-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="e1360-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e1360-108">reportRefreshDate</span></span> | <span data-ttu-id="e1360-109">日期</span><span class="sxs-lookup"><span data-stu-id="e1360-109">Date</span></span>   |
| <span data-ttu-id="e1360-110">web</span><span class="sxs-lookup"><span data-stu-id="e1360-110">web</span></span>               | <span data-ttu-id="e1360-111">Int32</span><span class="sxs-lookup"><span data-stu-id="e1360-111">Int32</span></span>  |
| <span data-ttu-id="e1360-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="e1360-112">windowsPhone</span></span>      | <span data-ttu-id="e1360-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e1360-113">Int32</span></span>  |
| <span data-ttu-id="e1360-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="e1360-114">androidPhone</span></span>      | <span data-ttu-id="e1360-115">Int32</span><span class="sxs-lookup"><span data-stu-id="e1360-115">Int32</span></span>  |
| <span data-ttu-id="e1360-116">iPhone</span><span class="sxs-lookup"><span data-stu-id="e1360-116">iPhone</span></span>            | <span data-ttu-id="e1360-117">Int32</span><span class="sxs-lookup"><span data-stu-id="e1360-117">Int32</span></span>  |
| <span data-ttu-id="e1360-118">iPad</span><span class="sxs-lookup"><span data-stu-id="e1360-118">iPad</span></span>              | <span data-ttu-id="e1360-119">Int32</span><span class="sxs-lookup"><span data-stu-id="e1360-119">Int32</span></span>  |
| <span data-ttu-id="e1360-120">相互</span><span class="sxs-lookup"><span data-stu-id="e1360-120">other</span></span>             | <span data-ttu-id="e1360-121">Int32</span><span class="sxs-lookup"><span data-stu-id="e1360-121">Int32</span></span>  |
| <span data-ttu-id="e1360-122">reportDate</span><span class="sxs-lookup"><span data-stu-id="e1360-122">reportDate</span></span>        | <span data-ttu-id="e1360-123">日期</span><span class="sxs-lookup"><span data-stu-id="e1360-123">Date</span></span>   |
| <span data-ttu-id="e1360-124">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e1360-124">reportPeriod</span></span>      | <span data-ttu-id="e1360-125">String</span><span class="sxs-lookup"><span data-stu-id="e1360-125">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e1360-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1360-126">JSON representation</span></span>

<span data-ttu-id="e1360-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1360-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "other": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


