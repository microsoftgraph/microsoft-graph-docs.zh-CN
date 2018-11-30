---
title: skypeForBusinessParticipantActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 1e61526b281a87370835e8f6558ab3f0cb5707a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045208"
---
# <a name="skypeforbusinessparticipantactivitycounts-resource-type"></a><span data-ttu-id="217ff-103">skypeForBusinessParticipantActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="217ff-103">skypeForBusinessParticipantActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="217ff-104">属性</span><span class="sxs-lookup"><span data-stu-id="217ff-104">Properties</span></span>

| <span data-ttu-id="217ff-105">属性</span><span class="sxs-lookup"><span data-stu-id="217ff-105">Property</span></span>          | <span data-ttu-id="217ff-106">类型</span><span class="sxs-lookup"><span data-stu-id="217ff-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="217ff-107">im</span><span class="sxs-lookup"><span data-stu-id="217ff-107">im</span></span>                | <span data-ttu-id="217ff-108">Int64</span><span class="sxs-lookup"><span data-stu-id="217ff-108">Int64</span></span>  |
| <span data-ttu-id="217ff-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="217ff-109">audioVideo</span></span>        | <span data-ttu-id="217ff-110">Int64</span><span class="sxs-lookup"><span data-stu-id="217ff-110">Int64</span></span>  |
| <span data-ttu-id="217ff-111">的</span><span class="sxs-lookup"><span data-stu-id="217ff-111">appSharing</span></span>        | <span data-ttu-id="217ff-112">Int64</span><span class="sxs-lookup"><span data-stu-id="217ff-112">Int64</span></span>  |
| <span data-ttu-id="217ff-113">web</span><span class="sxs-lookup"><span data-stu-id="217ff-113">web</span></span>               | <span data-ttu-id="217ff-114">Int64</span><span class="sxs-lookup"><span data-stu-id="217ff-114">Int64</span></span>  |
| <span data-ttu-id="217ff-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="217ff-115">dialInOut3rdParty</span></span> | <span data-ttu-id="217ff-116">Int64</span><span class="sxs-lookup"><span data-stu-id="217ff-116">Int64</span></span>  |
| <span data-ttu-id="217ff-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="217ff-117">reportRefreshDate</span></span> | <span data-ttu-id="217ff-118">日期</span><span class="sxs-lookup"><span data-stu-id="217ff-118">Date</span></span>   |
| <span data-ttu-id="217ff-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="217ff-119">reportDate</span></span>        | <span data-ttu-id="217ff-120">日期</span><span class="sxs-lookup"><span data-stu-id="217ff-120">Date</span></span>   |
| <span data-ttu-id="217ff-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="217ff-121">reportPeriod</span></span>      | <span data-ttu-id="217ff-122">String</span><span class="sxs-lookup"><span data-stu-id="217ff-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="217ff-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="217ff-123">JSON representation</span></span>

<span data-ttu-id="217ff-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="217ff-124">The following is a JSON representation of the resource.</span></span>

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
