---
title: skypeForBusinessDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: d98590e83637e45d35f135c56f2c0b8ff7d282bb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583499"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a><span data-ttu-id="e4385-103">skypeForBusinessDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4385-103">skypeForBusinessDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e4385-104">属性</span><span class="sxs-lookup"><span data-stu-id="e4385-104">Properties</span></span>

| <span data-ttu-id="e4385-105">属性</span><span class="sxs-lookup"><span data-stu-id="e4385-105">Property</span></span>          | <span data-ttu-id="e4385-106">类型</span><span class="sxs-lookup"><span data-stu-id="e4385-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="e4385-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e4385-107">reportRefreshDate</span></span> | <span data-ttu-id="e4385-108">Date</span><span class="sxs-lookup"><span data-stu-id="e4385-108">Date</span></span>   |
| <span data-ttu-id="e4385-109">时间</span><span class="sxs-lookup"><span data-stu-id="e4385-109">windows</span></span>           | <span data-ttu-id="e4385-110">Int64</span><span class="sxs-lookup"><span data-stu-id="e4385-110">Int64</span></span>  |
| <span data-ttu-id="e4385-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="e4385-111">windowsPhone</span></span>      | <span data-ttu-id="e4385-112">Int64</span><span class="sxs-lookup"><span data-stu-id="e4385-112">Int64</span></span>  |
| <span data-ttu-id="e4385-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="e4385-113">androidPhone</span></span>      | <span data-ttu-id="e4385-114">Int64</span><span class="sxs-lookup"><span data-stu-id="e4385-114">Int64</span></span>  |
| <span data-ttu-id="e4385-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="e4385-115">iPhone</span></span>            | <span data-ttu-id="e4385-116">Int64</span><span class="sxs-lookup"><span data-stu-id="e4385-116">Int64</span></span>  |
| <span data-ttu-id="e4385-117">iPad</span><span class="sxs-lookup"><span data-stu-id="e4385-117">iPad</span></span>              | <span data-ttu-id="e4385-118">Int64</span><span class="sxs-lookup"><span data-stu-id="e4385-118">Int64</span></span>  |
| <span data-ttu-id="e4385-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="e4385-119">reportDate</span></span>        | <span data-ttu-id="e4385-120">Date</span><span class="sxs-lookup"><span data-stu-id="e4385-120">Date</span></span>   |
| <span data-ttu-id="e4385-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e4385-121">reportPeriod</span></span>      | <span data-ttu-id="e4385-122">String</span><span class="sxs-lookup"><span data-stu-id="e4385-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e4385-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4385-123">JSON representation</span></span>

<span data-ttu-id="e4385-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4385-124">The following is a JSON representation of the resource.</span></span>

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
