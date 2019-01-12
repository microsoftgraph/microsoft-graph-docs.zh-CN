---
title: yammerDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 937691487046e2e77cc26b2c1f1a154966e1681b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936345"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="5c4d8-103">yammerDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c4d8-103">yammerDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5c4d8-104">属性</span><span class="sxs-lookup"><span data-stu-id="5c4d8-104">Properties</span></span>

| <span data-ttu-id="5c4d8-105">属性</span><span class="sxs-lookup"><span data-stu-id="5c4d8-105">Property</span></span>          | <span data-ttu-id="5c4d8-106">类型</span><span class="sxs-lookup"><span data-stu-id="5c4d8-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5c4d8-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5c4d8-107">reportRefreshDate</span></span> | <span data-ttu-id="5c4d8-108">日期</span><span class="sxs-lookup"><span data-stu-id="5c4d8-108">Date</span></span>   |
| <span data-ttu-id="5c4d8-109">web</span><span class="sxs-lookup"><span data-stu-id="5c4d8-109">web</span></span>               | <span data-ttu-id="5c4d8-110">Int32</span><span class="sxs-lookup"><span data-stu-id="5c4d8-110">Int32</span></span>  |
| <span data-ttu-id="5c4d8-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="5c4d8-111">windowsPhone</span></span>      | <span data-ttu-id="5c4d8-112">Int32</span><span class="sxs-lookup"><span data-stu-id="5c4d8-112">Int32</span></span>  |
| <span data-ttu-id="5c4d8-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="5c4d8-113">androidPhone</span></span>      | <span data-ttu-id="5c4d8-114">Int32</span><span class="sxs-lookup"><span data-stu-id="5c4d8-114">Int32</span></span>  |
| <span data-ttu-id="5c4d8-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="5c4d8-115">iPhone</span></span>            | <span data-ttu-id="5c4d8-116">Int32</span><span class="sxs-lookup"><span data-stu-id="5c4d8-116">Int32</span></span>  |
| <span data-ttu-id="5c4d8-117">iPad</span><span class="sxs-lookup"><span data-stu-id="5c4d8-117">iPad</span></span>              | <span data-ttu-id="5c4d8-118">Int32</span><span class="sxs-lookup"><span data-stu-id="5c4d8-118">Int32</span></span>  |
| <span data-ttu-id="5c4d8-119">其他</span><span class="sxs-lookup"><span data-stu-id="5c4d8-119">other</span></span>             | <span data-ttu-id="5c4d8-120">Int32</span><span class="sxs-lookup"><span data-stu-id="5c4d8-120">Int32</span></span>  |
| <span data-ttu-id="5c4d8-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5c4d8-121">reportPeriod</span></span>      | <span data-ttu-id="5c4d8-122">String</span><span class="sxs-lookup"><span data-stu-id="5c4d8-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5c4d8-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c4d8-123">JSON representation</span></span>

<span data-ttu-id="5c4d8-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c4d8-124">The following is a JSON representation of the resource.</span></span>

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
