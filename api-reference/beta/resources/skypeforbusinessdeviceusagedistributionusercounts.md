---
title: skypeForBusinessDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 3658bec2d99c5098b970e35240221dbf954beba6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581259"
---
# <a name="skypeforbusinessdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="5a651-103">skypeForBusinessDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="5a651-103">skypeForBusinessDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5a651-104">属性</span><span class="sxs-lookup"><span data-stu-id="5a651-104">Properties</span></span>

| <span data-ttu-id="5a651-105">属性</span><span class="sxs-lookup"><span data-stu-id="5a651-105">Property</span></span>          | <span data-ttu-id="5a651-106">类型</span><span class="sxs-lookup"><span data-stu-id="5a651-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5a651-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5a651-107">reportRefreshDate</span></span> | <span data-ttu-id="5a651-108">Date</span><span class="sxs-lookup"><span data-stu-id="5a651-108">Date</span></span>   |
| <span data-ttu-id="5a651-109">时间</span><span class="sxs-lookup"><span data-stu-id="5a651-109">windows</span></span>           | <span data-ttu-id="5a651-110">Int64</span><span class="sxs-lookup"><span data-stu-id="5a651-110">Int64</span></span>  |
| <span data-ttu-id="5a651-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="5a651-111">windowsPhone</span></span>      | <span data-ttu-id="5a651-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5a651-112">Int64</span></span>  |
| <span data-ttu-id="5a651-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="5a651-113">androidPhone</span></span>      | <span data-ttu-id="5a651-114">Int64</span><span class="sxs-lookup"><span data-stu-id="5a651-114">Int64</span></span>  |
| <span data-ttu-id="5a651-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="5a651-115">iPhone</span></span>            | <span data-ttu-id="5a651-116">Int64</span><span class="sxs-lookup"><span data-stu-id="5a651-116">Int64</span></span>  |
| <span data-ttu-id="5a651-117">iPad</span><span class="sxs-lookup"><span data-stu-id="5a651-117">iPad</span></span>              | <span data-ttu-id="5a651-118">Int64</span><span class="sxs-lookup"><span data-stu-id="5a651-118">Int64</span></span>  |
| <span data-ttu-id="5a651-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5a651-119">reportPeriod</span></span>      | <span data-ttu-id="5a651-120">String</span><span class="sxs-lookup"><span data-stu-id="5a651-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5a651-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a651-121">JSON representation</span></span>

<span data-ttu-id="5a651-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a651-122">The following is a JSON representation of the resource.</span></span>

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
