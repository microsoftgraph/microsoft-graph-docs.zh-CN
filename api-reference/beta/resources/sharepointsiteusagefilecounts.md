---
title: sharePointSiteUsageFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: ade81efa7494983a7f4b3c565c0ff4f7de532f67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042143"
---
# <a name="sharepointsiteusagefilecounts-resource-type"></a><span data-ttu-id="91f7d-103">sharePointSiteUsageFileCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="91f7d-103">sharePointSiteUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="91f7d-104">属性</span><span class="sxs-lookup"><span data-stu-id="91f7d-104">Properties</span></span>

| <span data-ttu-id="91f7d-105">属性</span><span class="sxs-lookup"><span data-stu-id="91f7d-105">Property</span></span>          | <span data-ttu-id="91f7d-106">类型</span><span class="sxs-lookup"><span data-stu-id="91f7d-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="91f7d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="91f7d-107">reportRefreshDate</span></span> | <span data-ttu-id="91f7d-108">日期</span><span class="sxs-lookup"><span data-stu-id="91f7d-108">Date</span></span>   |
| <span data-ttu-id="91f7d-109">键入一个文件夹</span><span class="sxs-lookup"><span data-stu-id="91f7d-109">siteType</span></span>          | <span data-ttu-id="91f7d-110">字符串</span><span class="sxs-lookup"><span data-stu-id="91f7d-110">String</span></span> |
| <span data-ttu-id="91f7d-111">total</span><span class="sxs-lookup"><span data-stu-id="91f7d-111">total</span></span>             | <span data-ttu-id="91f7d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="91f7d-112">Int64</span></span>  |
| <span data-ttu-id="91f7d-113">活动</span><span class="sxs-lookup"><span data-stu-id="91f7d-113">active</span></span>            | <span data-ttu-id="91f7d-114">Int64</span><span class="sxs-lookup"><span data-stu-id="91f7d-114">Int64</span></span>  |
| <span data-ttu-id="91f7d-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="91f7d-115">reportDate</span></span>        | <span data-ttu-id="91f7d-116">日期</span><span class="sxs-lookup"><span data-stu-id="91f7d-116">Date</span></span>   |
| <span data-ttu-id="91f7d-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="91f7d-117">reportPeriod</span></span>      | <span data-ttu-id="91f7d-118">String</span><span class="sxs-lookup"><span data-stu-id="91f7d-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="91f7d-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91f7d-119">JSON representation</span></span>

<span data-ttu-id="91f7d-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91f7d-120">The following is a JSON representation of the resource.</span></span>

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
