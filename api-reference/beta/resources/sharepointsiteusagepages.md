---
title: sharePointSiteUsagePages 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1a82c0a1174559db6d90e64f1fd1ed1403caa048
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950443"
---
# <a name="sharepointsiteusagepages-resource-type"></a><span data-ttu-id="dd668-103">sharePointSiteUsagePages 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd668-103">sharePointSiteUsagePages resource type</span></span>

## <a name="properties"></a><span data-ttu-id="dd668-104">属性</span><span class="sxs-lookup"><span data-stu-id="dd668-104">Properties</span></span>

| <span data-ttu-id="dd668-105">属性</span><span class="sxs-lookup"><span data-stu-id="dd668-105">Property</span></span>          | <span data-ttu-id="dd668-106">类型</span><span class="sxs-lookup"><span data-stu-id="dd668-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="dd668-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="dd668-107">reportRefreshDate</span></span> | <span data-ttu-id="dd668-108">日期</span><span class="sxs-lookup"><span data-stu-id="dd668-108">Date</span></span>   |
| <span data-ttu-id="dd668-109">键入一个文件夹</span><span class="sxs-lookup"><span data-stu-id="dd668-109">siteType</span></span>          | <span data-ttu-id="dd668-110">字符串</span><span class="sxs-lookup"><span data-stu-id="dd668-110">String</span></span> |
| <span data-ttu-id="dd668-111">pageViewCount</span><span class="sxs-lookup"><span data-stu-id="dd668-111">pageViewCount</span></span>     | <span data-ttu-id="dd668-112">Int64</span><span class="sxs-lookup"><span data-stu-id="dd668-112">Int64</span></span>  |
| <span data-ttu-id="dd668-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="dd668-113">reportDate</span></span>        | <span data-ttu-id="dd668-114">日期</span><span class="sxs-lookup"><span data-stu-id="dd668-114">Date</span></span>   |
| <span data-ttu-id="dd668-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="dd668-115">reportPeriod</span></span>      | <span data-ttu-id="dd668-116">String</span><span class="sxs-lookup"><span data-stu-id="dd668-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dd668-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd668-117">JSON representation</span></span>

<span data-ttu-id="dd668-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd668-118">The following is a JSON representation of the resource.</span></span>

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
