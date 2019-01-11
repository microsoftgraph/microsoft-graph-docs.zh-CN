---
title: emailActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 82fbdc2621b9c8746ed3028fe44414edeb7e56db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871342"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="2468f-103">emailActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="2468f-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2468f-104">属性</span><span class="sxs-lookup"><span data-stu-id="2468f-104">Properties</span></span>

| <span data-ttu-id="2468f-105">属性</span><span class="sxs-lookup"><span data-stu-id="2468f-105">Property</span></span>          | <span data-ttu-id="2468f-106">类型</span><span class="sxs-lookup"><span data-stu-id="2468f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="2468f-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2468f-107">reportRefreshDate</span></span> | <span data-ttu-id="2468f-108">日期</span><span class="sxs-lookup"><span data-stu-id="2468f-108">Date</span></span>   |
| <span data-ttu-id="2468f-109">发送</span><span class="sxs-lookup"><span data-stu-id="2468f-109">send</span></span>              | <span data-ttu-id="2468f-110">Int64</span><span class="sxs-lookup"><span data-stu-id="2468f-110">Int64</span></span>  |
| <span data-ttu-id="2468f-111">接收</span><span class="sxs-lookup"><span data-stu-id="2468f-111">receive</span></span>           | <span data-ttu-id="2468f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2468f-112">Int64</span></span>  |
| <span data-ttu-id="2468f-113">读取</span><span class="sxs-lookup"><span data-stu-id="2468f-113">read</span></span>              | <span data-ttu-id="2468f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="2468f-114">Int64</span></span>  |
| <span data-ttu-id="2468f-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="2468f-115">reportDate</span></span>        | <span data-ttu-id="2468f-116">日期</span><span class="sxs-lookup"><span data-stu-id="2468f-116">Date</span></span>   |
| <span data-ttu-id="2468f-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2468f-117">reportPeriod</span></span>      | <span data-ttu-id="2468f-118">String</span><span class="sxs-lookup"><span data-stu-id="2468f-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2468f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2468f-119">JSON representation</span></span>

<span data-ttu-id="2468f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2468f-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "send": 1024, 
  "receive": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
