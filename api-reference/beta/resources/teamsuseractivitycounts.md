---
title: teamsUserActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9e1a40d962ded7825b72d31675cefb9869750866
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007618"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="753d2-103">teamsUserActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="753d2-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="753d2-104">属性</span><span class="sxs-lookup"><span data-stu-id="753d2-104">Properties</span></span>

| <span data-ttu-id="753d2-105">属性</span><span class="sxs-lookup"><span data-stu-id="753d2-105">Property</span></span>            | <span data-ttu-id="753d2-106">类型</span><span class="sxs-lookup"><span data-stu-id="753d2-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="753d2-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="753d2-107">reportRefreshDate</span></span>   | <span data-ttu-id="753d2-108">日期</span><span class="sxs-lookup"><span data-stu-id="753d2-108">Date</span></span>   |
| <span data-ttu-id="753d2-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="753d2-109">reportDate</span></span>          | <span data-ttu-id="753d2-110">日期</span><span class="sxs-lookup"><span data-stu-id="753d2-110">Date</span></span>   |
| <span data-ttu-id="753d2-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="753d2-111">teamChatMessages</span></span>    | <span data-ttu-id="753d2-112">Int64</span><span class="sxs-lookup"><span data-stu-id="753d2-112">Int64</span></span>  |
| <span data-ttu-id="753d2-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="753d2-113">privateChatMessages</span></span> | <span data-ttu-id="753d2-114">Int64</span><span class="sxs-lookup"><span data-stu-id="753d2-114">Int64</span></span>  |
| <span data-ttu-id="753d2-115">calls</span><span class="sxs-lookup"><span data-stu-id="753d2-115">calls</span></span>               | <span data-ttu-id="753d2-116">Int64</span><span class="sxs-lookup"><span data-stu-id="753d2-116">Int64</span></span>  |
| <span data-ttu-id="753d2-117">会议</span><span class="sxs-lookup"><span data-stu-id="753d2-117">meetings</span></span>            | <span data-ttu-id="753d2-118">Int64</span><span class="sxs-lookup"><span data-stu-id="753d2-118">Int64</span></span>  |
| <span data-ttu-id="753d2-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="753d2-119">reportPeriod</span></span>        | <span data-ttu-id="753d2-120">String</span><span class="sxs-lookup"><span data-stu-id="753d2-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="753d2-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="753d2-121">JSON representation</span></span>

<span data-ttu-id="753d2-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="753d2-122">The following is a JSON representation of the resource.</span></span>

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
