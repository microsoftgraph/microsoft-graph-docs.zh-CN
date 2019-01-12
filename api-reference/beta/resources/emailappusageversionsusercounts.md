---
title: emailAppUsageVersionsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 371352c42e870f45224999b7a618d1bb694ea512
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965283"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="80b8a-103">emailAppUsageVersionsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="80b8a-103">emailAppUsageVersionsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="80b8a-104">属性</span><span class="sxs-lookup"><span data-stu-id="80b8a-104">Properties</span></span>

| <span data-ttu-id="80b8a-105">属性</span><span class="sxs-lookup"><span data-stu-id="80b8a-105">Property</span></span>          | <span data-ttu-id="80b8a-106">类型</span><span class="sxs-lookup"><span data-stu-id="80b8a-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="80b8a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="80b8a-107">reportRefreshDate</span></span> | <span data-ttu-id="80b8a-108">日期</span><span class="sxs-lookup"><span data-stu-id="80b8a-108">Date</span></span>   |
| <span data-ttu-id="80b8a-109">outlook2016</span><span class="sxs-lookup"><span data-stu-id="80b8a-109">outlook2016</span></span>       | <span data-ttu-id="80b8a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="80b8a-110">Int64</span></span>  |
| <span data-ttu-id="80b8a-111">outlook2013</span><span class="sxs-lookup"><span data-stu-id="80b8a-111">outlook2013</span></span>       | <span data-ttu-id="80b8a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="80b8a-112">Int64</span></span>  |
| <span data-ttu-id="80b8a-113">outlook2010</span><span class="sxs-lookup"><span data-stu-id="80b8a-113">outlook2010</span></span>       | <span data-ttu-id="80b8a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="80b8a-114">Int64</span></span>  |
| <span data-ttu-id="80b8a-115">outlook2007</span><span class="sxs-lookup"><span data-stu-id="80b8a-115">outlook2007</span></span>       | <span data-ttu-id="80b8a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="80b8a-116">Int64</span></span>  |
| <span data-ttu-id="80b8a-117">无法确定</span><span class="sxs-lookup"><span data-stu-id="80b8a-117">undetermined</span></span>      | <span data-ttu-id="80b8a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="80b8a-118">Int64</span></span>  |
| <span data-ttu-id="80b8a-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="80b8a-119">reportPeriod</span></span>      | <span data-ttu-id="80b8a-120">String</span><span class="sxs-lookup"><span data-stu-id="80b8a-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="80b8a-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80b8a-121">JSON representation</span></span>

<span data-ttu-id="80b8a-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80b8a-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "outlook2016": 1024, 
  "outlook2013": 1024, 
  "outlook2010": 1024, 
  "outlook2007": 1024, 
  "undetermined": 1024, 
  "reportPeriod": "String"
}
```
