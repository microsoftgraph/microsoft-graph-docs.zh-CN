---
title: skypeForBusinessParticipantActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: e53ef85ce3fbe0be2a36adc218d565bdb78f64a0
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811068"
---
# <a name="skypeforbusinessparticipantactivityusercounts-resource-type"></a><span data-ttu-id="51096-103">skypeForBusinessParticipantActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="51096-103">skypeForBusinessParticipantActivityUserCounts resource type</span></span>

<span data-ttu-id="51096-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51096-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="51096-105">属性</span><span class="sxs-lookup"><span data-stu-id="51096-105">Properties</span></span>

| <span data-ttu-id="51096-106">属性</span><span class="sxs-lookup"><span data-stu-id="51096-106">Property</span></span>          | <span data-ttu-id="51096-107">类型</span><span class="sxs-lookup"><span data-stu-id="51096-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="51096-108">即时消息</span><span class="sxs-lookup"><span data-stu-id="51096-108">im</span></span>                | <span data-ttu-id="51096-109">Int64</span><span class="sxs-lookup"><span data-stu-id="51096-109">Int64</span></span>  |
| <span data-ttu-id="51096-110">audioVideo</span><span class="sxs-lookup"><span data-stu-id="51096-110">audioVideo</span></span>        | <span data-ttu-id="51096-111">Int64</span><span class="sxs-lookup"><span data-stu-id="51096-111">Int64</span></span>  |
| <span data-ttu-id="51096-112">appSharing</span><span class="sxs-lookup"><span data-stu-id="51096-112">appSharing</span></span>        | <span data-ttu-id="51096-113">Int64</span><span class="sxs-lookup"><span data-stu-id="51096-113">Int64</span></span>  |
| <span data-ttu-id="51096-114">web</span><span class="sxs-lookup"><span data-stu-id="51096-114">web</span></span>               | <span data-ttu-id="51096-115">Int64</span><span class="sxs-lookup"><span data-stu-id="51096-115">Int64</span></span>  |
| <span data-ttu-id="51096-116">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="51096-116">dialInOut3rdParty</span></span> | <span data-ttu-id="51096-117">Int64</span><span class="sxs-lookup"><span data-stu-id="51096-117">Int64</span></span>  |
| <span data-ttu-id="51096-118">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="51096-118">reportRefreshDate</span></span> | <span data-ttu-id="51096-119">日期</span><span class="sxs-lookup"><span data-stu-id="51096-119">Date</span></span>   |
| <span data-ttu-id="51096-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="51096-120">reportDate</span></span>        | <span data-ttu-id="51096-121">日期</span><span class="sxs-lookup"><span data-stu-id="51096-121">Date</span></span>   |
| <span data-ttu-id="51096-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="51096-122">reportPeriod</span></span>      | <span data-ttu-id="51096-123">String</span><span class="sxs-lookup"><span data-stu-id="51096-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="51096-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51096-124">JSON representation</span></span>

<span data-ttu-id="51096-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51096-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityUserCounts"
} -->

```json
{
  "im": 1024,
  "audioVideo": 196,
  "appSharing": 196,
  "web": 196,
  "dialInOut3rdParty": 196,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```
