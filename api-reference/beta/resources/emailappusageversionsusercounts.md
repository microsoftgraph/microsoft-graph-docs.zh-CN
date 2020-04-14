---
title: emailAppUsageVersionsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c7fec61c71b9a5343470eec87fa59d65f59020f8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440531"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="94812-103">emailAppUsageVersionsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="94812-103">emailAppUsageVersionsUserCounts resource type</span></span>

<span data-ttu-id="94812-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94812-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="94812-105">属性</span><span class="sxs-lookup"><span data-stu-id="94812-105">Properties</span></span>

| <span data-ttu-id="94812-106">属性</span><span class="sxs-lookup"><span data-stu-id="94812-106">Property</span></span>          | <span data-ttu-id="94812-107">类型</span><span class="sxs-lookup"><span data-stu-id="94812-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="94812-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="94812-108">reportRefreshDate</span></span> | <span data-ttu-id="94812-109">日期</span><span class="sxs-lookup"><span data-stu-id="94812-109">Date</span></span>   |
| <span data-ttu-id="94812-110">outlook2016</span><span class="sxs-lookup"><span data-stu-id="94812-110">outlook2016</span></span>       | <span data-ttu-id="94812-111">Int64</span><span class="sxs-lookup"><span data-stu-id="94812-111">Int64</span></span>  |
| <span data-ttu-id="94812-112">outlook2013</span><span class="sxs-lookup"><span data-stu-id="94812-112">outlook2013</span></span>       | <span data-ttu-id="94812-113">Int64</span><span class="sxs-lookup"><span data-stu-id="94812-113">Int64</span></span>  |
| <span data-ttu-id="94812-114">outlook2010</span><span class="sxs-lookup"><span data-stu-id="94812-114">outlook2010</span></span>       | <span data-ttu-id="94812-115">Int64</span><span class="sxs-lookup"><span data-stu-id="94812-115">Int64</span></span>  |
| <span data-ttu-id="94812-116">outlook2007</span><span class="sxs-lookup"><span data-stu-id="94812-116">outlook2007</span></span>       | <span data-ttu-id="94812-117">Int64</span><span class="sxs-lookup"><span data-stu-id="94812-117">Int64</span></span>  |
| <span data-ttu-id="94812-118">流程</span><span class="sxs-lookup"><span data-stu-id="94812-118">undetermined</span></span>      | <span data-ttu-id="94812-119">Int64</span><span class="sxs-lookup"><span data-stu-id="94812-119">Int64</span></span>  |
| <span data-ttu-id="94812-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="94812-120">reportPeriod</span></span>      | <span data-ttu-id="94812-121">String</span><span class="sxs-lookup"><span data-stu-id="94812-121">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="94812-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94812-122">JSON representation</span></span>

<span data-ttu-id="94812-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94812-123">The following is a JSON representation of the resource.</span></span>

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
