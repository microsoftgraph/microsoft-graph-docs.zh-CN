---
title: teamsUserActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 39e90b4c9dc6b9929959139ba67ddb090d143e38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048131"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="307a3-103">teamsUserActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="307a3-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="307a3-104">属性</span><span class="sxs-lookup"><span data-stu-id="307a3-104">Properties</span></span>

| <span data-ttu-id="307a3-105">属性</span><span class="sxs-lookup"><span data-stu-id="307a3-105">Property</span></span>            | <span data-ttu-id="307a3-106">类型</span><span class="sxs-lookup"><span data-stu-id="307a3-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="307a3-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="307a3-107">reportRefreshDate</span></span>   | <span data-ttu-id="307a3-108">日期</span><span class="sxs-lookup"><span data-stu-id="307a3-108">Date</span></span>   |
| <span data-ttu-id="307a3-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="307a3-109">reportDate</span></span>          | <span data-ttu-id="307a3-110">日期</span><span class="sxs-lookup"><span data-stu-id="307a3-110">Date</span></span>   |
| <span data-ttu-id="307a3-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="307a3-111">teamChatMessages</span></span>    | <span data-ttu-id="307a3-112">Int64</span><span class="sxs-lookup"><span data-stu-id="307a3-112">Int64</span></span>  |
| <span data-ttu-id="307a3-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="307a3-113">privateChatMessages</span></span> | <span data-ttu-id="307a3-114">Int64</span><span class="sxs-lookup"><span data-stu-id="307a3-114">Int64</span></span>  |
| <span data-ttu-id="307a3-115">呼叫</span><span class="sxs-lookup"><span data-stu-id="307a3-115">calls</span></span>               | <span data-ttu-id="307a3-116">Int64</span><span class="sxs-lookup"><span data-stu-id="307a3-116">Int64</span></span>  |
| <span data-ttu-id="307a3-117">会议</span><span class="sxs-lookup"><span data-stu-id="307a3-117">meetings</span></span>            | <span data-ttu-id="307a3-118">Int64</span><span class="sxs-lookup"><span data-stu-id="307a3-118">Int64</span></span>  |
| <span data-ttu-id="307a3-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="307a3-119">reportPeriod</span></span>        | <span data-ttu-id="307a3-120">String</span><span class="sxs-lookup"><span data-stu-id="307a3-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="307a3-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="307a3-121">JSON representation</span></span>

<span data-ttu-id="307a3-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="307a3-122">The following is a JSON representation of the resource.</span></span>

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
