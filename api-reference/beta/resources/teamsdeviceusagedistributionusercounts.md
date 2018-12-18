---
title: teamsDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
ms.openlocfilehash: 01b9f67f30a7b2f13aac65cbcd4795792ee0aaa0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345848"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="4aea5-103">teamsDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="4aea5-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4aea5-104">属性</span><span class="sxs-lookup"><span data-stu-id="4aea5-104">Properties</span></span>

| <span data-ttu-id="4aea5-105">属性</span><span class="sxs-lookup"><span data-stu-id="4aea5-105">Property</span></span>          | <span data-ttu-id="4aea5-106">类型</span><span class="sxs-lookup"><span data-stu-id="4aea5-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="4aea5-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4aea5-107">reportRefreshDate</span></span> | <span data-ttu-id="4aea5-108">日期</span><span class="sxs-lookup"><span data-stu-id="4aea5-108">Date</span></span>   |
| <span data-ttu-id="4aea5-109">web</span><span class="sxs-lookup"><span data-stu-id="4aea5-109">web</span></span>               | <span data-ttu-id="4aea5-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4aea5-110">Int64</span></span>  |
| <span data-ttu-id="4aea5-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="4aea5-111">windowsPhone</span></span>      | <span data-ttu-id="4aea5-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4aea5-112">Int64</span></span>  |
| <span data-ttu-id="4aea5-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="4aea5-113">androidPhone</span></span>      | <span data-ttu-id="4aea5-114">Int64</span><span class="sxs-lookup"><span data-stu-id="4aea5-114">Int64</span></span>  |
| <span data-ttu-id="4aea5-115">ios</span><span class="sxs-lookup"><span data-stu-id="4aea5-115">ios</span></span>               | <span data-ttu-id="4aea5-116">Int64</span><span class="sxs-lookup"><span data-stu-id="4aea5-116">Int64</span></span>  |
| <span data-ttu-id="4aea5-117">mac</span><span class="sxs-lookup"><span data-stu-id="4aea5-117">mac</span></span>               | <span data-ttu-id="4aea5-118">Int64</span><span class="sxs-lookup"><span data-stu-id="4aea5-118">Int64</span></span>  |
| <span data-ttu-id="4aea5-119">windows</span><span class="sxs-lookup"><span data-stu-id="4aea5-119">windows</span></span>           | <span data-ttu-id="4aea5-120">Int64</span><span class="sxs-lookup"><span data-stu-id="4aea5-120">Int64</span></span>  |
| <span data-ttu-id="4aea5-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4aea5-121">reportPeriod</span></span>      | <span data-ttu-id="4aea5-122">String</span><span class="sxs-lookup"><span data-stu-id="4aea5-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4aea5-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4aea5-123">JSON representation</span></span>

<span data-ttu-id="4aea5-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4aea5-124">The following is a JSON representation of the resource.</span></span>

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
