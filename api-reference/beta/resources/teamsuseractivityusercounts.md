---
title: teamsUserActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7a330223a7b72b32387998d458456f0661979ae2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519818"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="d8704-103">teamsUserActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8704-103">teamsUserActivityUserCounts resource type</span></span>

<span data-ttu-id="d8704-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d8704-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d8704-105">属性</span><span class="sxs-lookup"><span data-stu-id="d8704-105">Properties</span></span>

| <span data-ttu-id="d8704-106">属性</span><span class="sxs-lookup"><span data-stu-id="d8704-106">Property</span></span>            | <span data-ttu-id="d8704-107">类型</span><span class="sxs-lookup"><span data-stu-id="d8704-107">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="d8704-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d8704-108">reportRefreshDate</span></span>   | <span data-ttu-id="d8704-109">日期</span><span class="sxs-lookup"><span data-stu-id="d8704-109">Date</span></span>   |
| <span data-ttu-id="d8704-110">reportDate</span><span class="sxs-lookup"><span data-stu-id="d8704-110">reportDate</span></span>          | <span data-ttu-id="d8704-111">日期</span><span class="sxs-lookup"><span data-stu-id="d8704-111">Date</span></span>   |
| <span data-ttu-id="d8704-112">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="d8704-112">teamChatMessages</span></span>    | <span data-ttu-id="d8704-113">Int64</span><span class="sxs-lookup"><span data-stu-id="d8704-113">Int64</span></span>  |
| <span data-ttu-id="d8704-114">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="d8704-114">privateChatMessages</span></span> | <span data-ttu-id="d8704-115">Int64</span><span class="sxs-lookup"><span data-stu-id="d8704-115">Int64</span></span>  |
| <span data-ttu-id="d8704-116">calls</span><span class="sxs-lookup"><span data-stu-id="d8704-116">calls</span></span>               | <span data-ttu-id="d8704-117">Int64</span><span class="sxs-lookup"><span data-stu-id="d8704-117">Int64</span></span>  |
| <span data-ttu-id="d8704-118">会议</span><span class="sxs-lookup"><span data-stu-id="d8704-118">meetings</span></span>            | <span data-ttu-id="d8704-119">Int64</span><span class="sxs-lookup"><span data-stu-id="d8704-119">Int64</span></span>  |
| <span data-ttu-id="d8704-120">otherActions</span><span class="sxs-lookup"><span data-stu-id="d8704-120">otherActions</span></span>        | <span data-ttu-id="d8704-121">Int64</span><span class="sxs-lookup"><span data-stu-id="d8704-121">Int64</span></span>  |
| <span data-ttu-id="d8704-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d8704-122">reportPeriod</span></span>        | <span data-ttu-id="d8704-123">String</span><span class="sxs-lookup"><span data-stu-id="d8704-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d8704-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8704-124">JSON representation</span></span>

<span data-ttu-id="d8704-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8704-125">The following is a JSON representation of the resource.</span></span>

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
