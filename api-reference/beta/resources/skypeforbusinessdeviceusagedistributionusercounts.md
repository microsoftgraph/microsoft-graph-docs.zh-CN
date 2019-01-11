---
title: skypeForBusinessDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 3658bec2d99c5098b970e35240221dbf954beba6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884431"
---
# <a name="skypeforbusinessdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="562ad-103">skypeForBusinessDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="562ad-103">skypeForBusinessDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="562ad-104">属性</span><span class="sxs-lookup"><span data-stu-id="562ad-104">Properties</span></span>

| <span data-ttu-id="562ad-105">属性</span><span class="sxs-lookup"><span data-stu-id="562ad-105">Property</span></span>          | <span data-ttu-id="562ad-106">类型</span><span class="sxs-lookup"><span data-stu-id="562ad-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="562ad-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="562ad-107">reportRefreshDate</span></span> | <span data-ttu-id="562ad-108">日期</span><span class="sxs-lookup"><span data-stu-id="562ad-108">Date</span></span>   |
| <span data-ttu-id="562ad-109">windows</span><span class="sxs-lookup"><span data-stu-id="562ad-109">windows</span></span>           | <span data-ttu-id="562ad-110">Int64</span><span class="sxs-lookup"><span data-stu-id="562ad-110">Int64</span></span>  |
| <span data-ttu-id="562ad-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="562ad-111">windowsPhone</span></span>      | <span data-ttu-id="562ad-112">Int64</span><span class="sxs-lookup"><span data-stu-id="562ad-112">Int64</span></span>  |
| <span data-ttu-id="562ad-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="562ad-113">androidPhone</span></span>      | <span data-ttu-id="562ad-114">Int64</span><span class="sxs-lookup"><span data-stu-id="562ad-114">Int64</span></span>  |
| <span data-ttu-id="562ad-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="562ad-115">iPhone</span></span>            | <span data-ttu-id="562ad-116">Int64</span><span class="sxs-lookup"><span data-stu-id="562ad-116">Int64</span></span>  |
| <span data-ttu-id="562ad-117">iPad</span><span class="sxs-lookup"><span data-stu-id="562ad-117">iPad</span></span>              | <span data-ttu-id="562ad-118">Int64</span><span class="sxs-lookup"><span data-stu-id="562ad-118">Int64</span></span>  |
| <span data-ttu-id="562ad-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="562ad-119">reportPeriod</span></span>      | <span data-ttu-id="562ad-120">String</span><span class="sxs-lookup"><span data-stu-id="562ad-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="562ad-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="562ad-121">JSON representation</span></span>

<span data-ttu-id="562ad-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="562ad-122">The following is a JSON representation of the resource.</span></span>

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
