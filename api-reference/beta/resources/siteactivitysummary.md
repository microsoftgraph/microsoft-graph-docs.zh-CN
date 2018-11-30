---
title: siteActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 354b329f592964249590b2f551d66681f45de485
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045210"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="d8286-103">siteActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8286-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d8286-104">属性</span><span class="sxs-lookup"><span data-stu-id="d8286-104">Properties</span></span>

| <span data-ttu-id="d8286-105">属性</span><span class="sxs-lookup"><span data-stu-id="d8286-105">Property</span></span>          | <span data-ttu-id="d8286-106">类型</span><span class="sxs-lookup"><span data-stu-id="d8286-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="d8286-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d8286-107">reportRefreshDate</span></span> | <span data-ttu-id="d8286-108">日期</span><span class="sxs-lookup"><span data-stu-id="d8286-108">Date</span></span>   |
| <span data-ttu-id="d8286-109">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="d8286-109">viewedOrEdited</span></span>    | <span data-ttu-id="d8286-110">Int64</span><span class="sxs-lookup"><span data-stu-id="d8286-110">Int64</span></span>  |
| <span data-ttu-id="d8286-111">同步</span><span class="sxs-lookup"><span data-stu-id="d8286-111">synced</span></span>            | <span data-ttu-id="d8286-112">Int64</span><span class="sxs-lookup"><span data-stu-id="d8286-112">Int64</span></span>  |
| <span data-ttu-id="d8286-113">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="d8286-113">sharedInternally</span></span>  | <span data-ttu-id="d8286-114">Int64</span><span class="sxs-lookup"><span data-stu-id="d8286-114">Int64</span></span>  |
| <span data-ttu-id="d8286-115">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="d8286-115">sharedExternally</span></span>  | <span data-ttu-id="d8286-116">Int64</span><span class="sxs-lookup"><span data-stu-id="d8286-116">Int64</span></span>  |
| <span data-ttu-id="d8286-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="d8286-117">reportDate</span></span>        | <span data-ttu-id="d8286-118">日期</span><span class="sxs-lookup"><span data-stu-id="d8286-118">Date</span></span>   |
| <span data-ttu-id="d8286-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d8286-119">reportPeriod</span></span>      | <span data-ttu-id="d8286-120">String</span><span class="sxs-lookup"><span data-stu-id="d8286-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d8286-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8286-121">JSON representation</span></span>

<span data-ttu-id="d8286-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8286-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "viewedOrEdited": 1024, 
  "synced": 1024, 
  "sharedInternally": 1024, 
  "sharedExternally": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
