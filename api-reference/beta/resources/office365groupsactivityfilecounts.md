---
title: office365GroupsActivityFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 1f4f26e141dc25e1e5e249ad116bc9a988274f18
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981499"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="acabd-103">office365GroupsActivityFileCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="acabd-103">office365GroupsActivityFileCounts resource type</span></span>

<span data-ttu-id="acabd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acabd-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="acabd-105">属性</span><span class="sxs-lookup"><span data-stu-id="acabd-105">Properties</span></span>

| <span data-ttu-id="acabd-106">属性</span><span class="sxs-lookup"><span data-stu-id="acabd-106">Property</span></span>          | <span data-ttu-id="acabd-107">类型</span><span class="sxs-lookup"><span data-stu-id="acabd-107">Type</span></span>   | <span data-ttu-id="acabd-108">说明</span><span class="sxs-lookup"><span data-stu-id="acabd-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="acabd-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="acabd-109">reportRefreshDate</span></span> | <span data-ttu-id="acabd-110">日期</span><span class="sxs-lookup"><span data-stu-id="acabd-110">Date</span></span>   | <span data-ttu-id="acabd-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="acabd-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="acabd-112">total</span><span class="sxs-lookup"><span data-stu-id="acabd-112">total</span></span>             | <span data-ttu-id="acabd-113">Int64</span><span class="sxs-lookup"><span data-stu-id="acabd-113">Int64</span></span>  | <span data-ttu-id="acabd-114">组的 SharePoint 文档库中的文件总数。</span><span class="sxs-lookup"><span data-stu-id="acabd-114">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="acabd-115">active</span><span class="sxs-lookup"><span data-stu-id="acabd-115">active</span></span>            | <span data-ttu-id="acabd-116">Int64</span><span class="sxs-lookup"><span data-stu-id="acabd-116">Int64</span></span>  | <span data-ttu-id="acabd-117">在组的 SharePoint 文档库中查看、编辑、共享或同步的文件数。</span><span class="sxs-lookup"><span data-stu-id="acabd-117">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="acabd-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="acabd-118">reportDate</span></span>        | <span data-ttu-id="acabd-119">日期</span><span class="sxs-lookup"><span data-stu-id="acabd-119">Date</span></span>   | <span data-ttu-id="acabd-120">许多文件在组的 SharePoint 网站中处于活动状态的日期。</span><span class="sxs-lookup"><span data-stu-id="acabd-120">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="acabd-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="acabd-121">reportPeriod</span></span>      | <span data-ttu-id="acabd-122">String</span><span class="sxs-lookup"><span data-stu-id="acabd-122">String</span></span> | <span data-ttu-id="acabd-123">报告涵盖的天数。</span><span class="sxs-lookup"><span data-stu-id="acabd-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="acabd-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="acabd-124">JSON representation</span></span>

<span data-ttu-id="acabd-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="acabd-125">The following is a JSON representation of the resource.</span></span>

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


