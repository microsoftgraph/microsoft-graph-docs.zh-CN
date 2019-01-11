---
title: sharePointActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: ffbbb8c4d33c94678e8d57d1d9e69da91b22fb39
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819929"
---
# <a name="sharepointactivityusercounts-resource-type"></a><span data-ttu-id="11161-103">sharePointActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="11161-103">sharePointActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="11161-104">属性</span><span class="sxs-lookup"><span data-stu-id="11161-104">Properties</span></span>

| <span data-ttu-id="11161-105">属性</span><span class="sxs-lookup"><span data-stu-id="11161-105">Property</span></span>          | <span data-ttu-id="11161-106">类型</span><span class="sxs-lookup"><span data-stu-id="11161-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="11161-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="11161-107">reportRefreshDate</span></span> | <span data-ttu-id="11161-108">日期</span><span class="sxs-lookup"><span data-stu-id="11161-108">Date</span></span>   |
| <span data-ttu-id="11161-109">visitedPage</span><span class="sxs-lookup"><span data-stu-id="11161-109">visitedPage</span></span>       | <span data-ttu-id="11161-110">Int64</span><span class="sxs-lookup"><span data-stu-id="11161-110">Int64</span></span>  |
| <span data-ttu-id="11161-111">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="11161-111">viewedOrEdited</span></span>    | <span data-ttu-id="11161-112">Int64</span><span class="sxs-lookup"><span data-stu-id="11161-112">Int64</span></span>  |
| <span data-ttu-id="11161-113">同步</span><span class="sxs-lookup"><span data-stu-id="11161-113">synced</span></span>            | <span data-ttu-id="11161-114">Int64</span><span class="sxs-lookup"><span data-stu-id="11161-114">Int64</span></span>  |
| <span data-ttu-id="11161-115">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="11161-115">sharedInternally</span></span>  | <span data-ttu-id="11161-116">Int64</span><span class="sxs-lookup"><span data-stu-id="11161-116">Int64</span></span>  |
| <span data-ttu-id="11161-117">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="11161-117">sharedExternally</span></span>  | <span data-ttu-id="11161-118">Int64</span><span class="sxs-lookup"><span data-stu-id="11161-118">Int64</span></span>  |
| <span data-ttu-id="11161-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="11161-119">reportDate</span></span>        | <span data-ttu-id="11161-120">日期</span><span class="sxs-lookup"><span data-stu-id="11161-120">Date</span></span>   |
| <span data-ttu-id="11161-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="11161-121">reportPeriod</span></span>      | <span data-ttu-id="11161-122">String</span><span class="sxs-lookup"><span data-stu-id="11161-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="11161-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11161-123">JSON representation</span></span>

<span data-ttu-id="11161-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11161-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "visitedPage": 1024, 
  "viewedOrEdited": 1024, 
  "synced": 1024, 
  "sharedInternally": 1024, 
  "sharedExternally": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
