---
title: sharePointSiteUsageSiteCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d261bb6db255f9e901c7f86d0767b8dcf0121aba
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584017"
---
# <a name="sharepointsiteusagesitecounts-resource-type"></a><span data-ttu-id="8b251-103">sharePointSiteUsageSiteCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="8b251-103">sharePointSiteUsageSiteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8b251-104">属性</span><span class="sxs-lookup"><span data-stu-id="8b251-104">Properties</span></span>

| <span data-ttu-id="8b251-105">属性</span><span class="sxs-lookup"><span data-stu-id="8b251-105">Property</span></span>          | <span data-ttu-id="8b251-106">类型</span><span class="sxs-lookup"><span data-stu-id="8b251-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="8b251-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8b251-107">reportRefreshDate</span></span> | <span data-ttu-id="8b251-108">Date</span><span class="sxs-lookup"><span data-stu-id="8b251-108">Date</span></span>   |
| <span data-ttu-id="8b251-109">siteType</span><span class="sxs-lookup"><span data-stu-id="8b251-109">siteType</span></span>          | <span data-ttu-id="8b251-110">String</span><span class="sxs-lookup"><span data-stu-id="8b251-110">String</span></span> |
| <span data-ttu-id="8b251-111">total</span><span class="sxs-lookup"><span data-stu-id="8b251-111">total</span></span>             | <span data-ttu-id="8b251-112">Int64</span><span class="sxs-lookup"><span data-stu-id="8b251-112">Int64</span></span>  |
| <span data-ttu-id="8b251-113">工作</span><span class="sxs-lookup"><span data-stu-id="8b251-113">active</span></span>            | <span data-ttu-id="8b251-114">Int64</span><span class="sxs-lookup"><span data-stu-id="8b251-114">Int64</span></span>  |
| <span data-ttu-id="8b251-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="8b251-115">reportDate</span></span>        | <span data-ttu-id="8b251-116">Date</span><span class="sxs-lookup"><span data-stu-id="8b251-116">Date</span></span>   |
| <span data-ttu-id="8b251-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8b251-117">reportPeriod</span></span>      | <span data-ttu-id="8b251-118">String</span><span class="sxs-lookup"><span data-stu-id="8b251-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8b251-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b251-119">JSON representation</span></span>

<span data-ttu-id="8b251-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b251-120">The following is a JSON representation of the resource.</span></span>

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
