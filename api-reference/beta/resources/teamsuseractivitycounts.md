---
title: teamsUserActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcc0e9d1ed5c93c3d9f4ba97165d0413025a89cd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987522"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="6ca8a-103">teamsUserActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ca8a-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6ca8a-104">属性</span><span class="sxs-lookup"><span data-stu-id="6ca8a-104">Properties</span></span>

| <span data-ttu-id="6ca8a-105">属性</span><span class="sxs-lookup"><span data-stu-id="6ca8a-105">Property</span></span>            | <span data-ttu-id="6ca8a-106">类型</span><span class="sxs-lookup"><span data-stu-id="6ca8a-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="6ca8a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6ca8a-107">reportRefreshDate</span></span>   | <span data-ttu-id="6ca8a-108">日期</span><span class="sxs-lookup"><span data-stu-id="6ca8a-108">Date</span></span>   |
| <span data-ttu-id="6ca8a-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="6ca8a-109">reportDate</span></span>          | <span data-ttu-id="6ca8a-110">日期</span><span class="sxs-lookup"><span data-stu-id="6ca8a-110">Date</span></span>   |
| <span data-ttu-id="6ca8a-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="6ca8a-111">teamChatMessages</span></span>    | <span data-ttu-id="6ca8a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6ca8a-112">Int64</span></span>  |
| <span data-ttu-id="6ca8a-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="6ca8a-113">privateChatMessages</span></span> | <span data-ttu-id="6ca8a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6ca8a-114">Int64</span></span>  |
| <span data-ttu-id="6ca8a-115">呼叫</span><span class="sxs-lookup"><span data-stu-id="6ca8a-115">calls</span></span>               | <span data-ttu-id="6ca8a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="6ca8a-116">Int64</span></span>  |
| <span data-ttu-id="6ca8a-117">会议</span><span class="sxs-lookup"><span data-stu-id="6ca8a-117">meetings</span></span>            | <span data-ttu-id="6ca8a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="6ca8a-118">Int64</span></span>  |
| <span data-ttu-id="6ca8a-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6ca8a-119">reportPeriod</span></span>        | <span data-ttu-id="6ca8a-120">String</span><span class="sxs-lookup"><span data-stu-id="6ca8a-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="6ca8a-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ca8a-121">JSON representation</span></span>

<span data-ttu-id="6ca8a-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ca8a-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```
