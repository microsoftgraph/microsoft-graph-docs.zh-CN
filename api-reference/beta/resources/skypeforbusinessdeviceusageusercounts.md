---
title: skypeForBusinessDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 04f14ce10a93d8bff870613e644b80f554d26573
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008206"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a><span data-ttu-id="6ef35-103">skypeForBusinessDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ef35-103">skypeForBusinessDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6ef35-104">属性</span><span class="sxs-lookup"><span data-stu-id="6ef35-104">Properties</span></span>

| <span data-ttu-id="6ef35-105">属性</span><span class="sxs-lookup"><span data-stu-id="6ef35-105">Property</span></span>          | <span data-ttu-id="6ef35-106">类型</span><span class="sxs-lookup"><span data-stu-id="6ef35-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="6ef35-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6ef35-107">reportRefreshDate</span></span> | <span data-ttu-id="6ef35-108">日期</span><span class="sxs-lookup"><span data-stu-id="6ef35-108">Date</span></span>   |
| <span data-ttu-id="6ef35-109">时间</span><span class="sxs-lookup"><span data-stu-id="6ef35-109">windows</span></span>           | <span data-ttu-id="6ef35-110">Int64</span><span class="sxs-lookup"><span data-stu-id="6ef35-110">Int64</span></span>  |
| <span data-ttu-id="6ef35-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="6ef35-111">windowsPhone</span></span>      | <span data-ttu-id="6ef35-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6ef35-112">Int64</span></span>  |
| <span data-ttu-id="6ef35-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="6ef35-113">androidPhone</span></span>      | <span data-ttu-id="6ef35-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6ef35-114">Int64</span></span>  |
| <span data-ttu-id="6ef35-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="6ef35-115">iPhone</span></span>            | <span data-ttu-id="6ef35-116">Int64</span><span class="sxs-lookup"><span data-stu-id="6ef35-116">Int64</span></span>  |
| <span data-ttu-id="6ef35-117">iPad</span><span class="sxs-lookup"><span data-stu-id="6ef35-117">iPad</span></span>              | <span data-ttu-id="6ef35-118">Int64</span><span class="sxs-lookup"><span data-stu-id="6ef35-118">Int64</span></span>  |
| <span data-ttu-id="6ef35-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="6ef35-119">reportDate</span></span>        | <span data-ttu-id="6ef35-120">日期</span><span class="sxs-lookup"><span data-stu-id="6ef35-120">Date</span></span>   |
| <span data-ttu-id="6ef35-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6ef35-121">reportPeriod</span></span>      | <span data-ttu-id="6ef35-122">String</span><span class="sxs-lookup"><span data-stu-id="6ef35-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6ef35-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ef35-123">JSON representation</span></span>

<span data-ttu-id="6ef35-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ef35-124">The following is a JSON representation of the resource.</span></span>

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
