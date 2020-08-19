---
title: skypeForBusinessOrganizerActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 6708a9e0ac1be42378933e217ec282982dee4981
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811048"
---
# <a name="skypeforbusinessorganizeractivitycounts-resource-type"></a><span data-ttu-id="563a9-103">skypeForBusinessOrganizerActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="563a9-103">skypeForBusinessOrganizerActivityCounts resource type</span></span>

<span data-ttu-id="563a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="563a9-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="563a9-105">属性</span><span class="sxs-lookup"><span data-stu-id="563a9-105">Properties</span></span>

| <span data-ttu-id="563a9-106">属性</span><span class="sxs-lookup"><span data-stu-id="563a9-106">Property</span></span>           | <span data-ttu-id="563a9-107">类型</span><span class="sxs-lookup"><span data-stu-id="563a9-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="563a9-108">即时消息</span><span class="sxs-lookup"><span data-stu-id="563a9-108">im</span></span>                 | <span data-ttu-id="563a9-109">Int64</span><span class="sxs-lookup"><span data-stu-id="563a9-109">Int64</span></span>  |
| <span data-ttu-id="563a9-110">audioVideo</span><span class="sxs-lookup"><span data-stu-id="563a9-110">audioVideo</span></span>         | <span data-ttu-id="563a9-111">Int64</span><span class="sxs-lookup"><span data-stu-id="563a9-111">Int64</span></span>  |
| <span data-ttu-id="563a9-112">appSharing</span><span class="sxs-lookup"><span data-stu-id="563a9-112">appSharing</span></span>         | <span data-ttu-id="563a9-113">Int64</span><span class="sxs-lookup"><span data-stu-id="563a9-113">Int64</span></span>  |
| <span data-ttu-id="563a9-114">web</span><span class="sxs-lookup"><span data-stu-id="563a9-114">web</span></span>                | <span data-ttu-id="563a9-115">Int64</span><span class="sxs-lookup"><span data-stu-id="563a9-115">Int64</span></span>  |
| <span data-ttu-id="563a9-116">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="563a9-116">dialInOut3rdParty</span></span>  | <span data-ttu-id="563a9-117">Int64</span><span class="sxs-lookup"><span data-stu-id="563a9-117">Int64</span></span>  |
| <span data-ttu-id="563a9-118">dialInOutMicrosoft</span><span class="sxs-lookup"><span data-stu-id="563a9-118">dialInOutMicrosoft</span></span> | <span data-ttu-id="563a9-119">Int64</span><span class="sxs-lookup"><span data-stu-id="563a9-119">Int64</span></span>  |
| <span data-ttu-id="563a9-120">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="563a9-120">reportRefreshDate</span></span>  | <span data-ttu-id="563a9-121">日期</span><span class="sxs-lookup"><span data-stu-id="563a9-121">Date</span></span>   |
| <span data-ttu-id="563a9-122">reportDate</span><span class="sxs-lookup"><span data-stu-id="563a9-122">reportDate</span></span>         | <span data-ttu-id="563a9-123">日期</span><span class="sxs-lookup"><span data-stu-id="563a9-123">Date</span></span>   |
| <span data-ttu-id="563a9-124">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="563a9-124">reportPeriod</span></span>       | <span data-ttu-id="563a9-125">String</span><span class="sxs-lookup"><span data-stu-id="563a9-125">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="563a9-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="563a9-126">JSON representation</span></span>

<span data-ttu-id="563a9-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="563a9-127">The following is a JSON representation of the resource.</span></span>

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
