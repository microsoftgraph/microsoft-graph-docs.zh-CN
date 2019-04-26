---
title: yammerGroupsActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 404dcd44baac005374634db097b79c10c86ae78f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551433"
---
# <a name="yammergroupsactivitycounts-resource-type"></a><span data-ttu-id="04df7-103">yammerGroupsActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="04df7-103">yammerGroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="04df7-104">属性</span><span class="sxs-lookup"><span data-stu-id="04df7-104">Properties</span></span>

| <span data-ttu-id="04df7-105">属性</span><span class="sxs-lookup"><span data-stu-id="04df7-105">Property</span></span>          | <span data-ttu-id="04df7-106">类型</span><span class="sxs-lookup"><span data-stu-id="04df7-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="04df7-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="04df7-107">reportRefreshDate</span></span> | <span data-ttu-id="04df7-108">Date</span><span class="sxs-lookup"><span data-stu-id="04df7-108">Date</span></span>   |
| <span data-ttu-id="04df7-109">人</span><span class="sxs-lookup"><span data-stu-id="04df7-109">liked</span></span>             | <span data-ttu-id="04df7-110">Int64</span><span class="sxs-lookup"><span data-stu-id="04df7-110">Int64</span></span>  |
| <span data-ttu-id="04df7-111">发布</span><span class="sxs-lookup"><span data-stu-id="04df7-111">posted</span></span>            | <span data-ttu-id="04df7-112">Int64</span><span class="sxs-lookup"><span data-stu-id="04df7-112">Int64</span></span>  |
| <span data-ttu-id="04df7-113">自述</span><span class="sxs-lookup"><span data-stu-id="04df7-113">read</span></span>              | <span data-ttu-id="04df7-114">Int64</span><span class="sxs-lookup"><span data-stu-id="04df7-114">Int64</span></span>  |
| <span data-ttu-id="04df7-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="04df7-115">reportDate</span></span>        | <span data-ttu-id="04df7-116">Date</span><span class="sxs-lookup"><span data-stu-id="04df7-116">Date</span></span>   |
| <span data-ttu-id="04df7-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="04df7-117">reportPeriod</span></span>      | <span data-ttu-id="04df7-118">String</span><span class="sxs-lookup"><span data-stu-id="04df7-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="04df7-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04df7-119">JSON representation</span></span>

<span data-ttu-id="04df7-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04df7-120">The following is a JSON representation of the resource.</span></span>

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
