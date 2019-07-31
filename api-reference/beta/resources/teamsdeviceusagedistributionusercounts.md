---
title: teamsDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1842d2edc9e527d577b6a44e61443018f8309c17
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007611"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="136b5-103">teamsDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="136b5-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="136b5-104">属性</span><span class="sxs-lookup"><span data-stu-id="136b5-104">Properties</span></span>

| <span data-ttu-id="136b5-105">属性</span><span class="sxs-lookup"><span data-stu-id="136b5-105">Property</span></span>          | <span data-ttu-id="136b5-106">类型</span><span class="sxs-lookup"><span data-stu-id="136b5-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="136b5-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="136b5-107">reportRefreshDate</span></span> | <span data-ttu-id="136b5-108">日期</span><span class="sxs-lookup"><span data-stu-id="136b5-108">Date</span></span>   |
| <span data-ttu-id="136b5-109">web</span><span class="sxs-lookup"><span data-stu-id="136b5-109">web</span></span>               | <span data-ttu-id="136b5-110">Int64</span><span class="sxs-lookup"><span data-stu-id="136b5-110">Int64</span></span>  |
| <span data-ttu-id="136b5-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="136b5-111">windowsPhone</span></span>      | <span data-ttu-id="136b5-112">Int64</span><span class="sxs-lookup"><span data-stu-id="136b5-112">Int64</span></span>  |
| <span data-ttu-id="136b5-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="136b5-113">androidPhone</span></span>      | <span data-ttu-id="136b5-114">Int64</span><span class="sxs-lookup"><span data-stu-id="136b5-114">Int64</span></span>  |
| <span data-ttu-id="136b5-115">ios</span><span class="sxs-lookup"><span data-stu-id="136b5-115">ios</span></span>               | <span data-ttu-id="136b5-116">Int64</span><span class="sxs-lookup"><span data-stu-id="136b5-116">Int64</span></span>  |
| <span data-ttu-id="136b5-117">mac</span><span class="sxs-lookup"><span data-stu-id="136b5-117">mac</span></span>               | <span data-ttu-id="136b5-118">Int64</span><span class="sxs-lookup"><span data-stu-id="136b5-118">Int64</span></span>  |
| <span data-ttu-id="136b5-119">时间</span><span class="sxs-lookup"><span data-stu-id="136b5-119">windows</span></span>           | <span data-ttu-id="136b5-120">Int64</span><span class="sxs-lookup"><span data-stu-id="136b5-120">Int64</span></span>  |
| <span data-ttu-id="136b5-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="136b5-121">reportPeriod</span></span>      | <span data-ttu-id="136b5-122">String</span><span class="sxs-lookup"><span data-stu-id="136b5-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="136b5-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="136b5-123">JSON representation</span></span>

<span data-ttu-id="136b5-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="136b5-124">The following is a JSON representation of the resource.</span></span>

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
