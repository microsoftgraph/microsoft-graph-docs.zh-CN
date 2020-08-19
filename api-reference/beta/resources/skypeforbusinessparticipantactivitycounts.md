---
title: skypeForBusinessParticipantActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 31e7e52de51647faa0748995452c67325c3da83f
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808548"
---
# <a name="skypeforbusinessparticipantactivitycounts-resource-type"></a><span data-ttu-id="03137-103">skypeForBusinessParticipantActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="03137-103">skypeForBusinessParticipantActivityCounts resource type</span></span>

<span data-ttu-id="03137-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03137-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="03137-105">属性</span><span class="sxs-lookup"><span data-stu-id="03137-105">Properties</span></span>

| <span data-ttu-id="03137-106">属性</span><span class="sxs-lookup"><span data-stu-id="03137-106">Property</span></span>          | <span data-ttu-id="03137-107">类型</span><span class="sxs-lookup"><span data-stu-id="03137-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="03137-108">即时消息</span><span class="sxs-lookup"><span data-stu-id="03137-108">im</span></span>                | <span data-ttu-id="03137-109">Int64</span><span class="sxs-lookup"><span data-stu-id="03137-109">Int64</span></span>  |
| <span data-ttu-id="03137-110">audioVideo</span><span class="sxs-lookup"><span data-stu-id="03137-110">audioVideo</span></span>        | <span data-ttu-id="03137-111">Int64</span><span class="sxs-lookup"><span data-stu-id="03137-111">Int64</span></span>  |
| <span data-ttu-id="03137-112">appSharing</span><span class="sxs-lookup"><span data-stu-id="03137-112">appSharing</span></span>        | <span data-ttu-id="03137-113">Int64</span><span class="sxs-lookup"><span data-stu-id="03137-113">Int64</span></span>  |
| <span data-ttu-id="03137-114">web</span><span class="sxs-lookup"><span data-stu-id="03137-114">web</span></span>               | <span data-ttu-id="03137-115">Int64</span><span class="sxs-lookup"><span data-stu-id="03137-115">Int64</span></span>  |
| <span data-ttu-id="03137-116">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="03137-116">dialInOut3rdParty</span></span> | <span data-ttu-id="03137-117">Int64</span><span class="sxs-lookup"><span data-stu-id="03137-117">Int64</span></span>  |
| <span data-ttu-id="03137-118">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="03137-118">reportRefreshDate</span></span> | <span data-ttu-id="03137-119">日期</span><span class="sxs-lookup"><span data-stu-id="03137-119">Date</span></span>   |
| <span data-ttu-id="03137-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="03137-120">reportDate</span></span>        | <span data-ttu-id="03137-121">日期</span><span class="sxs-lookup"><span data-stu-id="03137-121">Date</span></span>   |
| <span data-ttu-id="03137-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="03137-122">reportPeriod</span></span>      | <span data-ttu-id="03137-123">String</span><span class="sxs-lookup"><span data-stu-id="03137-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="03137-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03137-124">JSON representation</span></span>

<span data-ttu-id="03137-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03137-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityCounts"
} -->

```json
{
  "im": 1024,
  "audioVideo": 1024,
  "appSharing": 1024,
  "web": 1024,
  "dialInOut3rdParty": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```
