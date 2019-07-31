---
title: sharePointActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 97fbcb8c611bd497a7bf6613a5bde53738aff5e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008451"
---
# <a name="sharepointactivityusercounts-resource-type"></a><span data-ttu-id="744a0-103">sharePointActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="744a0-103">sharePointActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="744a0-104">属性</span><span class="sxs-lookup"><span data-stu-id="744a0-104">Properties</span></span>

| <span data-ttu-id="744a0-105">属性</span><span class="sxs-lookup"><span data-stu-id="744a0-105">Property</span></span>          | <span data-ttu-id="744a0-106">类型</span><span class="sxs-lookup"><span data-stu-id="744a0-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="744a0-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="744a0-107">reportRefreshDate</span></span> | <span data-ttu-id="744a0-108">日期</span><span class="sxs-lookup"><span data-stu-id="744a0-108">Date</span></span>   |
| <span data-ttu-id="744a0-109">visitedPage</span><span class="sxs-lookup"><span data-stu-id="744a0-109">visitedPage</span></span>       | <span data-ttu-id="744a0-110">Int64</span><span class="sxs-lookup"><span data-stu-id="744a0-110">Int64</span></span>  |
| <span data-ttu-id="744a0-111">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="744a0-111">viewedOrEdited</span></span>    | <span data-ttu-id="744a0-112">Int64</span><span class="sxs-lookup"><span data-stu-id="744a0-112">Int64</span></span>  |
| <span data-ttu-id="744a0-113">保持</span><span class="sxs-lookup"><span data-stu-id="744a0-113">synced</span></span>            | <span data-ttu-id="744a0-114">Int64</span><span class="sxs-lookup"><span data-stu-id="744a0-114">Int64</span></span>  |
| <span data-ttu-id="744a0-115">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="744a0-115">sharedInternally</span></span>  | <span data-ttu-id="744a0-116">Int64</span><span class="sxs-lookup"><span data-stu-id="744a0-116">Int64</span></span>  |
| <span data-ttu-id="744a0-117">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="744a0-117">sharedExternally</span></span>  | <span data-ttu-id="744a0-118">Int64</span><span class="sxs-lookup"><span data-stu-id="744a0-118">Int64</span></span>  |
| <span data-ttu-id="744a0-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="744a0-119">reportDate</span></span>        | <span data-ttu-id="744a0-120">日期</span><span class="sxs-lookup"><span data-stu-id="744a0-120">Date</span></span>   |
| <span data-ttu-id="744a0-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="744a0-121">reportPeriod</span></span>      | <span data-ttu-id="744a0-122">String</span><span class="sxs-lookup"><span data-stu-id="744a0-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="744a0-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="744a0-123">JSON representation</span></span>

<span data-ttu-id="744a0-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="744a0-124">The following is a JSON representation of the resource.</span></span>

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
