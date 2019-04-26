---
title: skypeForBusinessParticipantActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: de86c49da34c9af48478a912a6ab042a354a7bf5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568087"
---
# <a name="skypeforbusinessparticipantactivitycounts-resource-type"></a><span data-ttu-id="28bac-103">skypeForBusinessParticipantActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="28bac-103">skypeForBusinessParticipantActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="28bac-104">属性</span><span class="sxs-lookup"><span data-stu-id="28bac-104">Properties</span></span>

| <span data-ttu-id="28bac-105">属性</span><span class="sxs-lookup"><span data-stu-id="28bac-105">Property</span></span>          | <span data-ttu-id="28bac-106">类型</span><span class="sxs-lookup"><span data-stu-id="28bac-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="28bac-107">即时消息</span><span class="sxs-lookup"><span data-stu-id="28bac-107">im</span></span>                | <span data-ttu-id="28bac-108">Int64</span><span class="sxs-lookup"><span data-stu-id="28bac-108">Int64</span></span>  |
| <span data-ttu-id="28bac-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="28bac-109">audioVideo</span></span>        | <span data-ttu-id="28bac-110">Int64</span><span class="sxs-lookup"><span data-stu-id="28bac-110">Int64</span></span>  |
| <span data-ttu-id="28bac-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="28bac-111">appSharing</span></span>        | <span data-ttu-id="28bac-112">Int64</span><span class="sxs-lookup"><span data-stu-id="28bac-112">Int64</span></span>  |
| <span data-ttu-id="28bac-113">web</span><span class="sxs-lookup"><span data-stu-id="28bac-113">web</span></span>               | <span data-ttu-id="28bac-114">Int64</span><span class="sxs-lookup"><span data-stu-id="28bac-114">Int64</span></span>  |
| <span data-ttu-id="28bac-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="28bac-115">dialInOut3rdParty</span></span> | <span data-ttu-id="28bac-116">Int64</span><span class="sxs-lookup"><span data-stu-id="28bac-116">Int64</span></span>  |
| <span data-ttu-id="28bac-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="28bac-117">reportRefreshDate</span></span> | <span data-ttu-id="28bac-118">Date</span><span class="sxs-lookup"><span data-stu-id="28bac-118">Date</span></span>   |
| <span data-ttu-id="28bac-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="28bac-119">reportDate</span></span>        | <span data-ttu-id="28bac-120">Date</span><span class="sxs-lookup"><span data-stu-id="28bac-120">Date</span></span>   |
| <span data-ttu-id="28bac-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="28bac-121">reportPeriod</span></span>      | <span data-ttu-id="28bac-122">String</span><span class="sxs-lookup"><span data-stu-id="28bac-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="28bac-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28bac-123">JSON representation</span></span>

<span data-ttu-id="28bac-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28bac-124">The following is a JSON representation of the resource.</span></span>

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
