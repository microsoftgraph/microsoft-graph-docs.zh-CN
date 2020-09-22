---
title: skypeForBusinessOrganizerActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: aa0721c13d78be8b88e399b1342d8f0c0ecd3efa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997514"
---
# <a name="skypeforbusinessorganizeractivitycounts-resource-type"></a><span data-ttu-id="74469-103">skypeForBusinessOrganizerActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="74469-103">skypeForBusinessOrganizerActivityCounts resource type</span></span>

<span data-ttu-id="74469-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74469-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="74469-105">属性</span><span class="sxs-lookup"><span data-stu-id="74469-105">Properties</span></span>

| <span data-ttu-id="74469-106">属性</span><span class="sxs-lookup"><span data-stu-id="74469-106">Property</span></span>           | <span data-ttu-id="74469-107">类型</span><span class="sxs-lookup"><span data-stu-id="74469-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="74469-108">即时消息</span><span class="sxs-lookup"><span data-stu-id="74469-108">im</span></span>                 | <span data-ttu-id="74469-109">Int64</span><span class="sxs-lookup"><span data-stu-id="74469-109">Int64</span></span>  |
| <span data-ttu-id="74469-110">audioVideo</span><span class="sxs-lookup"><span data-stu-id="74469-110">audioVideo</span></span>         | <span data-ttu-id="74469-111">Int64</span><span class="sxs-lookup"><span data-stu-id="74469-111">Int64</span></span>  |
| <span data-ttu-id="74469-112">appSharing</span><span class="sxs-lookup"><span data-stu-id="74469-112">appSharing</span></span>         | <span data-ttu-id="74469-113">Int64</span><span class="sxs-lookup"><span data-stu-id="74469-113">Int64</span></span>  |
| <span data-ttu-id="74469-114">web</span><span class="sxs-lookup"><span data-stu-id="74469-114">web</span></span>                | <span data-ttu-id="74469-115">Int64</span><span class="sxs-lookup"><span data-stu-id="74469-115">Int64</span></span>  |
| <span data-ttu-id="74469-116">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="74469-116">dialInOut3rdParty</span></span>  | <span data-ttu-id="74469-117">Int64</span><span class="sxs-lookup"><span data-stu-id="74469-117">Int64</span></span>  |
| <span data-ttu-id="74469-118">dialInOutMicrosoft</span><span class="sxs-lookup"><span data-stu-id="74469-118">dialInOutMicrosoft</span></span> | <span data-ttu-id="74469-119">Int64</span><span class="sxs-lookup"><span data-stu-id="74469-119">Int64</span></span>  |
| <span data-ttu-id="74469-120">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="74469-120">reportRefreshDate</span></span>  | <span data-ttu-id="74469-121">日期</span><span class="sxs-lookup"><span data-stu-id="74469-121">Date</span></span>   |
| <span data-ttu-id="74469-122">reportDate</span><span class="sxs-lookup"><span data-stu-id="74469-122">reportDate</span></span>         | <span data-ttu-id="74469-123">日期</span><span class="sxs-lookup"><span data-stu-id="74469-123">Date</span></span>   |
| <span data-ttu-id="74469-124">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="74469-124">reportPeriod</span></span>       | <span data-ttu-id="74469-125">String</span><span class="sxs-lookup"><span data-stu-id="74469-125">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="74469-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="74469-126">JSON representation</span></span>

<span data-ttu-id="74469-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74469-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityCounts"
} -->

```json
{
  "im": 1024,
  "audioVideo": 1024,
  "appSharing": 1024,
  "web": 1024,
  "dialInOut3rdParty": 1024,
  "dialInOutMicrosoft": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```


