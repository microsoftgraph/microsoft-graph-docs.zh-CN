---
title: siteActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 2eb5bdb89924338d1d352ea80bd516b8fb948250
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817764"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="7cd16-103">siteActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="7cd16-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7cd16-104">属性</span><span class="sxs-lookup"><span data-stu-id="7cd16-104">Properties</span></span>

| <span data-ttu-id="7cd16-105">属性</span><span class="sxs-lookup"><span data-stu-id="7cd16-105">Property</span></span>          | <span data-ttu-id="7cd16-106">类型</span><span class="sxs-lookup"><span data-stu-id="7cd16-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="7cd16-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7cd16-107">reportRefreshDate</span></span> | <span data-ttu-id="7cd16-108">日期</span><span class="sxs-lookup"><span data-stu-id="7cd16-108">Date</span></span>   |
| <span data-ttu-id="7cd16-109">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="7cd16-109">viewedOrEdited</span></span>    | <span data-ttu-id="7cd16-110">Int64</span><span class="sxs-lookup"><span data-stu-id="7cd16-110">Int64</span></span>  |
| <span data-ttu-id="7cd16-111">同步</span><span class="sxs-lookup"><span data-stu-id="7cd16-111">synced</span></span>            | <span data-ttu-id="7cd16-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7cd16-112">Int64</span></span>  |
| <span data-ttu-id="7cd16-113">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="7cd16-113">sharedInternally</span></span>  | <span data-ttu-id="7cd16-114">Int64</span><span class="sxs-lookup"><span data-stu-id="7cd16-114">Int64</span></span>  |
| <span data-ttu-id="7cd16-115">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="7cd16-115">sharedExternally</span></span>  | <span data-ttu-id="7cd16-116">Int64</span><span class="sxs-lookup"><span data-stu-id="7cd16-116">Int64</span></span>  |
| <span data-ttu-id="7cd16-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="7cd16-117">reportDate</span></span>        | <span data-ttu-id="7cd16-118">日期</span><span class="sxs-lookup"><span data-stu-id="7cd16-118">Date</span></span>   |
| <span data-ttu-id="7cd16-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7cd16-119">reportPeriod</span></span>      | <span data-ttu-id="7cd16-120">String</span><span class="sxs-lookup"><span data-stu-id="7cd16-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7cd16-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7cd16-121">JSON representation</span></span>

<span data-ttu-id="7cd16-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7cd16-122">The following is a JSON representation of the resource.</span></span>

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
