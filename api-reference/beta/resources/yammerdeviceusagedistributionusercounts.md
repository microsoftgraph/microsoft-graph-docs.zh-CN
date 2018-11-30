---
title: yammerDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: f98c8831c147a82985d1e59b5559d88e1a4824c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044967"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="6f12a-103">yammerDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="6f12a-103">yammerDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6f12a-104">属性</span><span class="sxs-lookup"><span data-stu-id="6f12a-104">Properties</span></span>

| <span data-ttu-id="6f12a-105">属性</span><span class="sxs-lookup"><span data-stu-id="6f12a-105">Property</span></span>          | <span data-ttu-id="6f12a-106">类型</span><span class="sxs-lookup"><span data-stu-id="6f12a-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="6f12a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6f12a-107">reportRefreshDate</span></span> | <span data-ttu-id="6f12a-108">日期</span><span class="sxs-lookup"><span data-stu-id="6f12a-108">Date</span></span>   |
| <span data-ttu-id="6f12a-109">web</span><span class="sxs-lookup"><span data-stu-id="6f12a-109">web</span></span>               | <span data-ttu-id="6f12a-110">Int32</span><span class="sxs-lookup"><span data-stu-id="6f12a-110">Int32</span></span>  |
| <span data-ttu-id="6f12a-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="6f12a-111">windowsPhone</span></span>      | <span data-ttu-id="6f12a-112">Int32</span><span class="sxs-lookup"><span data-stu-id="6f12a-112">Int32</span></span>  |
| <span data-ttu-id="6f12a-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="6f12a-113">androidPhone</span></span>      | <span data-ttu-id="6f12a-114">Int32</span><span class="sxs-lookup"><span data-stu-id="6f12a-114">Int32</span></span>  |
| <span data-ttu-id="6f12a-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="6f12a-115">iPhone</span></span>            | <span data-ttu-id="6f12a-116">Int32</span><span class="sxs-lookup"><span data-stu-id="6f12a-116">Int32</span></span>  |
| <span data-ttu-id="6f12a-117">iPad</span><span class="sxs-lookup"><span data-stu-id="6f12a-117">iPad</span></span>              | <span data-ttu-id="6f12a-118">Int32</span><span class="sxs-lookup"><span data-stu-id="6f12a-118">Int32</span></span>  |
| <span data-ttu-id="6f12a-119">其他</span><span class="sxs-lookup"><span data-stu-id="6f12a-119">other</span></span>             | <span data-ttu-id="6f12a-120">Int32</span><span class="sxs-lookup"><span data-stu-id="6f12a-120">Int32</span></span>  |
| <span data-ttu-id="6f12a-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6f12a-121">reportPeriod</span></span>      | <span data-ttu-id="6f12a-122">String</span><span class="sxs-lookup"><span data-stu-id="6f12a-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6f12a-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f12a-123">JSON representation</span></span>

<span data-ttu-id="6f12a-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f12a-124">The following is a JSON representation of the resource.</span></span>

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
