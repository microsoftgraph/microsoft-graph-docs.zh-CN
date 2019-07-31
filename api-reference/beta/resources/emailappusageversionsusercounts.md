---
title: emailAppUsageVersionsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 18b86708071f1fab573571703dbb5bc253fcf2ce
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972136"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="b047a-103">emailAppUsageVersionsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="b047a-103">emailAppUsageVersionsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b047a-104">属性</span><span class="sxs-lookup"><span data-stu-id="b047a-104">Properties</span></span>

| <span data-ttu-id="b047a-105">属性</span><span class="sxs-lookup"><span data-stu-id="b047a-105">Property</span></span>          | <span data-ttu-id="b047a-106">类型</span><span class="sxs-lookup"><span data-stu-id="b047a-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="b047a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b047a-107">reportRefreshDate</span></span> | <span data-ttu-id="b047a-108">日期</span><span class="sxs-lookup"><span data-stu-id="b047a-108">Date</span></span>   |
| <span data-ttu-id="b047a-109">outlook2016</span><span class="sxs-lookup"><span data-stu-id="b047a-109">outlook2016</span></span>       | <span data-ttu-id="b047a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="b047a-110">Int64</span></span>  |
| <span data-ttu-id="b047a-111">outlook2013</span><span class="sxs-lookup"><span data-stu-id="b047a-111">outlook2013</span></span>       | <span data-ttu-id="b047a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b047a-112">Int64</span></span>  |
| <span data-ttu-id="b047a-113">outlook2010</span><span class="sxs-lookup"><span data-stu-id="b047a-113">outlook2010</span></span>       | <span data-ttu-id="b047a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="b047a-114">Int64</span></span>  |
| <span data-ttu-id="b047a-115">outlook2007</span><span class="sxs-lookup"><span data-stu-id="b047a-115">outlook2007</span></span>       | <span data-ttu-id="b047a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="b047a-116">Int64</span></span>  |
| <span data-ttu-id="b047a-117">流程</span><span class="sxs-lookup"><span data-stu-id="b047a-117">undetermined</span></span>      | <span data-ttu-id="b047a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="b047a-118">Int64</span></span>  |
| <span data-ttu-id="b047a-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b047a-119">reportPeriod</span></span>      | <span data-ttu-id="b047a-120">String</span><span class="sxs-lookup"><span data-stu-id="b047a-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b047a-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b047a-121">JSON representation</span></span>

<span data-ttu-id="b047a-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b047a-122">The following is a JSON representation of the resource.</span></span>

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
