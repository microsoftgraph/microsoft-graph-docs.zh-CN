---
title: sharePointSiteUsagePages 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: c66a41393f1842a66c8e57c3d9ba77e6cf863cfa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041509"
---
# <a name="sharepointsiteusagepages-resource-type"></a><span data-ttu-id="9699f-103">sharePointSiteUsagePages 资源类型</span><span class="sxs-lookup"><span data-stu-id="9699f-103">sharePointSiteUsagePages resource type</span></span>

## <a name="properties"></a><span data-ttu-id="9699f-104">属性</span><span class="sxs-lookup"><span data-stu-id="9699f-104">Properties</span></span>

| <span data-ttu-id="9699f-105">属性</span><span class="sxs-lookup"><span data-stu-id="9699f-105">Property</span></span>          | <span data-ttu-id="9699f-106">类型</span><span class="sxs-lookup"><span data-stu-id="9699f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="9699f-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="9699f-107">reportRefreshDate</span></span> | <span data-ttu-id="9699f-108">日期</span><span class="sxs-lookup"><span data-stu-id="9699f-108">Date</span></span>   |
| <span data-ttu-id="9699f-109">键入一个文件夹</span><span class="sxs-lookup"><span data-stu-id="9699f-109">siteType</span></span>          | <span data-ttu-id="9699f-110">字符串</span><span class="sxs-lookup"><span data-stu-id="9699f-110">String</span></span> |
| <span data-ttu-id="9699f-111">pageViewCount</span><span class="sxs-lookup"><span data-stu-id="9699f-111">pageViewCount</span></span>     | <span data-ttu-id="9699f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="9699f-112">Int64</span></span>  |
| <span data-ttu-id="9699f-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="9699f-113">reportDate</span></span>        | <span data-ttu-id="9699f-114">日期</span><span class="sxs-lookup"><span data-stu-id="9699f-114">Date</span></span>   |
| <span data-ttu-id="9699f-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="9699f-115">reportPeriod</span></span>      | <span data-ttu-id="9699f-116">String</span><span class="sxs-lookup"><span data-stu-id="9699f-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9699f-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9699f-117">JSON representation</span></span>

<span data-ttu-id="9699f-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9699f-118">The following is a JSON representation of the resource.</span></span>

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
