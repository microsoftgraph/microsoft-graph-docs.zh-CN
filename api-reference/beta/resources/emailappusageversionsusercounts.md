---
title: emailAppUsageVersionsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 25ccb7352319c9faa58a36ad2272448f8428457a
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983613"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="19646-103">emailAppUsageVersionsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="19646-103">emailAppUsageVersionsUserCounts resource type</span></span>

<span data-ttu-id="19646-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19646-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="19646-105">属性</span><span class="sxs-lookup"><span data-stu-id="19646-105">Properties</span></span>

| <span data-ttu-id="19646-106">属性</span><span class="sxs-lookup"><span data-stu-id="19646-106">Property</span></span>          | <span data-ttu-id="19646-107">类型</span><span class="sxs-lookup"><span data-stu-id="19646-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="19646-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="19646-108">reportRefreshDate</span></span> | <span data-ttu-id="19646-109">日期</span><span class="sxs-lookup"><span data-stu-id="19646-109">Date</span></span>   |
| <span data-ttu-id="19646-110">outlook2016</span><span class="sxs-lookup"><span data-stu-id="19646-110">outlook2016</span></span>       | <span data-ttu-id="19646-111">Int64</span><span class="sxs-lookup"><span data-stu-id="19646-111">Int64</span></span>  |
| <span data-ttu-id="19646-112">outlook2013</span><span class="sxs-lookup"><span data-stu-id="19646-112">outlook2013</span></span>       | <span data-ttu-id="19646-113">Int64</span><span class="sxs-lookup"><span data-stu-id="19646-113">Int64</span></span>  |
| <span data-ttu-id="19646-114">outlook2010</span><span class="sxs-lookup"><span data-stu-id="19646-114">outlook2010</span></span>       | <span data-ttu-id="19646-115">Int64</span><span class="sxs-lookup"><span data-stu-id="19646-115">Int64</span></span>  |
| <span data-ttu-id="19646-116">outlook2007</span><span class="sxs-lookup"><span data-stu-id="19646-116">outlook2007</span></span>       | <span data-ttu-id="19646-117">Int64</span><span class="sxs-lookup"><span data-stu-id="19646-117">Int64</span></span>  |
| <span data-ttu-id="19646-118">不确定</span><span class="sxs-lookup"><span data-stu-id="19646-118">undetermined</span></span>      | <span data-ttu-id="19646-119">Int64</span><span class="sxs-lookup"><span data-stu-id="19646-119">Int64</span></span>  |
| <span data-ttu-id="19646-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="19646-120">reportPeriod</span></span>      | <span data-ttu-id="19646-121">String</span><span class="sxs-lookup"><span data-stu-id="19646-121">String</span></span> |
| <span data-ttu-id="19646-122">outlookM365</span><span class="sxs-lookup"><span data-stu-id="19646-122">outlookM365</span></span>       | <span data-ttu-id="19646-123">Int64</span><span class="sxs-lookup"><span data-stu-id="19646-123">Int64</span></span>  |
| <span data-ttu-id="19646-124">outlook2019</span><span class="sxs-lookup"><span data-stu-id="19646-124">outlook2019</span></span>       | <span data-ttu-id="19646-125">Int64</span><span class="sxs-lookup"><span data-stu-id="19646-125">Int64</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="19646-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19646-126">JSON representation</span></span>

<span data-ttu-id="19646-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19646-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "outlook2016": 1024, 
  "outlook2013": 1024, 
  "outlook2010": 1024, 
  "outlook2007": 1024, 
  "undetermined": 1024, 
  "reportPeriod": "String",
  "outlookM365": 1024,
  "outlook2019": 1024
}
```


