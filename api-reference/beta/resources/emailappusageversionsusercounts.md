---
title: emailAppUsageVersionsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: edc9242a99f0a993b2fa21c95259582bdf31c3da
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499412"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="aa06f-103">emailAppUsageVersionsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa06f-103">emailAppUsageVersionsUserCounts resource type</span></span>

<span data-ttu-id="aa06f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="aa06f-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="aa06f-105">属性</span><span class="sxs-lookup"><span data-stu-id="aa06f-105">Properties</span></span>

| <span data-ttu-id="aa06f-106">属性</span><span class="sxs-lookup"><span data-stu-id="aa06f-106">Property</span></span>          | <span data-ttu-id="aa06f-107">类型</span><span class="sxs-lookup"><span data-stu-id="aa06f-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="aa06f-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="aa06f-108">reportRefreshDate</span></span> | <span data-ttu-id="aa06f-109">日期</span><span class="sxs-lookup"><span data-stu-id="aa06f-109">Date</span></span>   |
| <span data-ttu-id="aa06f-110">outlook2016</span><span class="sxs-lookup"><span data-stu-id="aa06f-110">outlook2016</span></span>       | <span data-ttu-id="aa06f-111">Int64</span><span class="sxs-lookup"><span data-stu-id="aa06f-111">Int64</span></span>  |
| <span data-ttu-id="aa06f-112">outlook2013</span><span class="sxs-lookup"><span data-stu-id="aa06f-112">outlook2013</span></span>       | <span data-ttu-id="aa06f-113">Int64</span><span class="sxs-lookup"><span data-stu-id="aa06f-113">Int64</span></span>  |
| <span data-ttu-id="aa06f-114">outlook2010</span><span class="sxs-lookup"><span data-stu-id="aa06f-114">outlook2010</span></span>       | <span data-ttu-id="aa06f-115">Int64</span><span class="sxs-lookup"><span data-stu-id="aa06f-115">Int64</span></span>  |
| <span data-ttu-id="aa06f-116">outlook2007</span><span class="sxs-lookup"><span data-stu-id="aa06f-116">outlook2007</span></span>       | <span data-ttu-id="aa06f-117">Int64</span><span class="sxs-lookup"><span data-stu-id="aa06f-117">Int64</span></span>  |
| <span data-ttu-id="aa06f-118">流程</span><span class="sxs-lookup"><span data-stu-id="aa06f-118">undetermined</span></span>      | <span data-ttu-id="aa06f-119">Int64</span><span class="sxs-lookup"><span data-stu-id="aa06f-119">Int64</span></span>  |
| <span data-ttu-id="aa06f-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="aa06f-120">reportPeriod</span></span>      | <span data-ttu-id="aa06f-121">String</span><span class="sxs-lookup"><span data-stu-id="aa06f-121">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aa06f-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa06f-122">JSON representation</span></span>

<span data-ttu-id="aa06f-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa06f-123">The following is a JSON representation of the resource.</span></span>

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
