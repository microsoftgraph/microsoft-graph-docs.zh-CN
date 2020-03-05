---
title: skypeForBusinessParticipantActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 863a8ff1fa9b44159cb873c48694cdef749b2e8a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520378"
---
# <a name="skypeforbusinessparticipantactivitycounts-resource-type"></a><span data-ttu-id="e9475-103">skypeForBusinessParticipantActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="e9475-103">skypeForBusinessParticipantActivityCounts resource type</span></span>

<span data-ttu-id="e9475-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e9475-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="e9475-105">属性</span><span class="sxs-lookup"><span data-stu-id="e9475-105">Properties</span></span>

| <span data-ttu-id="e9475-106">属性</span><span class="sxs-lookup"><span data-stu-id="e9475-106">Property</span></span>          | <span data-ttu-id="e9475-107">类型</span><span class="sxs-lookup"><span data-stu-id="e9475-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="e9475-108">即时消息</span><span class="sxs-lookup"><span data-stu-id="e9475-108">im</span></span>                | <span data-ttu-id="e9475-109">Int64</span><span class="sxs-lookup"><span data-stu-id="e9475-109">Int64</span></span>  |
| <span data-ttu-id="e9475-110">audioVideo</span><span class="sxs-lookup"><span data-stu-id="e9475-110">audioVideo</span></span>        | <span data-ttu-id="e9475-111">Int64</span><span class="sxs-lookup"><span data-stu-id="e9475-111">Int64</span></span>  |
| <span data-ttu-id="e9475-112">appSharing</span><span class="sxs-lookup"><span data-stu-id="e9475-112">appSharing</span></span>        | <span data-ttu-id="e9475-113">Int64</span><span class="sxs-lookup"><span data-stu-id="e9475-113">Int64</span></span>  |
| <span data-ttu-id="e9475-114">web</span><span class="sxs-lookup"><span data-stu-id="e9475-114">web</span></span>               | <span data-ttu-id="e9475-115">Int64</span><span class="sxs-lookup"><span data-stu-id="e9475-115">Int64</span></span>  |
| <span data-ttu-id="e9475-116">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="e9475-116">dialInOut3rdParty</span></span> | <span data-ttu-id="e9475-117">Int64</span><span class="sxs-lookup"><span data-stu-id="e9475-117">Int64</span></span>  |
| <span data-ttu-id="e9475-118">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e9475-118">reportRefreshDate</span></span> | <span data-ttu-id="e9475-119">日期</span><span class="sxs-lookup"><span data-stu-id="e9475-119">Date</span></span>   |
| <span data-ttu-id="e9475-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="e9475-120">reportDate</span></span>        | <span data-ttu-id="e9475-121">日期</span><span class="sxs-lookup"><span data-stu-id="e9475-121">Date</span></span>   |
| <span data-ttu-id="e9475-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e9475-122">reportPeriod</span></span>      | <span data-ttu-id="e9475-123">String</span><span class="sxs-lookup"><span data-stu-id="e9475-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e9475-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9475-124">JSON representation</span></span>

<span data-ttu-id="e9475-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9475-125">The following is a JSON representation of the resource.</span></span>

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
