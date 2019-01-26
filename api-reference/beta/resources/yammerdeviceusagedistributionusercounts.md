---
title: yammerDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1797facecb5047badb35c0a4d876680e817cc643
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576799"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="fef87-103">yammerDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="fef87-103">yammerDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="fef87-104">属性</span><span class="sxs-lookup"><span data-stu-id="fef87-104">Properties</span></span>

| <span data-ttu-id="fef87-105">属性</span><span class="sxs-lookup"><span data-stu-id="fef87-105">Property</span></span>          | <span data-ttu-id="fef87-106">类型</span><span class="sxs-lookup"><span data-stu-id="fef87-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="fef87-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fef87-107">reportRefreshDate</span></span> | <span data-ttu-id="fef87-108">Date</span><span class="sxs-lookup"><span data-stu-id="fef87-108">Date</span></span>   |
| <span data-ttu-id="fef87-109">web</span><span class="sxs-lookup"><span data-stu-id="fef87-109">web</span></span>               | <span data-ttu-id="fef87-110">Int32</span><span class="sxs-lookup"><span data-stu-id="fef87-110">Int32</span></span>  |
| <span data-ttu-id="fef87-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="fef87-111">windowsPhone</span></span>      | <span data-ttu-id="fef87-112">Int32</span><span class="sxs-lookup"><span data-stu-id="fef87-112">Int32</span></span>  |
| <span data-ttu-id="fef87-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="fef87-113">androidPhone</span></span>      | <span data-ttu-id="fef87-114">Int32</span><span class="sxs-lookup"><span data-stu-id="fef87-114">Int32</span></span>  |
| <span data-ttu-id="fef87-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="fef87-115">iPhone</span></span>            | <span data-ttu-id="fef87-116">Int32</span><span class="sxs-lookup"><span data-stu-id="fef87-116">Int32</span></span>  |
| <span data-ttu-id="fef87-117">iPad</span><span class="sxs-lookup"><span data-stu-id="fef87-117">iPad</span></span>              | <span data-ttu-id="fef87-118">Int32</span><span class="sxs-lookup"><span data-stu-id="fef87-118">Int32</span></span>  |
| <span data-ttu-id="fef87-119">其他</span><span class="sxs-lookup"><span data-stu-id="fef87-119">other</span></span>             | <span data-ttu-id="fef87-120">Int32</span><span class="sxs-lookup"><span data-stu-id="fef87-120">Int32</span></span>  |
| <span data-ttu-id="fef87-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fef87-121">reportPeriod</span></span>      | <span data-ttu-id="fef87-122">String</span><span class="sxs-lookup"><span data-stu-id="fef87-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fef87-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fef87-123">JSON representation</span></span>

<span data-ttu-id="fef87-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fef87-124">The following is a JSON representation of the resource.</span></span>

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
