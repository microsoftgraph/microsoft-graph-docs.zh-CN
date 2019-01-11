---
title: sharePointSiteUsagePages 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 625dc6ff15a7a9efb8a2b2b545fcc78a4e7e9407
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865637"
---
# <a name="sharepointsiteusagepages-resource-type"></a><span data-ttu-id="462d8-103">sharePointSiteUsagePages 资源类型</span><span class="sxs-lookup"><span data-stu-id="462d8-103">sharePointSiteUsagePages resource type</span></span>

## <a name="properties"></a><span data-ttu-id="462d8-104">属性</span><span class="sxs-lookup"><span data-stu-id="462d8-104">Properties</span></span>

| <span data-ttu-id="462d8-105">属性</span><span class="sxs-lookup"><span data-stu-id="462d8-105">Property</span></span>          | <span data-ttu-id="462d8-106">类型</span><span class="sxs-lookup"><span data-stu-id="462d8-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="462d8-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="462d8-107">reportRefreshDate</span></span> | <span data-ttu-id="462d8-108">日期</span><span class="sxs-lookup"><span data-stu-id="462d8-108">Date</span></span>   |
| <span data-ttu-id="462d8-109">键入一个文件夹</span><span class="sxs-lookup"><span data-stu-id="462d8-109">siteType</span></span>          | <span data-ttu-id="462d8-110">字符串</span><span class="sxs-lookup"><span data-stu-id="462d8-110">String</span></span> |
| <span data-ttu-id="462d8-111">pageViewCount</span><span class="sxs-lookup"><span data-stu-id="462d8-111">pageViewCount</span></span>     | <span data-ttu-id="462d8-112">Int64</span><span class="sxs-lookup"><span data-stu-id="462d8-112">Int64</span></span>  |
| <span data-ttu-id="462d8-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="462d8-113">reportDate</span></span>        | <span data-ttu-id="462d8-114">日期</span><span class="sxs-lookup"><span data-stu-id="462d8-114">Date</span></span>   |
| <span data-ttu-id="462d8-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="462d8-115">reportPeriod</span></span>      | <span data-ttu-id="462d8-116">String</span><span class="sxs-lookup"><span data-stu-id="462d8-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="462d8-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="462d8-117">JSON representation</span></span>

<span data-ttu-id="462d8-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="462d8-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsagePages"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "pageViewCount": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
