---
title: skypeForBusinessParticipantActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 6579552ef3ca5e9fefe8690a161bef4752ad2492
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853002"
---
# <a name="skypeforbusinessparticipantactivityusercounts-resource-type"></a><span data-ttu-id="55a17-103">skypeForBusinessParticipantActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="55a17-103">skypeForBusinessParticipantActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="55a17-104">属性</span><span class="sxs-lookup"><span data-stu-id="55a17-104">Properties</span></span>

| <span data-ttu-id="55a17-105">属性</span><span class="sxs-lookup"><span data-stu-id="55a17-105">Property</span></span>          | <span data-ttu-id="55a17-106">类型</span><span class="sxs-lookup"><span data-stu-id="55a17-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="55a17-107">im</span><span class="sxs-lookup"><span data-stu-id="55a17-107">im</span></span>                | <span data-ttu-id="55a17-108">Int64</span><span class="sxs-lookup"><span data-stu-id="55a17-108">Int64</span></span>  |
| <span data-ttu-id="55a17-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="55a17-109">audioVideo</span></span>        | <span data-ttu-id="55a17-110">Int64</span><span class="sxs-lookup"><span data-stu-id="55a17-110">Int64</span></span>  |
| <span data-ttu-id="55a17-111">的</span><span class="sxs-lookup"><span data-stu-id="55a17-111">appSharing</span></span>        | <span data-ttu-id="55a17-112">Int64</span><span class="sxs-lookup"><span data-stu-id="55a17-112">Int64</span></span>  |
| <span data-ttu-id="55a17-113">web</span><span class="sxs-lookup"><span data-stu-id="55a17-113">web</span></span>               | <span data-ttu-id="55a17-114">Int64</span><span class="sxs-lookup"><span data-stu-id="55a17-114">Int64</span></span>  |
| <span data-ttu-id="55a17-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="55a17-115">dialInOut3rdParty</span></span> | <span data-ttu-id="55a17-116">Int64</span><span class="sxs-lookup"><span data-stu-id="55a17-116">Int64</span></span>  |
| <span data-ttu-id="55a17-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="55a17-117">reportRefreshDate</span></span> | <span data-ttu-id="55a17-118">日期</span><span class="sxs-lookup"><span data-stu-id="55a17-118">Date</span></span>   |
| <span data-ttu-id="55a17-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="55a17-119">reportDate</span></span>        | <span data-ttu-id="55a17-120">日期</span><span class="sxs-lookup"><span data-stu-id="55a17-120">Date</span></span>   |
| <span data-ttu-id="55a17-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="55a17-121">reportPeriod</span></span>      | <span data-ttu-id="55a17-122">String</span><span class="sxs-lookup"><span data-stu-id="55a17-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="55a17-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55a17-123">JSON representation</span></span>

<span data-ttu-id="55a17-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55a17-124">The following is a JSON representation of the resource.</span></span>

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
