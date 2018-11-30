---
title: teamsDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: b039320e389e1a61832089991b2368b27e51c475
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041734"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="7a438-103">teamsDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a438-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7a438-104">属性</span><span class="sxs-lookup"><span data-stu-id="7a438-104">Properties</span></span>

| <span data-ttu-id="7a438-105">属性</span><span class="sxs-lookup"><span data-stu-id="7a438-105">Property</span></span>          | <span data-ttu-id="7a438-106">类型</span><span class="sxs-lookup"><span data-stu-id="7a438-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="7a438-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7a438-107">reportRefreshDate</span></span> | <span data-ttu-id="7a438-108">日期</span><span class="sxs-lookup"><span data-stu-id="7a438-108">Date</span></span>   |
| <span data-ttu-id="7a438-109">web</span><span class="sxs-lookup"><span data-stu-id="7a438-109">web</span></span>               | <span data-ttu-id="7a438-110">Int64</span><span class="sxs-lookup"><span data-stu-id="7a438-110">Int64</span></span>  |
| <span data-ttu-id="7a438-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="7a438-111">windowsPhone</span></span>      | <span data-ttu-id="7a438-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7a438-112">Int64</span></span>  |
| <span data-ttu-id="7a438-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="7a438-113">androidPhone</span></span>      | <span data-ttu-id="7a438-114">Int64</span><span class="sxs-lookup"><span data-stu-id="7a438-114">Int64</span></span>  |
| <span data-ttu-id="7a438-115">ios</span><span class="sxs-lookup"><span data-stu-id="7a438-115">ios</span></span>               | <span data-ttu-id="7a438-116">Int64</span><span class="sxs-lookup"><span data-stu-id="7a438-116">Int64</span></span>  |
| <span data-ttu-id="7a438-117">mac</span><span class="sxs-lookup"><span data-stu-id="7a438-117">mac</span></span>               | <span data-ttu-id="7a438-118">Int64</span><span class="sxs-lookup"><span data-stu-id="7a438-118">Int64</span></span>  |
| <span data-ttu-id="7a438-119">windows</span><span class="sxs-lookup"><span data-stu-id="7a438-119">windows</span></span>           | <span data-ttu-id="7a438-120">Int64</span><span class="sxs-lookup"><span data-stu-id="7a438-120">Int64</span></span>  |
| <span data-ttu-id="7a438-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7a438-121">reportPeriod</span></span>      | <span data-ttu-id="7a438-122">String</span><span class="sxs-lookup"><span data-stu-id="7a438-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7a438-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a438-123">JSON representation</span></span>

<span data-ttu-id="7a438-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a438-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "reportPeriod": "String"
}
```
