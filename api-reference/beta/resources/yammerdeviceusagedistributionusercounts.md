---
title: yammerDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1797facecb5047badb35c0a4d876680e817cc643
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555078"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="37b0d-103">yammerDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="37b0d-103">yammerDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="37b0d-104">属性</span><span class="sxs-lookup"><span data-stu-id="37b0d-104">Properties</span></span>

| <span data-ttu-id="37b0d-105">属性</span><span class="sxs-lookup"><span data-stu-id="37b0d-105">Property</span></span>          | <span data-ttu-id="37b0d-106">类型</span><span class="sxs-lookup"><span data-stu-id="37b0d-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="37b0d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="37b0d-107">reportRefreshDate</span></span> | <span data-ttu-id="37b0d-108">Date</span><span class="sxs-lookup"><span data-stu-id="37b0d-108">Date</span></span>   |
| <span data-ttu-id="37b0d-109">web</span><span class="sxs-lookup"><span data-stu-id="37b0d-109">web</span></span>               | <span data-ttu-id="37b0d-110">Int32</span><span class="sxs-lookup"><span data-stu-id="37b0d-110">Int32</span></span>  |
| <span data-ttu-id="37b0d-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="37b0d-111">windowsPhone</span></span>      | <span data-ttu-id="37b0d-112">Int32</span><span class="sxs-lookup"><span data-stu-id="37b0d-112">Int32</span></span>  |
| <span data-ttu-id="37b0d-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="37b0d-113">androidPhone</span></span>      | <span data-ttu-id="37b0d-114">Int32</span><span class="sxs-lookup"><span data-stu-id="37b0d-114">Int32</span></span>  |
| <span data-ttu-id="37b0d-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="37b0d-115">iPhone</span></span>            | <span data-ttu-id="37b0d-116">Int32</span><span class="sxs-lookup"><span data-stu-id="37b0d-116">Int32</span></span>  |
| <span data-ttu-id="37b0d-117">iPad</span><span class="sxs-lookup"><span data-stu-id="37b0d-117">iPad</span></span>              | <span data-ttu-id="37b0d-118">Int32</span><span class="sxs-lookup"><span data-stu-id="37b0d-118">Int32</span></span>  |
| <span data-ttu-id="37b0d-119">相互</span><span class="sxs-lookup"><span data-stu-id="37b0d-119">other</span></span>             | <span data-ttu-id="37b0d-120">Int32</span><span class="sxs-lookup"><span data-stu-id="37b0d-120">Int32</span></span>  |
| <span data-ttu-id="37b0d-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="37b0d-121">reportPeriod</span></span>      | <span data-ttu-id="37b0d-122">String</span><span class="sxs-lookup"><span data-stu-id="37b0d-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="37b0d-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37b0d-123">JSON representation</span></span>

<span data-ttu-id="37b0d-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37b0d-124">The following is a JSON representation of the resource.</span></span>

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
