---
title: office365GroupsActivityStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 9824d3d172a8578f8a25a049c2d0d3b407bbc47e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862249"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="e7f77-103">office365GroupsActivityStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7f77-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e7f77-104">属性</span><span class="sxs-lookup"><span data-stu-id="e7f77-104">Properties</span></span>

| <span data-ttu-id="e7f77-105">属性</span><span class="sxs-lookup"><span data-stu-id="e7f77-105">Property</span></span>                  | <span data-ttu-id="e7f77-106">类型</span><span class="sxs-lookup"><span data-stu-id="e7f77-106">Type</span></span>   | <span data-ttu-id="e7f77-107">Description</span><span class="sxs-lookup"><span data-stu-id="e7f77-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="e7f77-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e7f77-108">reportRefreshDate</span></span>         | <span data-ttu-id="e7f77-109">日期</span><span class="sxs-lookup"><span data-stu-id="e7f77-109">Date</span></span>   | <span data-ttu-id="e7f77-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="e7f77-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="e7f77-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="e7f77-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="e7f77-112">Int64</span><span class="sxs-lookup"><span data-stu-id="e7f77-112">Int64</span></span>  | <span data-ttu-id="e7f77-113">使用组邮箱中的存储。</span><span class="sxs-lookup"><span data-stu-id="e7f77-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="e7f77-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="e7f77-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="e7f77-115">Int64</span><span class="sxs-lookup"><span data-stu-id="e7f77-115">Int64</span></span>  | <span data-ttu-id="e7f77-116">在 SharePoint 文档库中使用的存储。</span><span class="sxs-lookup"><span data-stu-id="e7f77-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="e7f77-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="e7f77-117">reportDate</span></span>                | <span data-ttu-id="e7f77-118">日期</span><span class="sxs-lookup"><span data-stu-id="e7f77-118">Date</span></span>   | <span data-ttu-id="e7f77-119">Exchange 和 SharePoint 的快照日期用于存储。</span><span class="sxs-lookup"><span data-stu-id="e7f77-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="e7f77-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e7f77-120">reportPeriod</span></span>              | <span data-ttu-id="e7f77-121">字符串</span><span class="sxs-lookup"><span data-stu-id="e7f77-121">String</span></span> | <span data-ttu-id="e7f77-122">报告涵盖天数。</span><span class="sxs-lookup"><span data-stu-id="e7f77-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="e7f77-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7f77-123">JSON representation</span></span>

<span data-ttu-id="e7f77-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7f77-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailboxStorageUsedInBytes": 1024, 
  "siteStorageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
