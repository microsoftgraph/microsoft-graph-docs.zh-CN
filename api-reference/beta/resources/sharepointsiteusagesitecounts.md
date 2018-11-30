---
title: sharePointSiteUsageSiteCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 631e01a417e177e356b701ca8dc93ffa51b4f50f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043114"
---
# <a name="sharepointsiteusagesitecounts-resource-type"></a><span data-ttu-id="d75c4-103">sharePointSiteUsageSiteCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="d75c4-103">sharePointSiteUsageSiteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d75c4-104">属性</span><span class="sxs-lookup"><span data-stu-id="d75c4-104">Properties</span></span>

| <span data-ttu-id="d75c4-105">属性</span><span class="sxs-lookup"><span data-stu-id="d75c4-105">Property</span></span>          | <span data-ttu-id="d75c4-106">类型</span><span class="sxs-lookup"><span data-stu-id="d75c4-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="d75c4-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d75c4-107">reportRefreshDate</span></span> | <span data-ttu-id="d75c4-108">日期</span><span class="sxs-lookup"><span data-stu-id="d75c4-108">Date</span></span>   |
| <span data-ttu-id="d75c4-109">键入一个文件夹</span><span class="sxs-lookup"><span data-stu-id="d75c4-109">siteType</span></span>          | <span data-ttu-id="d75c4-110">字符串</span><span class="sxs-lookup"><span data-stu-id="d75c4-110">String</span></span> |
| <span data-ttu-id="d75c4-111">total</span><span class="sxs-lookup"><span data-stu-id="d75c4-111">total</span></span>             | <span data-ttu-id="d75c4-112">Int64</span><span class="sxs-lookup"><span data-stu-id="d75c4-112">Int64</span></span>  |
| <span data-ttu-id="d75c4-113">活动</span><span class="sxs-lookup"><span data-stu-id="d75c4-113">active</span></span>            | <span data-ttu-id="d75c4-114">Int64</span><span class="sxs-lookup"><span data-stu-id="d75c4-114">Int64</span></span>  |
| <span data-ttu-id="d75c4-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="d75c4-115">reportDate</span></span>        | <span data-ttu-id="d75c4-116">日期</span><span class="sxs-lookup"><span data-stu-id="d75c4-116">Date</span></span>   |
| <span data-ttu-id="d75c4-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d75c4-117">reportPeriod</span></span>      | <span data-ttu-id="d75c4-118">String</span><span class="sxs-lookup"><span data-stu-id="d75c4-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d75c4-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d75c4-119">JSON representation</span></span>

<span data-ttu-id="d75c4-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d75c4-120">The following is a JSON representation of the resource.</span></span>

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
