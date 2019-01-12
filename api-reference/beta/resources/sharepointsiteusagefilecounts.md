---
title: sharePointSiteUsageFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1c88cd75e1b38da87042b7b67388ef869c15ec38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950429"
---
# <a name="sharepointsiteusagefilecounts-resource-type"></a><span data-ttu-id="3b623-103">sharePointSiteUsageFileCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b623-103">sharePointSiteUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="3b623-104">属性</span><span class="sxs-lookup"><span data-stu-id="3b623-104">Properties</span></span>

| <span data-ttu-id="3b623-105">属性</span><span class="sxs-lookup"><span data-stu-id="3b623-105">Property</span></span>          | <span data-ttu-id="3b623-106">类型</span><span class="sxs-lookup"><span data-stu-id="3b623-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="3b623-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3b623-107">reportRefreshDate</span></span> | <span data-ttu-id="3b623-108">日期</span><span class="sxs-lookup"><span data-stu-id="3b623-108">Date</span></span>   |
| <span data-ttu-id="3b623-109">键入一个文件夹</span><span class="sxs-lookup"><span data-stu-id="3b623-109">siteType</span></span>          | <span data-ttu-id="3b623-110">字符串</span><span class="sxs-lookup"><span data-stu-id="3b623-110">String</span></span> |
| <span data-ttu-id="3b623-111">total</span><span class="sxs-lookup"><span data-stu-id="3b623-111">total</span></span>             | <span data-ttu-id="3b623-112">Int64</span><span class="sxs-lookup"><span data-stu-id="3b623-112">Int64</span></span>  |
| <span data-ttu-id="3b623-113">活动</span><span class="sxs-lookup"><span data-stu-id="3b623-113">active</span></span>            | <span data-ttu-id="3b623-114">Int64</span><span class="sxs-lookup"><span data-stu-id="3b623-114">Int64</span></span>  |
| <span data-ttu-id="3b623-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="3b623-115">reportDate</span></span>        | <span data-ttu-id="3b623-116">日期</span><span class="sxs-lookup"><span data-stu-id="3b623-116">Date</span></span>   |
| <span data-ttu-id="3b623-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3b623-117">reportPeriod</span></span>      | <span data-ttu-id="3b623-118">String</span><span class="sxs-lookup"><span data-stu-id="3b623-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3b623-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b623-119">JSON representation</span></span>

<span data-ttu-id="3b623-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b623-120">The following is a JSON representation of the resource.</span></span>

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
