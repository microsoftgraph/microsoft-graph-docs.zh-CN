---
title: skypeForBusinessParticipantActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 00a5fb92c4007ad9f5a902abad53291f7b5d8527
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063924"
---
# <a name="skypeforbusinessparticipantactivitycounts-resource-type"></a><span data-ttu-id="9d737-103">skypeForBusinessParticipantActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d737-103">skypeForBusinessParticipantActivityCounts resource type</span></span>

<span data-ttu-id="9d737-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d737-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="9d737-105">属性</span><span class="sxs-lookup"><span data-stu-id="9d737-105">Properties</span></span>

| <span data-ttu-id="9d737-106">属性</span><span class="sxs-lookup"><span data-stu-id="9d737-106">Property</span></span>          | <span data-ttu-id="9d737-107">类型</span><span class="sxs-lookup"><span data-stu-id="9d737-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="9d737-108">即时消息</span><span class="sxs-lookup"><span data-stu-id="9d737-108">im</span></span>                | <span data-ttu-id="9d737-109">Int64</span><span class="sxs-lookup"><span data-stu-id="9d737-109">Int64</span></span>  |
| <span data-ttu-id="9d737-110">audioVideo</span><span class="sxs-lookup"><span data-stu-id="9d737-110">audioVideo</span></span>        | <span data-ttu-id="9d737-111">Int64</span><span class="sxs-lookup"><span data-stu-id="9d737-111">Int64</span></span>  |
| <span data-ttu-id="9d737-112">appSharing</span><span class="sxs-lookup"><span data-stu-id="9d737-112">appSharing</span></span>        | <span data-ttu-id="9d737-113">Int64</span><span class="sxs-lookup"><span data-stu-id="9d737-113">Int64</span></span>  |
| <span data-ttu-id="9d737-114">web</span><span class="sxs-lookup"><span data-stu-id="9d737-114">web</span></span>               | <span data-ttu-id="9d737-115">Int64</span><span class="sxs-lookup"><span data-stu-id="9d737-115">Int64</span></span>  |
| <span data-ttu-id="9d737-116">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="9d737-116">dialInOut3rdParty</span></span> | <span data-ttu-id="9d737-117">Int64</span><span class="sxs-lookup"><span data-stu-id="9d737-117">Int64</span></span>  |
| <span data-ttu-id="9d737-118">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="9d737-118">reportRefreshDate</span></span> | <span data-ttu-id="9d737-119">日期</span><span class="sxs-lookup"><span data-stu-id="9d737-119">Date</span></span>   |
| <span data-ttu-id="9d737-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="9d737-120">reportDate</span></span>        | <span data-ttu-id="9d737-121">日期</span><span class="sxs-lookup"><span data-stu-id="9d737-121">Date</span></span>   |
| <span data-ttu-id="9d737-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="9d737-122">reportPeriod</span></span>      | <span data-ttu-id="9d737-123">String</span><span class="sxs-lookup"><span data-stu-id="9d737-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9d737-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d737-124">JSON representation</span></span>

<span data-ttu-id="9d737-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d737-125">The following is a JSON representation of the resource.</span></span>

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


