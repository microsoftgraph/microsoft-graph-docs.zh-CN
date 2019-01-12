---
title: sharePointSiteUsageSiteCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d261bb6db255f9e901c7f86d0767b8dcf0121aba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970330"
---
# <a name="sharepointsiteusagesitecounts-resource-type"></a><span data-ttu-id="5daf6-103">sharePointSiteUsageSiteCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="5daf6-103">sharePointSiteUsageSiteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5daf6-104">属性</span><span class="sxs-lookup"><span data-stu-id="5daf6-104">Properties</span></span>

| <span data-ttu-id="5daf6-105">属性</span><span class="sxs-lookup"><span data-stu-id="5daf6-105">Property</span></span>          | <span data-ttu-id="5daf6-106">类型</span><span class="sxs-lookup"><span data-stu-id="5daf6-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5daf6-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5daf6-107">reportRefreshDate</span></span> | <span data-ttu-id="5daf6-108">日期</span><span class="sxs-lookup"><span data-stu-id="5daf6-108">Date</span></span>   |
| <span data-ttu-id="5daf6-109">键入一个文件夹</span><span class="sxs-lookup"><span data-stu-id="5daf6-109">siteType</span></span>          | <span data-ttu-id="5daf6-110">字符串</span><span class="sxs-lookup"><span data-stu-id="5daf6-110">String</span></span> |
| <span data-ttu-id="5daf6-111">total</span><span class="sxs-lookup"><span data-stu-id="5daf6-111">total</span></span>             | <span data-ttu-id="5daf6-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5daf6-112">Int64</span></span>  |
| <span data-ttu-id="5daf6-113">活动</span><span class="sxs-lookup"><span data-stu-id="5daf6-113">active</span></span>            | <span data-ttu-id="5daf6-114">Int64</span><span class="sxs-lookup"><span data-stu-id="5daf6-114">Int64</span></span>  |
| <span data-ttu-id="5daf6-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="5daf6-115">reportDate</span></span>        | <span data-ttu-id="5daf6-116">日期</span><span class="sxs-lookup"><span data-stu-id="5daf6-116">Date</span></span>   |
| <span data-ttu-id="5daf6-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5daf6-117">reportPeriod</span></span>      | <span data-ttu-id="5daf6-118">String</span><span class="sxs-lookup"><span data-stu-id="5daf6-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5daf6-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5daf6-119">JSON representation</span></span>

<span data-ttu-id="5daf6-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5daf6-120">The following is a JSON representation of the resource.</span></span>

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
