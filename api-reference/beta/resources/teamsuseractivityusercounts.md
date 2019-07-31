---
title: teamsUserActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f0b6d9d77518b6e40a5793c6715bfbae69600f3c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964359"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="0285a-103">teamsUserActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="0285a-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="0285a-104">属性</span><span class="sxs-lookup"><span data-stu-id="0285a-104">Properties</span></span>

| <span data-ttu-id="0285a-105">属性</span><span class="sxs-lookup"><span data-stu-id="0285a-105">Property</span></span>            | <span data-ttu-id="0285a-106">类型</span><span class="sxs-lookup"><span data-stu-id="0285a-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="0285a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0285a-107">reportRefreshDate</span></span>   | <span data-ttu-id="0285a-108">日期</span><span class="sxs-lookup"><span data-stu-id="0285a-108">Date</span></span>   |
| <span data-ttu-id="0285a-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="0285a-109">reportDate</span></span>          | <span data-ttu-id="0285a-110">日期</span><span class="sxs-lookup"><span data-stu-id="0285a-110">Date</span></span>   |
| <span data-ttu-id="0285a-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="0285a-111">teamChatMessages</span></span>    | <span data-ttu-id="0285a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="0285a-112">Int64</span></span>  |
| <span data-ttu-id="0285a-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="0285a-113">privateChatMessages</span></span> | <span data-ttu-id="0285a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="0285a-114">Int64</span></span>  |
| <span data-ttu-id="0285a-115">calls</span><span class="sxs-lookup"><span data-stu-id="0285a-115">calls</span></span>               | <span data-ttu-id="0285a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="0285a-116">Int64</span></span>  |
| <span data-ttu-id="0285a-117">会议</span><span class="sxs-lookup"><span data-stu-id="0285a-117">meetings</span></span>            | <span data-ttu-id="0285a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="0285a-118">Int64</span></span>  |
| <span data-ttu-id="0285a-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="0285a-119">otherActions</span></span>        | <span data-ttu-id="0285a-120">Int64</span><span class="sxs-lookup"><span data-stu-id="0285a-120">Int64</span></span>  |
| <span data-ttu-id="0285a-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0285a-121">reportPeriod</span></span>        | <span data-ttu-id="0285a-122">String</span><span class="sxs-lookup"><span data-stu-id="0285a-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0285a-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0285a-123">JSON representation</span></span>

<span data-ttu-id="0285a-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0285a-124">The following is a JSON representation of the resource.</span></span>

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
