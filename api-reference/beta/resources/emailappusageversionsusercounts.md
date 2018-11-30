---
title: emailAppUsageVersionsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 7b4a59a1e15ddf41f0e4204efc4d3e0c6549e587
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046871"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="829c8-103">emailAppUsageVersionsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="829c8-103">emailAppUsageVersionsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="829c8-104">属性</span><span class="sxs-lookup"><span data-stu-id="829c8-104">Properties</span></span>

| <span data-ttu-id="829c8-105">属性</span><span class="sxs-lookup"><span data-stu-id="829c8-105">Property</span></span>          | <span data-ttu-id="829c8-106">类型</span><span class="sxs-lookup"><span data-stu-id="829c8-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="829c8-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="829c8-107">reportRefreshDate</span></span> | <span data-ttu-id="829c8-108">日期</span><span class="sxs-lookup"><span data-stu-id="829c8-108">Date</span></span>   |
| <span data-ttu-id="829c8-109">outlook2016</span><span class="sxs-lookup"><span data-stu-id="829c8-109">outlook2016</span></span>       | <span data-ttu-id="829c8-110">Int64</span><span class="sxs-lookup"><span data-stu-id="829c8-110">Int64</span></span>  |
| <span data-ttu-id="829c8-111">outlook2013</span><span class="sxs-lookup"><span data-stu-id="829c8-111">outlook2013</span></span>       | <span data-ttu-id="829c8-112">Int64</span><span class="sxs-lookup"><span data-stu-id="829c8-112">Int64</span></span>  |
| <span data-ttu-id="829c8-113">outlook2010</span><span class="sxs-lookup"><span data-stu-id="829c8-113">outlook2010</span></span>       | <span data-ttu-id="829c8-114">Int64</span><span class="sxs-lookup"><span data-stu-id="829c8-114">Int64</span></span>  |
| <span data-ttu-id="829c8-115">outlook2007</span><span class="sxs-lookup"><span data-stu-id="829c8-115">outlook2007</span></span>       | <span data-ttu-id="829c8-116">Int64</span><span class="sxs-lookup"><span data-stu-id="829c8-116">Int64</span></span>  |
| <span data-ttu-id="829c8-117">无法确定</span><span class="sxs-lookup"><span data-stu-id="829c8-117">undetermined</span></span>      | <span data-ttu-id="829c8-118">Int64</span><span class="sxs-lookup"><span data-stu-id="829c8-118">Int64</span></span>  |
| <span data-ttu-id="829c8-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="829c8-119">reportPeriod</span></span>      | <span data-ttu-id="829c8-120">String</span><span class="sxs-lookup"><span data-stu-id="829c8-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="829c8-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="829c8-121">JSON representation</span></span>

<span data-ttu-id="829c8-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="829c8-122">The following is a JSON representation of the resource.</span></span>

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
