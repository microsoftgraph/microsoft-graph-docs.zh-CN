---
title: yammerDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: d3fbfaeac312096393c3c5a2d406327551cbaa33
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867947"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a><span data-ttu-id="daa90-103">yammerDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="daa90-103">yammerDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="daa90-104">属性</span><span class="sxs-lookup"><span data-stu-id="daa90-104">Properties</span></span>

| <span data-ttu-id="daa90-105">属性</span><span class="sxs-lookup"><span data-stu-id="daa90-105">Property</span></span>          | <span data-ttu-id="daa90-106">类型</span><span class="sxs-lookup"><span data-stu-id="daa90-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="daa90-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="daa90-107">reportRefreshDate</span></span> | <span data-ttu-id="daa90-108">日期</span><span class="sxs-lookup"><span data-stu-id="daa90-108">Date</span></span>   |
| <span data-ttu-id="daa90-109">web</span><span class="sxs-lookup"><span data-stu-id="daa90-109">web</span></span>               | <span data-ttu-id="daa90-110">Int32</span><span class="sxs-lookup"><span data-stu-id="daa90-110">Int32</span></span>  |
| <span data-ttu-id="daa90-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="daa90-111">windowsPhone</span></span>      | <span data-ttu-id="daa90-112">Int32</span><span class="sxs-lookup"><span data-stu-id="daa90-112">Int32</span></span>  |
| <span data-ttu-id="daa90-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="daa90-113">androidPhone</span></span>      | <span data-ttu-id="daa90-114">Int32</span><span class="sxs-lookup"><span data-stu-id="daa90-114">Int32</span></span>  |
| <span data-ttu-id="daa90-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="daa90-115">iPhone</span></span>            | <span data-ttu-id="daa90-116">Int32</span><span class="sxs-lookup"><span data-stu-id="daa90-116">Int32</span></span>  |
| <span data-ttu-id="daa90-117">iPad</span><span class="sxs-lookup"><span data-stu-id="daa90-117">iPad</span></span>              | <span data-ttu-id="daa90-118">Int32</span><span class="sxs-lookup"><span data-stu-id="daa90-118">Int32</span></span>  |
| <span data-ttu-id="daa90-119">其他</span><span class="sxs-lookup"><span data-stu-id="daa90-119">other</span></span>             | <span data-ttu-id="daa90-120">Int32</span><span class="sxs-lookup"><span data-stu-id="daa90-120">Int32</span></span>  |
| <span data-ttu-id="daa90-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="daa90-121">reportDate</span></span>        | <span data-ttu-id="daa90-122">日期</span><span class="sxs-lookup"><span data-stu-id="daa90-122">Date</span></span>   |
| <span data-ttu-id="daa90-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="daa90-123">reportPeriod</span></span>      | <span data-ttu-id="daa90-124">String</span><span class="sxs-lookup"><span data-stu-id="daa90-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="daa90-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="daa90-125">JSON representation</span></span>

<span data-ttu-id="daa90-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="daa90-126">The following is a JSON representation of the resource.</span></span>

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
