---
title: skypeForBusinessActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: e59bd33b1709780bac9726ee716ef9d81ef33c1f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810127"
---
# <a name="skypeforbusinessactivitycounts-resource-type"></a><span data-ttu-id="b26c4-103">skypeForBusinessActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="b26c4-103">skypeForBusinessActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b26c4-104">属性</span><span class="sxs-lookup"><span data-stu-id="b26c4-104">Properties</span></span>

| <span data-ttu-id="b26c4-105">属性</span><span class="sxs-lookup"><span data-stu-id="b26c4-105">Property</span></span>          | <span data-ttu-id="b26c4-106">类型</span><span class="sxs-lookup"><span data-stu-id="b26c4-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="b26c4-107">peerToPeer</span><span class="sxs-lookup"><span data-stu-id="b26c4-107">peerToPeer</span></span>        | <span data-ttu-id="b26c4-108">Int64</span><span class="sxs-lookup"><span data-stu-id="b26c4-108">Int64</span></span>  |
| <span data-ttu-id="b26c4-109">组织</span><span class="sxs-lookup"><span data-stu-id="b26c4-109">organized</span></span>         | <span data-ttu-id="b26c4-110">Int64</span><span class="sxs-lookup"><span data-stu-id="b26c4-110">Int64</span></span>  |
| <span data-ttu-id="b26c4-111">则参与了会议</span><span class="sxs-lookup"><span data-stu-id="b26c4-111">participated</span></span>      | <span data-ttu-id="b26c4-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b26c4-112">Int64</span></span>  |
| <span data-ttu-id="b26c4-113">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b26c4-113">reportRefreshDate</span></span> | <span data-ttu-id="b26c4-114">日期</span><span class="sxs-lookup"><span data-stu-id="b26c4-114">Date</span></span>   |
| <span data-ttu-id="b26c4-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="b26c4-115">reportDate</span></span>        | <span data-ttu-id="b26c4-116">日期</span><span class="sxs-lookup"><span data-stu-id="b26c4-116">Date</span></span>   |
| <span data-ttu-id="b26c4-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b26c4-117">reportPeriod</span></span>      | <span data-ttu-id="b26c4-118">String</span><span class="sxs-lookup"><span data-stu-id="b26c4-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b26c4-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b26c4-119">JSON representation</span></span>

<span data-ttu-id="b26c4-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b26c4-120">The following is a JSON representation of the resource.</span></span>

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
