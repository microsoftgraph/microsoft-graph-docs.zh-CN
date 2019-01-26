---
title: office365GroupsActivityStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0485fd95046bc83350983bc1333dba83c79139d6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576379"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="5e5cd-103">office365GroupsActivityStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e5cd-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5e5cd-104">属性</span><span class="sxs-lookup"><span data-stu-id="5e5cd-104">Properties</span></span>

| <span data-ttu-id="5e5cd-105">属性</span><span class="sxs-lookup"><span data-stu-id="5e5cd-105">Property</span></span>                  | <span data-ttu-id="5e5cd-106">类型</span><span class="sxs-lookup"><span data-stu-id="5e5cd-106">Type</span></span>   | <span data-ttu-id="5e5cd-107">说明</span><span class="sxs-lookup"><span data-stu-id="5e5cd-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="5e5cd-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5e5cd-108">reportRefreshDate</span></span>         | <span data-ttu-id="5e5cd-109">Date</span><span class="sxs-lookup"><span data-stu-id="5e5cd-109">Date</span></span>   | <span data-ttu-id="5e5cd-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="5e5cd-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="5e5cd-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="5e5cd-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="5e5cd-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5e5cd-112">Int64</span></span>  | <span data-ttu-id="5e5cd-113">使用组邮箱中的存储。</span><span class="sxs-lookup"><span data-stu-id="5e5cd-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="5e5cd-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="5e5cd-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="5e5cd-115">Int64</span><span class="sxs-lookup"><span data-stu-id="5e5cd-115">Int64</span></span>  | <span data-ttu-id="5e5cd-116">在 SharePoint 文档库中使用的存储。</span><span class="sxs-lookup"><span data-stu-id="5e5cd-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="5e5cd-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="5e5cd-117">reportDate</span></span>                | <span data-ttu-id="5e5cd-118">Date</span><span class="sxs-lookup"><span data-stu-id="5e5cd-118">Date</span></span>   | <span data-ttu-id="5e5cd-119">Exchange 和 SharePoint 的快照日期用于存储。</span><span class="sxs-lookup"><span data-stu-id="5e5cd-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="5e5cd-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5e5cd-120">reportPeriod</span></span>              | <span data-ttu-id="5e5cd-121">String</span><span class="sxs-lookup"><span data-stu-id="5e5cd-121">String</span></span> | <span data-ttu-id="5e5cd-122">报告涵盖天数。</span><span class="sxs-lookup"><span data-stu-id="5e5cd-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="5e5cd-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e5cd-123">JSON representation</span></span>

<span data-ttu-id="5e5cd-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e5cd-124">The following is a JSON representation of the resource.</span></span>

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
