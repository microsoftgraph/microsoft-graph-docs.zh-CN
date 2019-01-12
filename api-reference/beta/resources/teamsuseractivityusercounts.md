---
title: teamsUserActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcb69c09d621ce3cce006fd9130afa0a70e4cdb8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912818"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="356be-103">teamsUserActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="356be-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="356be-104">属性</span><span class="sxs-lookup"><span data-stu-id="356be-104">Properties</span></span>

| <span data-ttu-id="356be-105">属性</span><span class="sxs-lookup"><span data-stu-id="356be-105">Property</span></span>            | <span data-ttu-id="356be-106">类型</span><span class="sxs-lookup"><span data-stu-id="356be-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="356be-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="356be-107">reportRefreshDate</span></span>   | <span data-ttu-id="356be-108">日期</span><span class="sxs-lookup"><span data-stu-id="356be-108">Date</span></span>   |
| <span data-ttu-id="356be-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="356be-109">reportDate</span></span>          | <span data-ttu-id="356be-110">日期</span><span class="sxs-lookup"><span data-stu-id="356be-110">Date</span></span>   |
| <span data-ttu-id="356be-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="356be-111">teamChatMessages</span></span>    | <span data-ttu-id="356be-112">Int64</span><span class="sxs-lookup"><span data-stu-id="356be-112">Int64</span></span>  |
| <span data-ttu-id="356be-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="356be-113">privateChatMessages</span></span> | <span data-ttu-id="356be-114">Int64</span><span class="sxs-lookup"><span data-stu-id="356be-114">Int64</span></span>  |
| <span data-ttu-id="356be-115">呼叫</span><span class="sxs-lookup"><span data-stu-id="356be-115">calls</span></span>               | <span data-ttu-id="356be-116">Int64</span><span class="sxs-lookup"><span data-stu-id="356be-116">Int64</span></span>  |
| <span data-ttu-id="356be-117">会议</span><span class="sxs-lookup"><span data-stu-id="356be-117">meetings</span></span>            | <span data-ttu-id="356be-118">Int64</span><span class="sxs-lookup"><span data-stu-id="356be-118">Int64</span></span>  |
| <span data-ttu-id="356be-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="356be-119">otherActions</span></span>        | <span data-ttu-id="356be-120">Int64</span><span class="sxs-lookup"><span data-stu-id="356be-120">Int64</span></span>  |
| <span data-ttu-id="356be-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="356be-121">reportPeriod</span></span>        | <span data-ttu-id="356be-122">String</span><span class="sxs-lookup"><span data-stu-id="356be-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="356be-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="356be-123">JSON representation</span></span>

<span data-ttu-id="356be-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="356be-124">The following is a JSON representation of the resource.</span></span>

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
