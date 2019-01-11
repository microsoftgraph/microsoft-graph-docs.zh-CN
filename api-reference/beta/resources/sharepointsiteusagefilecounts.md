---
title: sharePointSiteUsageFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: b304a5bb519f8ffb2a23087b2ea38fd12fde6fab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836125"
---
# <a name="sharepointsiteusagefilecounts-resource-type"></a><span data-ttu-id="e57db-103">sharePointSiteUsageFileCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="e57db-103">sharePointSiteUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e57db-104">属性</span><span class="sxs-lookup"><span data-stu-id="e57db-104">Properties</span></span>

| <span data-ttu-id="e57db-105">属性</span><span class="sxs-lookup"><span data-stu-id="e57db-105">Property</span></span>          | <span data-ttu-id="e57db-106">类型</span><span class="sxs-lookup"><span data-stu-id="e57db-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="e57db-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e57db-107">reportRefreshDate</span></span> | <span data-ttu-id="e57db-108">日期</span><span class="sxs-lookup"><span data-stu-id="e57db-108">Date</span></span>   |
| <span data-ttu-id="e57db-109">键入一个文件夹</span><span class="sxs-lookup"><span data-stu-id="e57db-109">siteType</span></span>          | <span data-ttu-id="e57db-110">字符串</span><span class="sxs-lookup"><span data-stu-id="e57db-110">String</span></span> |
| <span data-ttu-id="e57db-111">total</span><span class="sxs-lookup"><span data-stu-id="e57db-111">total</span></span>             | <span data-ttu-id="e57db-112">Int64</span><span class="sxs-lookup"><span data-stu-id="e57db-112">Int64</span></span>  |
| <span data-ttu-id="e57db-113">活动</span><span class="sxs-lookup"><span data-stu-id="e57db-113">active</span></span>            | <span data-ttu-id="e57db-114">Int64</span><span class="sxs-lookup"><span data-stu-id="e57db-114">Int64</span></span>  |
| <span data-ttu-id="e57db-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="e57db-115">reportDate</span></span>        | <span data-ttu-id="e57db-116">日期</span><span class="sxs-lookup"><span data-stu-id="e57db-116">Date</span></span>   |
| <span data-ttu-id="e57db-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e57db-117">reportPeriod</span></span>      | <span data-ttu-id="e57db-118">String</span><span class="sxs-lookup"><span data-stu-id="e57db-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e57db-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e57db-119">JSON representation</span></span>

<span data-ttu-id="e57db-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e57db-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsageFileCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
