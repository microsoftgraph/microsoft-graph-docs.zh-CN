---
title: yammerDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: ad8707d33c4200ea6729205819871d890929f001
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889031"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="c819f-103">yammerDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="c819f-103">yammerDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c819f-104">属性</span><span class="sxs-lookup"><span data-stu-id="c819f-104">Properties</span></span>

| <span data-ttu-id="c819f-105">属性</span><span class="sxs-lookup"><span data-stu-id="c819f-105">Property</span></span>          | <span data-ttu-id="c819f-106">类型</span><span class="sxs-lookup"><span data-stu-id="c819f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="c819f-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c819f-107">reportRefreshDate</span></span> | <span data-ttu-id="c819f-108">日期</span><span class="sxs-lookup"><span data-stu-id="c819f-108">Date</span></span>   |
| <span data-ttu-id="c819f-109">web</span><span class="sxs-lookup"><span data-stu-id="c819f-109">web</span></span>               | <span data-ttu-id="c819f-110">Int32</span><span class="sxs-lookup"><span data-stu-id="c819f-110">Int32</span></span>  |
| <span data-ttu-id="c819f-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="c819f-111">windowsPhone</span></span>      | <span data-ttu-id="c819f-112">Int32</span><span class="sxs-lookup"><span data-stu-id="c819f-112">Int32</span></span>  |
| <span data-ttu-id="c819f-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="c819f-113">androidPhone</span></span>      | <span data-ttu-id="c819f-114">Int32</span><span class="sxs-lookup"><span data-stu-id="c819f-114">Int32</span></span>  |
| <span data-ttu-id="c819f-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="c819f-115">iPhone</span></span>            | <span data-ttu-id="c819f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c819f-116">Int32</span></span>  |
| <span data-ttu-id="c819f-117">iPad</span><span class="sxs-lookup"><span data-stu-id="c819f-117">iPad</span></span>              | <span data-ttu-id="c819f-118">Int32</span><span class="sxs-lookup"><span data-stu-id="c819f-118">Int32</span></span>  |
| <span data-ttu-id="c819f-119">其他</span><span class="sxs-lookup"><span data-stu-id="c819f-119">other</span></span>             | <span data-ttu-id="c819f-120">Int32</span><span class="sxs-lookup"><span data-stu-id="c819f-120">Int32</span></span>  |
| <span data-ttu-id="c819f-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c819f-121">reportPeriod</span></span>      | <span data-ttu-id="c819f-122">String</span><span class="sxs-lookup"><span data-stu-id="c819f-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c819f-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c819f-123">JSON representation</span></span>

<span data-ttu-id="c819f-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c819f-124">The following is a JSON representation of the resource.</span></span>

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
