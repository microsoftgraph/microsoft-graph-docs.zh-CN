---
title: skypeForBusinessActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c4f97f8377ec5693be1cc477ab40119675a24908
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008199"
---
# <a name="skypeforbusinessactivitycounts-resource-type"></a><span data-ttu-id="840df-103">skypeForBusinessActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="840df-103">skypeForBusinessActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="840df-104">属性</span><span class="sxs-lookup"><span data-stu-id="840df-104">Properties</span></span>

| <span data-ttu-id="840df-105">属性</span><span class="sxs-lookup"><span data-stu-id="840df-105">Property</span></span>          | <span data-ttu-id="840df-106">类型</span><span class="sxs-lookup"><span data-stu-id="840df-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="840df-107">peerToPeer</span><span class="sxs-lookup"><span data-stu-id="840df-107">peerToPeer</span></span>        | <span data-ttu-id="840df-108">Int64</span><span class="sxs-lookup"><span data-stu-id="840df-108">Int64</span></span>  |
| <span data-ttu-id="840df-109">有条不紊</span><span class="sxs-lookup"><span data-stu-id="840df-109">organized</span></span>         | <span data-ttu-id="840df-110">Int64</span><span class="sxs-lookup"><span data-stu-id="840df-110">Int64</span></span>  |
| <span data-ttu-id="840df-111">参与</span><span class="sxs-lookup"><span data-stu-id="840df-111">participated</span></span>      | <span data-ttu-id="840df-112">Int64</span><span class="sxs-lookup"><span data-stu-id="840df-112">Int64</span></span>  |
| <span data-ttu-id="840df-113">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="840df-113">reportRefreshDate</span></span> | <span data-ttu-id="840df-114">日期</span><span class="sxs-lookup"><span data-stu-id="840df-114">Date</span></span>   |
| <span data-ttu-id="840df-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="840df-115">reportDate</span></span>        | <span data-ttu-id="840df-116">日期</span><span class="sxs-lookup"><span data-stu-id="840df-116">Date</span></span>   |
| <span data-ttu-id="840df-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="840df-117">reportPeriod</span></span>      | <span data-ttu-id="840df-118">String</span><span class="sxs-lookup"><span data-stu-id="840df-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="840df-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="840df-119">JSON representation</span></span>

<span data-ttu-id="840df-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="840df-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityCounts"
} -->

```json
{
  "peerToPeer": 1024, 
  "organized": 1024, 
  "participated": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
