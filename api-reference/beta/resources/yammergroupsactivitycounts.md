---
title: yammerGroupsActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 828997f6bc89d23d63ab997418f6b3e8d48d1f83
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046060"
---
# <a name="yammergroupsactivitycounts-resource-type"></a><span data-ttu-id="192de-103">yammerGroupsActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="192de-103">yammerGroupsActivityCounts resource type</span></span>

<span data-ttu-id="192de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="192de-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="192de-105">属性</span><span class="sxs-lookup"><span data-stu-id="192de-105">Properties</span></span>

| <span data-ttu-id="192de-106">属性</span><span class="sxs-lookup"><span data-stu-id="192de-106">Property</span></span>          | <span data-ttu-id="192de-107">类型</span><span class="sxs-lookup"><span data-stu-id="192de-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="192de-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="192de-108">reportRefreshDate</span></span> | <span data-ttu-id="192de-109">日期</span><span class="sxs-lookup"><span data-stu-id="192de-109">Date</span></span>   |
| <span data-ttu-id="192de-110">人</span><span class="sxs-lookup"><span data-stu-id="192de-110">liked</span></span>             | <span data-ttu-id="192de-111">Int64</span><span class="sxs-lookup"><span data-stu-id="192de-111">Int64</span></span>  |
| <span data-ttu-id="192de-112">发布</span><span class="sxs-lookup"><span data-stu-id="192de-112">posted</span></span>            | <span data-ttu-id="192de-113">Int64</span><span class="sxs-lookup"><span data-stu-id="192de-113">Int64</span></span>  |
| <span data-ttu-id="192de-114">阅读</span><span class="sxs-lookup"><span data-stu-id="192de-114">read</span></span>              | <span data-ttu-id="192de-115">Int64</span><span class="sxs-lookup"><span data-stu-id="192de-115">Int64</span></span>  |
| <span data-ttu-id="192de-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="192de-116">reportDate</span></span>        | <span data-ttu-id="192de-117">日期</span><span class="sxs-lookup"><span data-stu-id="192de-117">Date</span></span>   |
| <span data-ttu-id="192de-118">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="192de-118">reportPeriod</span></span>      | <span data-ttu-id="192de-119">String</span><span class="sxs-lookup"><span data-stu-id="192de-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="192de-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="192de-120">JSON representation</span></span>

<span data-ttu-id="192de-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="192de-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "liked": 1024, 
  "posted": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


