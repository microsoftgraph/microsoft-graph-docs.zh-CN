---
title: teamsUserActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3982b679802a2ca80eac5fe4e8f76fee91bbf1d3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046347"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="cb621-103">teamsUserActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="cb621-103">teamsUserActivityUserCounts resource type</span></span>

<span data-ttu-id="cb621-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb621-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="cb621-105">属性</span><span class="sxs-lookup"><span data-stu-id="cb621-105">Properties</span></span>

| <span data-ttu-id="cb621-106">属性</span><span class="sxs-lookup"><span data-stu-id="cb621-106">Property</span></span>            | <span data-ttu-id="cb621-107">类型</span><span class="sxs-lookup"><span data-stu-id="cb621-107">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="cb621-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="cb621-108">reportRefreshDate</span></span>   | <span data-ttu-id="cb621-109">日期</span><span class="sxs-lookup"><span data-stu-id="cb621-109">Date</span></span>   |
| <span data-ttu-id="cb621-110">reportDate</span><span class="sxs-lookup"><span data-stu-id="cb621-110">reportDate</span></span>          | <span data-ttu-id="cb621-111">日期</span><span class="sxs-lookup"><span data-stu-id="cb621-111">Date</span></span>   |
| <span data-ttu-id="cb621-112">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="cb621-112">teamChatMessages</span></span>    | <span data-ttu-id="cb621-113">Int64</span><span class="sxs-lookup"><span data-stu-id="cb621-113">Int64</span></span>  |
| <span data-ttu-id="cb621-114">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="cb621-114">privateChatMessages</span></span> | <span data-ttu-id="cb621-115">Int64</span><span class="sxs-lookup"><span data-stu-id="cb621-115">Int64</span></span>  |
| <span data-ttu-id="cb621-116">calls</span><span class="sxs-lookup"><span data-stu-id="cb621-116">calls</span></span>               | <span data-ttu-id="cb621-117">Int64</span><span class="sxs-lookup"><span data-stu-id="cb621-117">Int64</span></span>  |
| <span data-ttu-id="cb621-118">会议</span><span class="sxs-lookup"><span data-stu-id="cb621-118">meetings</span></span>            | <span data-ttu-id="cb621-119">Int64</span><span class="sxs-lookup"><span data-stu-id="cb621-119">Int64</span></span>  |
| <span data-ttu-id="cb621-120">otherActions</span><span class="sxs-lookup"><span data-stu-id="cb621-120">otherActions</span></span>        | <span data-ttu-id="cb621-121">Int64</span><span class="sxs-lookup"><span data-stu-id="cb621-121">Int64</span></span>  |
| <span data-ttu-id="cb621-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="cb621-122">reportPeriod</span></span>        | <span data-ttu-id="cb621-123">String</span><span class="sxs-lookup"><span data-stu-id="cb621-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cb621-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cb621-124">JSON representation</span></span>

<span data-ttu-id="cb621-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb621-125">The following is a JSON representation of the resource.</span></span>

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


