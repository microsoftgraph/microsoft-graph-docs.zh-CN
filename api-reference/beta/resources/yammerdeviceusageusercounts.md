---
title: yammerDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 9780d75ee75d45675c21ad639fccdf4edd32a949
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982360"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a><span data-ttu-id="f8634-103">yammerDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="f8634-103">yammerDeviceUsageUserCounts resource type</span></span>

<span data-ttu-id="f8634-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8634-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="f8634-105">属性</span><span class="sxs-lookup"><span data-stu-id="f8634-105">Properties</span></span>

| <span data-ttu-id="f8634-106">属性</span><span class="sxs-lookup"><span data-stu-id="f8634-106">Property</span></span>          | <span data-ttu-id="f8634-107">类型</span><span class="sxs-lookup"><span data-stu-id="f8634-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f8634-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f8634-108">reportRefreshDate</span></span> | <span data-ttu-id="f8634-109">日期</span><span class="sxs-lookup"><span data-stu-id="f8634-109">Date</span></span>   |
| <span data-ttu-id="f8634-110">web</span><span class="sxs-lookup"><span data-stu-id="f8634-110">web</span></span>               | <span data-ttu-id="f8634-111">Int32</span><span class="sxs-lookup"><span data-stu-id="f8634-111">Int32</span></span>  |
| <span data-ttu-id="f8634-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="f8634-112">windowsPhone</span></span>      | <span data-ttu-id="f8634-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f8634-113">Int32</span></span>  |
| <span data-ttu-id="f8634-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="f8634-114">androidPhone</span></span>      | <span data-ttu-id="f8634-115">Int32</span><span class="sxs-lookup"><span data-stu-id="f8634-115">Int32</span></span>  |
| <span data-ttu-id="f8634-116">iPhone</span><span class="sxs-lookup"><span data-stu-id="f8634-116">iPhone</span></span>            | <span data-ttu-id="f8634-117">Int32</span><span class="sxs-lookup"><span data-stu-id="f8634-117">Int32</span></span>  |
| <span data-ttu-id="f8634-118">iPad</span><span class="sxs-lookup"><span data-stu-id="f8634-118">iPad</span></span>              | <span data-ttu-id="f8634-119">Int32</span><span class="sxs-lookup"><span data-stu-id="f8634-119">Int32</span></span>  |
| <span data-ttu-id="f8634-120">other</span><span class="sxs-lookup"><span data-stu-id="f8634-120">other</span></span>             | <span data-ttu-id="f8634-121">Int32</span><span class="sxs-lookup"><span data-stu-id="f8634-121">Int32</span></span>  |
| <span data-ttu-id="f8634-122">reportDate</span><span class="sxs-lookup"><span data-stu-id="f8634-122">reportDate</span></span>        | <span data-ttu-id="f8634-123">日期</span><span class="sxs-lookup"><span data-stu-id="f8634-123">Date</span></span>   |
| <span data-ttu-id="f8634-124">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f8634-124">reportPeriod</span></span>      | <span data-ttu-id="f8634-125">String</span><span class="sxs-lookup"><span data-stu-id="f8634-125">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f8634-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8634-126">JSON representation</span></span>

<span data-ttu-id="f8634-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8634-127">The following is a JSON representation of the resource.</span></span>

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


