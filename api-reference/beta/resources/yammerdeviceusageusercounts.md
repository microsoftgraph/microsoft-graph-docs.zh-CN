---
title: yammerDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 63bd3e150e822d3c356f4409c2920e4998e53ec2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551517"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a><span data-ttu-id="04543-103">yammerDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="04543-103">yammerDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="04543-104">属性</span><span class="sxs-lookup"><span data-stu-id="04543-104">Properties</span></span>

| <span data-ttu-id="04543-105">属性</span><span class="sxs-lookup"><span data-stu-id="04543-105">Property</span></span>          | <span data-ttu-id="04543-106">类型</span><span class="sxs-lookup"><span data-stu-id="04543-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="04543-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="04543-107">reportRefreshDate</span></span> | <span data-ttu-id="04543-108">Date</span><span class="sxs-lookup"><span data-stu-id="04543-108">Date</span></span>   |
| <span data-ttu-id="04543-109">web</span><span class="sxs-lookup"><span data-stu-id="04543-109">web</span></span>               | <span data-ttu-id="04543-110">Int32</span><span class="sxs-lookup"><span data-stu-id="04543-110">Int32</span></span>  |
| <span data-ttu-id="04543-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="04543-111">windowsPhone</span></span>      | <span data-ttu-id="04543-112">Int32</span><span class="sxs-lookup"><span data-stu-id="04543-112">Int32</span></span>  |
| <span data-ttu-id="04543-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="04543-113">androidPhone</span></span>      | <span data-ttu-id="04543-114">Int32</span><span class="sxs-lookup"><span data-stu-id="04543-114">Int32</span></span>  |
| <span data-ttu-id="04543-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="04543-115">iPhone</span></span>            | <span data-ttu-id="04543-116">Int32</span><span class="sxs-lookup"><span data-stu-id="04543-116">Int32</span></span>  |
| <span data-ttu-id="04543-117">iPad</span><span class="sxs-lookup"><span data-stu-id="04543-117">iPad</span></span>              | <span data-ttu-id="04543-118">Int32</span><span class="sxs-lookup"><span data-stu-id="04543-118">Int32</span></span>  |
| <span data-ttu-id="04543-119">相互</span><span class="sxs-lookup"><span data-stu-id="04543-119">other</span></span>             | <span data-ttu-id="04543-120">Int32</span><span class="sxs-lookup"><span data-stu-id="04543-120">Int32</span></span>  |
| <span data-ttu-id="04543-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="04543-121">reportDate</span></span>        | <span data-ttu-id="04543-122">Date</span><span class="sxs-lookup"><span data-stu-id="04543-122">Date</span></span>   |
| <span data-ttu-id="04543-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="04543-123">reportPeriod</span></span>      | <span data-ttu-id="04543-124">String</span><span class="sxs-lookup"><span data-stu-id="04543-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="04543-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04543-125">JSON representation</span></span>

<span data-ttu-id="04543-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04543-126">The following is a JSON representation of the resource.</span></span>

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
