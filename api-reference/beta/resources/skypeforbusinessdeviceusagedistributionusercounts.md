---
title: skypeForBusinessDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b5c90db3ec241017781d52bbb623d728a7959445
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964940"
---
# <a name="skypeforbusinessdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="b3c0f-103">skypeForBusinessDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3c0f-103">skypeForBusinessDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b3c0f-104">属性</span><span class="sxs-lookup"><span data-stu-id="b3c0f-104">Properties</span></span>

| <span data-ttu-id="b3c0f-105">属性</span><span class="sxs-lookup"><span data-stu-id="b3c0f-105">Property</span></span>          | <span data-ttu-id="b3c0f-106">类型</span><span class="sxs-lookup"><span data-stu-id="b3c0f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="b3c0f-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b3c0f-107">reportRefreshDate</span></span> | <span data-ttu-id="b3c0f-108">日期</span><span class="sxs-lookup"><span data-stu-id="b3c0f-108">Date</span></span>   |
| <span data-ttu-id="b3c0f-109">时间</span><span class="sxs-lookup"><span data-stu-id="b3c0f-109">windows</span></span>           | <span data-ttu-id="b3c0f-110">Int64</span><span class="sxs-lookup"><span data-stu-id="b3c0f-110">Int64</span></span>  |
| <span data-ttu-id="b3c0f-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="b3c0f-111">windowsPhone</span></span>      | <span data-ttu-id="b3c0f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b3c0f-112">Int64</span></span>  |
| <span data-ttu-id="b3c0f-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="b3c0f-113">androidPhone</span></span>      | <span data-ttu-id="b3c0f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="b3c0f-114">Int64</span></span>  |
| <span data-ttu-id="b3c0f-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="b3c0f-115">iPhone</span></span>            | <span data-ttu-id="b3c0f-116">Int64</span><span class="sxs-lookup"><span data-stu-id="b3c0f-116">Int64</span></span>  |
| <span data-ttu-id="b3c0f-117">iPad</span><span class="sxs-lookup"><span data-stu-id="b3c0f-117">iPad</span></span>              | <span data-ttu-id="b3c0f-118">Int64</span><span class="sxs-lookup"><span data-stu-id="b3c0f-118">Int64</span></span>  |
| <span data-ttu-id="b3c0f-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b3c0f-119">reportPeriod</span></span>      | <span data-ttu-id="b3c0f-120">String</span><span class="sxs-lookup"><span data-stu-id="b3c0f-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b3c0f-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3c0f-121">JSON representation</span></span>

<span data-ttu-id="b3c0f-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3c0f-122">The following is a JSON representation of the resource.</span></span>

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
