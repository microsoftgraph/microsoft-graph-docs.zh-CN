---
title: teamsDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c6b10af0e4b32c37a5fe365dc8deedae63efc8c4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519874"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="84a7a-103">teamsDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="84a7a-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

<span data-ttu-id="84a7a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="84a7a-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="84a7a-105">属性</span><span class="sxs-lookup"><span data-stu-id="84a7a-105">Properties</span></span>

| <span data-ttu-id="84a7a-106">属性</span><span class="sxs-lookup"><span data-stu-id="84a7a-106">Property</span></span>          | <span data-ttu-id="84a7a-107">类型</span><span class="sxs-lookup"><span data-stu-id="84a7a-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="84a7a-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="84a7a-108">reportRefreshDate</span></span> | <span data-ttu-id="84a7a-109">日期</span><span class="sxs-lookup"><span data-stu-id="84a7a-109">Date</span></span>   |
| <span data-ttu-id="84a7a-110">web</span><span class="sxs-lookup"><span data-stu-id="84a7a-110">web</span></span>               | <span data-ttu-id="84a7a-111">Int64</span><span class="sxs-lookup"><span data-stu-id="84a7a-111">Int64</span></span>  |
| <span data-ttu-id="84a7a-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="84a7a-112">windowsPhone</span></span>      | <span data-ttu-id="84a7a-113">Int64</span><span class="sxs-lookup"><span data-stu-id="84a7a-113">Int64</span></span>  |
| <span data-ttu-id="84a7a-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="84a7a-114">androidPhone</span></span>      | <span data-ttu-id="84a7a-115">Int64</span><span class="sxs-lookup"><span data-stu-id="84a7a-115">Int64</span></span>  |
| <span data-ttu-id="84a7a-116">ios</span><span class="sxs-lookup"><span data-stu-id="84a7a-116">ios</span></span>               | <span data-ttu-id="84a7a-117">Int64</span><span class="sxs-lookup"><span data-stu-id="84a7a-117">Int64</span></span>  |
| <span data-ttu-id="84a7a-118">mac</span><span class="sxs-lookup"><span data-stu-id="84a7a-118">mac</span></span>               | <span data-ttu-id="84a7a-119">Int64</span><span class="sxs-lookup"><span data-stu-id="84a7a-119">Int64</span></span>  |
| <span data-ttu-id="84a7a-120">时间</span><span class="sxs-lookup"><span data-stu-id="84a7a-120">windows</span></span>           | <span data-ttu-id="84a7a-121">Int64</span><span class="sxs-lookup"><span data-stu-id="84a7a-121">Int64</span></span>  |
| <span data-ttu-id="84a7a-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="84a7a-122">reportPeriod</span></span>      | <span data-ttu-id="84a7a-123">String</span><span class="sxs-lookup"><span data-stu-id="84a7a-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="84a7a-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84a7a-124">JSON representation</span></span>

<span data-ttu-id="84a7a-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84a7a-125">The following is a JSON representation of the resource.</span></span>

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
