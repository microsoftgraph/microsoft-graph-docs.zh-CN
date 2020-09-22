---
title: yammerDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 8dc388356a029b0a0587affbcb84b305a5f6b767
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046066"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="fee18-103">yammerDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="fee18-103">yammerDeviceUsageDistributionUserCounts resource type</span></span>

<span data-ttu-id="fee18-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fee18-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="fee18-105">属性</span><span class="sxs-lookup"><span data-stu-id="fee18-105">Properties</span></span>

| <span data-ttu-id="fee18-106">属性</span><span class="sxs-lookup"><span data-stu-id="fee18-106">Property</span></span>          | <span data-ttu-id="fee18-107">类型</span><span class="sxs-lookup"><span data-stu-id="fee18-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="fee18-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fee18-108">reportRefreshDate</span></span> | <span data-ttu-id="fee18-109">日期</span><span class="sxs-lookup"><span data-stu-id="fee18-109">Date</span></span>   |
| <span data-ttu-id="fee18-110">web</span><span class="sxs-lookup"><span data-stu-id="fee18-110">web</span></span>               | <span data-ttu-id="fee18-111">Int32</span><span class="sxs-lookup"><span data-stu-id="fee18-111">Int32</span></span>  |
| <span data-ttu-id="fee18-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="fee18-112">windowsPhone</span></span>      | <span data-ttu-id="fee18-113">Int32</span><span class="sxs-lookup"><span data-stu-id="fee18-113">Int32</span></span>  |
| <span data-ttu-id="fee18-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="fee18-114">androidPhone</span></span>      | <span data-ttu-id="fee18-115">Int32</span><span class="sxs-lookup"><span data-stu-id="fee18-115">Int32</span></span>  |
| <span data-ttu-id="fee18-116">iPhone</span><span class="sxs-lookup"><span data-stu-id="fee18-116">iPhone</span></span>            | <span data-ttu-id="fee18-117">Int32</span><span class="sxs-lookup"><span data-stu-id="fee18-117">Int32</span></span>  |
| <span data-ttu-id="fee18-118">iPad</span><span class="sxs-lookup"><span data-stu-id="fee18-118">iPad</span></span>              | <span data-ttu-id="fee18-119">Int32</span><span class="sxs-lookup"><span data-stu-id="fee18-119">Int32</span></span>  |
| <span data-ttu-id="fee18-120">相互</span><span class="sxs-lookup"><span data-stu-id="fee18-120">other</span></span>             | <span data-ttu-id="fee18-121">Int32</span><span class="sxs-lookup"><span data-stu-id="fee18-121">Int32</span></span>  |
| <span data-ttu-id="fee18-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fee18-122">reportPeriod</span></span>      | <span data-ttu-id="fee18-123">String</span><span class="sxs-lookup"><span data-stu-id="fee18-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fee18-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fee18-124">JSON representation</span></span>

<span data-ttu-id="fee18-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fee18-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageDistributionUserCounts"
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
  "reportPeriod": "String"
}
```


