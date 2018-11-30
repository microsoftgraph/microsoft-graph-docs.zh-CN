---
title: sharePointActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 271ea6a70d56c55cf5a9561c2a1485c674a365f1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044774"
---
# <a name="sharepointactivityusercounts-resource-type"></a><span data-ttu-id="2b192-103">sharePointActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b192-103">sharePointActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2b192-104">属性</span><span class="sxs-lookup"><span data-stu-id="2b192-104">Properties</span></span>

| <span data-ttu-id="2b192-105">属性</span><span class="sxs-lookup"><span data-stu-id="2b192-105">Property</span></span>          | <span data-ttu-id="2b192-106">类型</span><span class="sxs-lookup"><span data-stu-id="2b192-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="2b192-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2b192-107">reportRefreshDate</span></span> | <span data-ttu-id="2b192-108">日期</span><span class="sxs-lookup"><span data-stu-id="2b192-108">Date</span></span>   |
| <span data-ttu-id="2b192-109">visitedPage</span><span class="sxs-lookup"><span data-stu-id="2b192-109">visitedPage</span></span>       | <span data-ttu-id="2b192-110">Int64</span><span class="sxs-lookup"><span data-stu-id="2b192-110">Int64</span></span>  |
| <span data-ttu-id="2b192-111">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="2b192-111">viewedOrEdited</span></span>    | <span data-ttu-id="2b192-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2b192-112">Int64</span></span>  |
| <span data-ttu-id="2b192-113">同步</span><span class="sxs-lookup"><span data-stu-id="2b192-113">synced</span></span>            | <span data-ttu-id="2b192-114">Int64</span><span class="sxs-lookup"><span data-stu-id="2b192-114">Int64</span></span>  |
| <span data-ttu-id="2b192-115">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="2b192-115">sharedInternally</span></span>  | <span data-ttu-id="2b192-116">Int64</span><span class="sxs-lookup"><span data-stu-id="2b192-116">Int64</span></span>  |
| <span data-ttu-id="2b192-117">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="2b192-117">sharedExternally</span></span>  | <span data-ttu-id="2b192-118">Int64</span><span class="sxs-lookup"><span data-stu-id="2b192-118">Int64</span></span>  |
| <span data-ttu-id="2b192-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="2b192-119">reportDate</span></span>        | <span data-ttu-id="2b192-120">日期</span><span class="sxs-lookup"><span data-stu-id="2b192-120">Date</span></span>   |
| <span data-ttu-id="2b192-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2b192-121">reportPeriod</span></span>      | <span data-ttu-id="2b192-122">String</span><span class="sxs-lookup"><span data-stu-id="2b192-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2b192-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b192-123">JSON representation</span></span>

<span data-ttu-id="2b192-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b192-124">The following is a JSON representation of the resource.</span></span>

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
