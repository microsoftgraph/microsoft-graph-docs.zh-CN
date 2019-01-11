---
title: skypeForBusinessDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: d98590e83637e45d35f135c56f2c0b8ff7d282bb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866925"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a><span data-ttu-id="4e6d1-103">skypeForBusinessDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e6d1-103">skypeForBusinessDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4e6d1-104">属性</span><span class="sxs-lookup"><span data-stu-id="4e6d1-104">Properties</span></span>

| <span data-ttu-id="4e6d1-105">属性</span><span class="sxs-lookup"><span data-stu-id="4e6d1-105">Property</span></span>          | <span data-ttu-id="4e6d1-106">类型</span><span class="sxs-lookup"><span data-stu-id="4e6d1-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="4e6d1-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4e6d1-107">reportRefreshDate</span></span> | <span data-ttu-id="4e6d1-108">日期</span><span class="sxs-lookup"><span data-stu-id="4e6d1-108">Date</span></span>   |
| <span data-ttu-id="4e6d1-109">windows</span><span class="sxs-lookup"><span data-stu-id="4e6d1-109">windows</span></span>           | <span data-ttu-id="4e6d1-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4e6d1-110">Int64</span></span>  |
| <span data-ttu-id="4e6d1-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="4e6d1-111">windowsPhone</span></span>      | <span data-ttu-id="4e6d1-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4e6d1-112">Int64</span></span>  |
| <span data-ttu-id="4e6d1-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="4e6d1-113">androidPhone</span></span>      | <span data-ttu-id="4e6d1-114">Int64</span><span class="sxs-lookup"><span data-stu-id="4e6d1-114">Int64</span></span>  |
| <span data-ttu-id="4e6d1-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="4e6d1-115">iPhone</span></span>            | <span data-ttu-id="4e6d1-116">Int64</span><span class="sxs-lookup"><span data-stu-id="4e6d1-116">Int64</span></span>  |
| <span data-ttu-id="4e6d1-117">iPad</span><span class="sxs-lookup"><span data-stu-id="4e6d1-117">iPad</span></span>              | <span data-ttu-id="4e6d1-118">Int64</span><span class="sxs-lookup"><span data-stu-id="4e6d1-118">Int64</span></span>  |
| <span data-ttu-id="4e6d1-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="4e6d1-119">reportDate</span></span>        | <span data-ttu-id="4e6d1-120">日期</span><span class="sxs-lookup"><span data-stu-id="4e6d1-120">Date</span></span>   |
| <span data-ttu-id="4e6d1-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4e6d1-121">reportPeriod</span></span>      | <span data-ttu-id="4e6d1-122">String</span><span class="sxs-lookup"><span data-stu-id="4e6d1-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4e6d1-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e6d1-123">JSON representation</span></span>

<span data-ttu-id="4e6d1-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e6d1-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "windows": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
