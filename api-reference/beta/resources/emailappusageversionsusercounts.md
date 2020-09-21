---
title: emailAppUsageVersionsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 68ff3fad4275fe4b013c7c527de786a8c02c10cd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979432"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="6eec9-103">emailAppUsageVersionsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="6eec9-103">emailAppUsageVersionsUserCounts resource type</span></span>

<span data-ttu-id="6eec9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6eec9-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="6eec9-105">属性</span><span class="sxs-lookup"><span data-stu-id="6eec9-105">Properties</span></span>

| <span data-ttu-id="6eec9-106">属性</span><span class="sxs-lookup"><span data-stu-id="6eec9-106">Property</span></span>          | <span data-ttu-id="6eec9-107">类型</span><span class="sxs-lookup"><span data-stu-id="6eec9-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="6eec9-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6eec9-108">reportRefreshDate</span></span> | <span data-ttu-id="6eec9-109">日期</span><span class="sxs-lookup"><span data-stu-id="6eec9-109">Date</span></span>   |
| <span data-ttu-id="6eec9-110">outlook2016</span><span class="sxs-lookup"><span data-stu-id="6eec9-110">outlook2016</span></span>       | <span data-ttu-id="6eec9-111">Int64</span><span class="sxs-lookup"><span data-stu-id="6eec9-111">Int64</span></span>  |
| <span data-ttu-id="6eec9-112">outlook2013</span><span class="sxs-lookup"><span data-stu-id="6eec9-112">outlook2013</span></span>       | <span data-ttu-id="6eec9-113">Int64</span><span class="sxs-lookup"><span data-stu-id="6eec9-113">Int64</span></span>  |
| <span data-ttu-id="6eec9-114">outlook2010</span><span class="sxs-lookup"><span data-stu-id="6eec9-114">outlook2010</span></span>       | <span data-ttu-id="6eec9-115">Int64</span><span class="sxs-lookup"><span data-stu-id="6eec9-115">Int64</span></span>  |
| <span data-ttu-id="6eec9-116">outlook2007</span><span class="sxs-lookup"><span data-stu-id="6eec9-116">outlook2007</span></span>       | <span data-ttu-id="6eec9-117">Int64</span><span class="sxs-lookup"><span data-stu-id="6eec9-117">Int64</span></span>  |
| <span data-ttu-id="6eec9-118">流程</span><span class="sxs-lookup"><span data-stu-id="6eec9-118">undetermined</span></span>      | <span data-ttu-id="6eec9-119">Int64</span><span class="sxs-lookup"><span data-stu-id="6eec9-119">Int64</span></span>  |
| <span data-ttu-id="6eec9-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6eec9-120">reportPeriod</span></span>      | <span data-ttu-id="6eec9-121">String</span><span class="sxs-lookup"><span data-stu-id="6eec9-121">String</span></span> |
| <span data-ttu-id="6eec9-122">outlookM365</span><span class="sxs-lookup"><span data-stu-id="6eec9-122">outlookM365</span></span>       | <span data-ttu-id="6eec9-123">Int64</span><span class="sxs-lookup"><span data-stu-id="6eec9-123">Int64</span></span>  |
| <span data-ttu-id="6eec9-124">outlook2019</span><span class="sxs-lookup"><span data-stu-id="6eec9-124">outlook2019</span></span>       | <span data-ttu-id="6eec9-125">Int64</span><span class="sxs-lookup"><span data-stu-id="6eec9-125">Int64</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="6eec9-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6eec9-126">JSON representation</span></span>

<span data-ttu-id="6eec9-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6eec9-127">The following is a JSON representation of the resource.</span></span>

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


