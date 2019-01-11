---
title: sharePointActivityPages 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 758dcfd2e1c48b0bf8d0d85f06a68f26bfbbef99
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811842"
---
# <a name="sharepointactivitypages-resource-type"></a><span data-ttu-id="fe0c5-103">sharePointActivityPages 资源类型</span><span class="sxs-lookup"><span data-stu-id="fe0c5-103">sharePointActivityPages resource type</span></span>

## <a name="properties"></a><span data-ttu-id="fe0c5-104">属性</span><span class="sxs-lookup"><span data-stu-id="fe0c5-104">Properties</span></span>

| <span data-ttu-id="fe0c5-105">属性</span><span class="sxs-lookup"><span data-stu-id="fe0c5-105">Property</span></span>          | <span data-ttu-id="fe0c5-106">类型</span><span class="sxs-lookup"><span data-stu-id="fe0c5-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="fe0c5-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fe0c5-107">reportRefreshDate</span></span> | <span data-ttu-id="fe0c5-108">日期</span><span class="sxs-lookup"><span data-stu-id="fe0c5-108">Date</span></span>   |
| <span data-ttu-id="fe0c5-109">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="fe0c5-109">visitedPageCount</span></span>  | <span data-ttu-id="fe0c5-110">Int64</span><span class="sxs-lookup"><span data-stu-id="fe0c5-110">Int64</span></span>  |
| <span data-ttu-id="fe0c5-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="fe0c5-111">reportDate</span></span>        | <span data-ttu-id="fe0c5-112">日期</span><span class="sxs-lookup"><span data-stu-id="fe0c5-112">Date</span></span>   |
| <span data-ttu-id="fe0c5-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fe0c5-113">reportPeriod</span></span>      | <span data-ttu-id="fe0c5-114">String</span><span class="sxs-lookup"><span data-stu-id="fe0c5-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fe0c5-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fe0c5-115">JSON representation</span></span>

<span data-ttu-id="fe0c5-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe0c5-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityPages"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "visitedPageCount": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
