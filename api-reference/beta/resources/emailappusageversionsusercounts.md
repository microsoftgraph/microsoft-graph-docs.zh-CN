---
title: emailAppUsageVersionsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 371352c42e870f45224999b7a618d1bb694ea512
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506676"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="22a68-103">emailAppUsageVersionsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="22a68-103">emailAppUsageVersionsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="22a68-104">属性</span><span class="sxs-lookup"><span data-stu-id="22a68-104">Properties</span></span>

| <span data-ttu-id="22a68-105">属性</span><span class="sxs-lookup"><span data-stu-id="22a68-105">Property</span></span>          | <span data-ttu-id="22a68-106">类型</span><span class="sxs-lookup"><span data-stu-id="22a68-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="22a68-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="22a68-107">reportRefreshDate</span></span> | <span data-ttu-id="22a68-108">Date</span><span class="sxs-lookup"><span data-stu-id="22a68-108">Date</span></span>   |
| <span data-ttu-id="22a68-109">outlook2016</span><span class="sxs-lookup"><span data-stu-id="22a68-109">outlook2016</span></span>       | <span data-ttu-id="22a68-110">Int64</span><span class="sxs-lookup"><span data-stu-id="22a68-110">Int64</span></span>  |
| <span data-ttu-id="22a68-111">outlook2013</span><span class="sxs-lookup"><span data-stu-id="22a68-111">outlook2013</span></span>       | <span data-ttu-id="22a68-112">Int64</span><span class="sxs-lookup"><span data-stu-id="22a68-112">Int64</span></span>  |
| <span data-ttu-id="22a68-113">outlook2010</span><span class="sxs-lookup"><span data-stu-id="22a68-113">outlook2010</span></span>       | <span data-ttu-id="22a68-114">Int64</span><span class="sxs-lookup"><span data-stu-id="22a68-114">Int64</span></span>  |
| <span data-ttu-id="22a68-115">outlook2007</span><span class="sxs-lookup"><span data-stu-id="22a68-115">outlook2007</span></span>       | <span data-ttu-id="22a68-116">Int64</span><span class="sxs-lookup"><span data-stu-id="22a68-116">Int64</span></span>  |
| <span data-ttu-id="22a68-117">流程</span><span class="sxs-lookup"><span data-stu-id="22a68-117">undetermined</span></span>      | <span data-ttu-id="22a68-118">Int64</span><span class="sxs-lookup"><span data-stu-id="22a68-118">Int64</span></span>  |
| <span data-ttu-id="22a68-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="22a68-119">reportPeriod</span></span>      | <span data-ttu-id="22a68-120">字符串</span><span class="sxs-lookup"><span data-stu-id="22a68-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="22a68-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22a68-121">JSON representation</span></span>

<span data-ttu-id="22a68-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22a68-122">The following is a JSON representation of the resource.</span></span>

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
