---
title: skypeForBusinessDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 56468f8df7704de66dde5e649100ca5c33b4b00c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997541"
---
# <a name="skypeforbusinessdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="bde3a-103">skypeForBusinessDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="bde3a-103">skypeForBusinessDeviceUsageDistributionUserCounts resource type</span></span>

<span data-ttu-id="bde3a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bde3a-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="bde3a-105">属性</span><span class="sxs-lookup"><span data-stu-id="bde3a-105">Properties</span></span>

| <span data-ttu-id="bde3a-106">属性</span><span class="sxs-lookup"><span data-stu-id="bde3a-106">Property</span></span>          | <span data-ttu-id="bde3a-107">类型</span><span class="sxs-lookup"><span data-stu-id="bde3a-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="bde3a-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="bde3a-108">reportRefreshDate</span></span> | <span data-ttu-id="bde3a-109">日期</span><span class="sxs-lookup"><span data-stu-id="bde3a-109">Date</span></span>   |
| <span data-ttu-id="bde3a-110">时间</span><span class="sxs-lookup"><span data-stu-id="bde3a-110">windows</span></span>           | <span data-ttu-id="bde3a-111">Int64</span><span class="sxs-lookup"><span data-stu-id="bde3a-111">Int64</span></span>  |
| <span data-ttu-id="bde3a-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="bde3a-112">windowsPhone</span></span>      | <span data-ttu-id="bde3a-113">Int64</span><span class="sxs-lookup"><span data-stu-id="bde3a-113">Int64</span></span>  |
| <span data-ttu-id="bde3a-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="bde3a-114">androidPhone</span></span>      | <span data-ttu-id="bde3a-115">Int64</span><span class="sxs-lookup"><span data-stu-id="bde3a-115">Int64</span></span>  |
| <span data-ttu-id="bde3a-116">iPhone</span><span class="sxs-lookup"><span data-stu-id="bde3a-116">iPhone</span></span>            | <span data-ttu-id="bde3a-117">Int64</span><span class="sxs-lookup"><span data-stu-id="bde3a-117">Int64</span></span>  |
| <span data-ttu-id="bde3a-118">iPad</span><span class="sxs-lookup"><span data-stu-id="bde3a-118">iPad</span></span>              | <span data-ttu-id="bde3a-119">Int64</span><span class="sxs-lookup"><span data-stu-id="bde3a-119">Int64</span></span>  |
| <span data-ttu-id="bde3a-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="bde3a-120">reportPeriod</span></span>      | <span data-ttu-id="bde3a-121">String</span><span class="sxs-lookup"><span data-stu-id="bde3a-121">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bde3a-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bde3a-122">JSON representation</span></span>

<span data-ttu-id="bde3a-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bde3a-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date",
  "windows": 1024,
  "windowsPhone": 1024,
  "androidPhone": 1024,
  "iPhone": 1024,
  "iPad": 1024,
  "reportPeriod": "String"
}
```


