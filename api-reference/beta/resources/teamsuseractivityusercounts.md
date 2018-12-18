---
title: teamsUserActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
ms.openlocfilehash: f4e10f1e34d4c6bdbed83279b98632c504630bc7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330455"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="f2ab3-103">teamsUserActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2ab3-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f2ab3-104">属性</span><span class="sxs-lookup"><span data-stu-id="f2ab3-104">Properties</span></span>

| <span data-ttu-id="f2ab3-105">属性</span><span class="sxs-lookup"><span data-stu-id="f2ab3-105">Property</span></span>            | <span data-ttu-id="f2ab3-106">类型</span><span class="sxs-lookup"><span data-stu-id="f2ab3-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="f2ab3-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f2ab3-107">reportRefreshDate</span></span>   | <span data-ttu-id="f2ab3-108">日期</span><span class="sxs-lookup"><span data-stu-id="f2ab3-108">Date</span></span>   |
| <span data-ttu-id="f2ab3-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="f2ab3-109">reportDate</span></span>          | <span data-ttu-id="f2ab3-110">日期</span><span class="sxs-lookup"><span data-stu-id="f2ab3-110">Date</span></span>   |
| <span data-ttu-id="f2ab3-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="f2ab3-111">teamChatMessages</span></span>    | <span data-ttu-id="f2ab3-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f2ab3-112">Int64</span></span>  |
| <span data-ttu-id="f2ab3-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="f2ab3-113">privateChatMessages</span></span> | <span data-ttu-id="f2ab3-114">Int64</span><span class="sxs-lookup"><span data-stu-id="f2ab3-114">Int64</span></span>  |
| <span data-ttu-id="f2ab3-115">呼叫</span><span class="sxs-lookup"><span data-stu-id="f2ab3-115">calls</span></span>               | <span data-ttu-id="f2ab3-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f2ab3-116">Int64</span></span>  |
| <span data-ttu-id="f2ab3-117">会议</span><span class="sxs-lookup"><span data-stu-id="f2ab3-117">meetings</span></span>            | <span data-ttu-id="f2ab3-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f2ab3-118">Int64</span></span>  |
| <span data-ttu-id="f2ab3-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="f2ab3-119">otherActions</span></span>        | <span data-ttu-id="f2ab3-120">Int64</span><span class="sxs-lookup"><span data-stu-id="f2ab3-120">Int64</span></span>  |
| <span data-ttu-id="f2ab3-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f2ab3-121">reportPeriod</span></span>        | <span data-ttu-id="f2ab3-122">String</span><span class="sxs-lookup"><span data-stu-id="f2ab3-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f2ab3-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2ab3-123">JSON representation</span></span>

<span data-ttu-id="f2ab3-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2ab3-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "otherActions": 1024, 
  "reportPeriod": "String"
}
```
