---
title: teamsUserActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3066877d109e7dd61243b7cd2f4c105b03c0c533
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519825"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="f0fce-103">teamsUserActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0fce-103">teamsUserActivityCounts resource type</span></span>

<span data-ttu-id="f0fce-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f0fce-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="f0fce-105">属性</span><span class="sxs-lookup"><span data-stu-id="f0fce-105">Properties</span></span>

| <span data-ttu-id="f0fce-106">属性</span><span class="sxs-lookup"><span data-stu-id="f0fce-106">Property</span></span>            | <span data-ttu-id="f0fce-107">类型</span><span class="sxs-lookup"><span data-stu-id="f0fce-107">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="f0fce-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f0fce-108">reportRefreshDate</span></span>   | <span data-ttu-id="f0fce-109">日期</span><span class="sxs-lookup"><span data-stu-id="f0fce-109">Date</span></span>   |
| <span data-ttu-id="f0fce-110">reportDate</span><span class="sxs-lookup"><span data-stu-id="f0fce-110">reportDate</span></span>          | <span data-ttu-id="f0fce-111">日期</span><span class="sxs-lookup"><span data-stu-id="f0fce-111">Date</span></span>   |
| <span data-ttu-id="f0fce-112">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="f0fce-112">teamChatMessages</span></span>    | <span data-ttu-id="f0fce-113">Int64</span><span class="sxs-lookup"><span data-stu-id="f0fce-113">Int64</span></span>  |
| <span data-ttu-id="f0fce-114">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="f0fce-114">privateChatMessages</span></span> | <span data-ttu-id="f0fce-115">Int64</span><span class="sxs-lookup"><span data-stu-id="f0fce-115">Int64</span></span>  |
| <span data-ttu-id="f0fce-116">calls</span><span class="sxs-lookup"><span data-stu-id="f0fce-116">calls</span></span>               | <span data-ttu-id="f0fce-117">Int64</span><span class="sxs-lookup"><span data-stu-id="f0fce-117">Int64</span></span>  |
| <span data-ttu-id="f0fce-118">会议</span><span class="sxs-lookup"><span data-stu-id="f0fce-118">meetings</span></span>            | <span data-ttu-id="f0fce-119">Int64</span><span class="sxs-lookup"><span data-stu-id="f0fce-119">Int64</span></span>  |
| <span data-ttu-id="f0fce-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f0fce-120">reportPeriod</span></span>        | <span data-ttu-id="f0fce-121">String</span><span class="sxs-lookup"><span data-stu-id="f0fce-121">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f0fce-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0fce-122">JSON representation</span></span>

<span data-ttu-id="f0fce-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0fce-123">The following is a JSON representation of the resource.</span></span>

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
