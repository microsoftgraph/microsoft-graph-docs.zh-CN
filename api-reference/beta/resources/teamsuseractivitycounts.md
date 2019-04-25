---
title: teamsUserActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcc0e9d1ed5c93c3d9f4ba97165d0413025a89cd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582918"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="a9da9-103">teamsUserActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9da9-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a9da9-104">属性</span><span class="sxs-lookup"><span data-stu-id="a9da9-104">Properties</span></span>

| <span data-ttu-id="a9da9-105">属性</span><span class="sxs-lookup"><span data-stu-id="a9da9-105">Property</span></span>            | <span data-ttu-id="a9da9-106">类型</span><span class="sxs-lookup"><span data-stu-id="a9da9-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="a9da9-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a9da9-107">reportRefreshDate</span></span>   | <span data-ttu-id="a9da9-108">Date</span><span class="sxs-lookup"><span data-stu-id="a9da9-108">Date</span></span>   |
| <span data-ttu-id="a9da9-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="a9da9-109">reportDate</span></span>          | <span data-ttu-id="a9da9-110">Date</span><span class="sxs-lookup"><span data-stu-id="a9da9-110">Date</span></span>   |
| <span data-ttu-id="a9da9-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="a9da9-111">teamChatMessages</span></span>    | <span data-ttu-id="a9da9-112">Int64</span><span class="sxs-lookup"><span data-stu-id="a9da9-112">Int64</span></span>  |
| <span data-ttu-id="a9da9-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="a9da9-113">privateChatMessages</span></span> | <span data-ttu-id="a9da9-114">Int64</span><span class="sxs-lookup"><span data-stu-id="a9da9-114">Int64</span></span>  |
| <span data-ttu-id="a9da9-115">calls</span><span class="sxs-lookup"><span data-stu-id="a9da9-115">calls</span></span>               | <span data-ttu-id="a9da9-116">Int64</span><span class="sxs-lookup"><span data-stu-id="a9da9-116">Int64</span></span>  |
| <span data-ttu-id="a9da9-117">会议</span><span class="sxs-lookup"><span data-stu-id="a9da9-117">meetings</span></span>            | <span data-ttu-id="a9da9-118">Int64</span><span class="sxs-lookup"><span data-stu-id="a9da9-118">Int64</span></span>  |
| <span data-ttu-id="a9da9-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a9da9-119">reportPeriod</span></span>        | <span data-ttu-id="a9da9-120">String</span><span class="sxs-lookup"><span data-stu-id="a9da9-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="a9da9-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9da9-121">JSON representation</span></span>

<span data-ttu-id="a9da9-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9da9-122">The following is a JSON representation of the resource.</span></span>

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
