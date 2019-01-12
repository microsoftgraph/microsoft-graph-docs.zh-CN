---
title: sharePointActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9656b39572eac5b6474dd7884eb7d1d2edb17310
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984722"
---
# <a name="sharepointactivityusercounts-resource-type"></a><span data-ttu-id="7c836-103">sharePointActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c836-103">sharePointActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7c836-104">属性</span><span class="sxs-lookup"><span data-stu-id="7c836-104">Properties</span></span>

| <span data-ttu-id="7c836-105">属性</span><span class="sxs-lookup"><span data-stu-id="7c836-105">Property</span></span>          | <span data-ttu-id="7c836-106">类型</span><span class="sxs-lookup"><span data-stu-id="7c836-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="7c836-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7c836-107">reportRefreshDate</span></span> | <span data-ttu-id="7c836-108">日期</span><span class="sxs-lookup"><span data-stu-id="7c836-108">Date</span></span>   |
| <span data-ttu-id="7c836-109">visitedPage</span><span class="sxs-lookup"><span data-stu-id="7c836-109">visitedPage</span></span>       | <span data-ttu-id="7c836-110">Int64</span><span class="sxs-lookup"><span data-stu-id="7c836-110">Int64</span></span>  |
| <span data-ttu-id="7c836-111">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="7c836-111">viewedOrEdited</span></span>    | <span data-ttu-id="7c836-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7c836-112">Int64</span></span>  |
| <span data-ttu-id="7c836-113">同步</span><span class="sxs-lookup"><span data-stu-id="7c836-113">synced</span></span>            | <span data-ttu-id="7c836-114">Int64</span><span class="sxs-lookup"><span data-stu-id="7c836-114">Int64</span></span>  |
| <span data-ttu-id="7c836-115">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="7c836-115">sharedInternally</span></span>  | <span data-ttu-id="7c836-116">Int64</span><span class="sxs-lookup"><span data-stu-id="7c836-116">Int64</span></span>  |
| <span data-ttu-id="7c836-117">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="7c836-117">sharedExternally</span></span>  | <span data-ttu-id="7c836-118">Int64</span><span class="sxs-lookup"><span data-stu-id="7c836-118">Int64</span></span>  |
| <span data-ttu-id="7c836-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="7c836-119">reportDate</span></span>        | <span data-ttu-id="7c836-120">日期</span><span class="sxs-lookup"><span data-stu-id="7c836-120">Date</span></span>   |
| <span data-ttu-id="7c836-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7c836-121">reportPeriod</span></span>      | <span data-ttu-id="7c836-122">String</span><span class="sxs-lookup"><span data-stu-id="7c836-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7c836-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c836-123">JSON representation</span></span>

<span data-ttu-id="7c836-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c836-124">The following is a JSON representation of the resource.</span></span>

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
