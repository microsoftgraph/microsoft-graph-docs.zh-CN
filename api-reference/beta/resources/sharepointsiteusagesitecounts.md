---
title: sharePointSiteUsageSiteCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 913f9de5972d857b859b713298a0413d615b8991
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828124"
---
# <a name="sharepointsiteusagesitecounts-resource-type"></a><span data-ttu-id="88974-103">sharePointSiteUsageSiteCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="88974-103">sharePointSiteUsageSiteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="88974-104">属性</span><span class="sxs-lookup"><span data-stu-id="88974-104">Properties</span></span>

| <span data-ttu-id="88974-105">属性</span><span class="sxs-lookup"><span data-stu-id="88974-105">Property</span></span>          | <span data-ttu-id="88974-106">类型</span><span class="sxs-lookup"><span data-stu-id="88974-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="88974-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="88974-107">reportRefreshDate</span></span> | <span data-ttu-id="88974-108">日期</span><span class="sxs-lookup"><span data-stu-id="88974-108">Date</span></span>   |
| <span data-ttu-id="88974-109">键入一个文件夹</span><span class="sxs-lookup"><span data-stu-id="88974-109">siteType</span></span>          | <span data-ttu-id="88974-110">字符串</span><span class="sxs-lookup"><span data-stu-id="88974-110">String</span></span> |
| <span data-ttu-id="88974-111">total</span><span class="sxs-lookup"><span data-stu-id="88974-111">total</span></span>             | <span data-ttu-id="88974-112">Int64</span><span class="sxs-lookup"><span data-stu-id="88974-112">Int64</span></span>  |
| <span data-ttu-id="88974-113">活动</span><span class="sxs-lookup"><span data-stu-id="88974-113">active</span></span>            | <span data-ttu-id="88974-114">Int64</span><span class="sxs-lookup"><span data-stu-id="88974-114">Int64</span></span>  |
| <span data-ttu-id="88974-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="88974-115">reportDate</span></span>        | <span data-ttu-id="88974-116">日期</span><span class="sxs-lookup"><span data-stu-id="88974-116">Date</span></span>   |
| <span data-ttu-id="88974-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="88974-117">reportPeriod</span></span>      | <span data-ttu-id="88974-118">String</span><span class="sxs-lookup"><span data-stu-id="88974-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="88974-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88974-119">JSON representation</span></span>

<span data-ttu-id="88974-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88974-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsageSiteCounts"
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
