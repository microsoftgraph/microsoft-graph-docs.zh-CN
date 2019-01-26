---
title: office365GroupsActivityFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 89ac23b89730ec98515d6d0d3c06867e57b19ed1
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575574"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="3e83c-103">office365GroupsActivityFileCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e83c-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="3e83c-104">属性</span><span class="sxs-lookup"><span data-stu-id="3e83c-104">Properties</span></span>

| <span data-ttu-id="3e83c-105">属性</span><span class="sxs-lookup"><span data-stu-id="3e83c-105">Property</span></span>          | <span data-ttu-id="3e83c-106">类型</span><span class="sxs-lookup"><span data-stu-id="3e83c-106">Type</span></span>   | <span data-ttu-id="3e83c-107">说明</span><span class="sxs-lookup"><span data-stu-id="3e83c-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="3e83c-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3e83c-108">reportRefreshDate</span></span> | <span data-ttu-id="3e83c-109">Date</span><span class="sxs-lookup"><span data-stu-id="3e83c-109">Date</span></span>   | <span data-ttu-id="3e83c-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="3e83c-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="3e83c-111">total</span><span class="sxs-lookup"><span data-stu-id="3e83c-111">total</span></span>             | <span data-ttu-id="3e83c-112">Int64</span><span class="sxs-lookup"><span data-stu-id="3e83c-112">Int64</span></span>  | <span data-ttu-id="3e83c-113">组的 SharePoint 文档库中的文件总数。</span><span class="sxs-lookup"><span data-stu-id="3e83c-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="3e83c-114">活动</span><span class="sxs-lookup"><span data-stu-id="3e83c-114">active</span></span>            | <span data-ttu-id="3e83c-115">Int64</span><span class="sxs-lookup"><span data-stu-id="3e83c-115">Int64</span></span>  | <span data-ttu-id="3e83c-116">查看过的文件数编辑、 共享，或组的 SharePoint 文档库同步。</span><span class="sxs-lookup"><span data-stu-id="3e83c-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="3e83c-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="3e83c-117">reportDate</span></span>        | <span data-ttu-id="3e83c-118">Date</span><span class="sxs-lookup"><span data-stu-id="3e83c-118">Date</span></span>   | <span data-ttu-id="3e83c-119">在其的文件数处于活动状态的组的 SharePoint 网站中的日期。</span><span class="sxs-lookup"><span data-stu-id="3e83c-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="3e83c-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3e83c-120">reportPeriod</span></span>      | <span data-ttu-id="3e83c-121">String</span><span class="sxs-lookup"><span data-stu-id="3e83c-121">String</span></span> | <span data-ttu-id="3e83c-122">报告涵盖天数。</span><span class="sxs-lookup"><span data-stu-id="3e83c-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="3e83c-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e83c-123">JSON representation</span></span>

<span data-ttu-id="3e83c-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e83c-124">The following is a JSON representation of the resource.</span></span>

<!-- {

  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityFileCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
