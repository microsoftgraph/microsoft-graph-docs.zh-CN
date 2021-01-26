---
title: yammerDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: a64748ff506c3f72e4144ee2090229424f9334d4
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982374"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="f4103-103">yammerDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4103-103">yammerDeviceUsageDistributionUserCounts resource type</span></span>

<span data-ttu-id="f4103-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4103-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="f4103-105">属性</span><span class="sxs-lookup"><span data-stu-id="f4103-105">Properties</span></span>

| <span data-ttu-id="f4103-106">属性</span><span class="sxs-lookup"><span data-stu-id="f4103-106">Property</span></span>          | <span data-ttu-id="f4103-107">类型</span><span class="sxs-lookup"><span data-stu-id="f4103-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f4103-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f4103-108">reportRefreshDate</span></span> | <span data-ttu-id="f4103-109">日期</span><span class="sxs-lookup"><span data-stu-id="f4103-109">Date</span></span>   |
| <span data-ttu-id="f4103-110">web</span><span class="sxs-lookup"><span data-stu-id="f4103-110">web</span></span>               | <span data-ttu-id="f4103-111">Int32</span><span class="sxs-lookup"><span data-stu-id="f4103-111">Int32</span></span>  |
| <span data-ttu-id="f4103-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="f4103-112">windowsPhone</span></span>      | <span data-ttu-id="f4103-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f4103-113">Int32</span></span>  |
| <span data-ttu-id="f4103-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="f4103-114">androidPhone</span></span>      | <span data-ttu-id="f4103-115">Int32</span><span class="sxs-lookup"><span data-stu-id="f4103-115">Int32</span></span>  |
| <span data-ttu-id="f4103-116">iPhone</span><span class="sxs-lookup"><span data-stu-id="f4103-116">iPhone</span></span>            | <span data-ttu-id="f4103-117">Int32</span><span class="sxs-lookup"><span data-stu-id="f4103-117">Int32</span></span>  |
| <span data-ttu-id="f4103-118">iPad</span><span class="sxs-lookup"><span data-stu-id="f4103-118">iPad</span></span>              | <span data-ttu-id="f4103-119">Int32</span><span class="sxs-lookup"><span data-stu-id="f4103-119">Int32</span></span>  |
| <span data-ttu-id="f4103-120">other</span><span class="sxs-lookup"><span data-stu-id="f4103-120">other</span></span>             | <span data-ttu-id="f4103-121">Int32</span><span class="sxs-lookup"><span data-stu-id="f4103-121">Int32</span></span>  |
| <span data-ttu-id="f4103-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f4103-122">reportPeriod</span></span>      | <span data-ttu-id="f4103-123">String</span><span class="sxs-lookup"><span data-stu-id="f4103-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f4103-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4103-124">JSON representation</span></span>

<span data-ttu-id="f4103-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4103-125">The following is a JSON representation of the resource.</span></span>

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


