---
title: office365GroupsActivityGroupCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: ad2610f5cbd3aae56651a0a5651e4ee4319b3bb2
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981492"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="8da7c-103">office365GroupsActivityGroupCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="8da7c-103">office365GroupsActivityGroupCounts resource type</span></span>

<span data-ttu-id="8da7c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8da7c-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="8da7c-105">属性</span><span class="sxs-lookup"><span data-stu-id="8da7c-105">Properties</span></span>

| <span data-ttu-id="8da7c-106">属性</span><span class="sxs-lookup"><span data-stu-id="8da7c-106">Property</span></span>          | <span data-ttu-id="8da7c-107">类型</span><span class="sxs-lookup"><span data-stu-id="8da7c-107">Type</span></span>   | <span data-ttu-id="8da7c-108">说明</span><span class="sxs-lookup"><span data-stu-id="8da7c-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="8da7c-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8da7c-109">reportRefreshDate</span></span> | <span data-ttu-id="8da7c-110">日期</span><span class="sxs-lookup"><span data-stu-id="8da7c-110">Date</span></span>   | <span data-ttu-id="8da7c-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="8da7c-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="8da7c-112">total</span><span class="sxs-lookup"><span data-stu-id="8da7c-112">total</span></span>             | <span data-ttu-id="8da7c-113">Int64</span><span class="sxs-lookup"><span data-stu-id="8da7c-113">Int64</span></span>  | <span data-ttu-id="8da7c-114">组总数。</span><span class="sxs-lookup"><span data-stu-id="8da7c-114">The total number of groups.</span></span>              |
| <span data-ttu-id="8da7c-115">active</span><span class="sxs-lookup"><span data-stu-id="8da7c-115">active</span></span>            | <span data-ttu-id="8da7c-116">Int64</span><span class="sxs-lookup"><span data-stu-id="8da7c-116">Int64</span></span>  | <span data-ttu-id="8da7c-117">活动组的数量。</span><span class="sxs-lookup"><span data-stu-id="8da7c-117">The number of active groups.</span></span> <span data-ttu-id="8da7c-118">如果发生以下任一情况，则认为组处于活动状态：组邮箱收到电子邮件;用户在 SharePoint 文档库中查看、编辑、共享或同步的文件;用户查看的 SharePoint 页面;用户发布、阅读或喜欢的 Yammer 组中的消息。</span><span class="sxs-lookup"><span data-stu-id="8da7c-118">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="8da7c-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="8da7c-119">reportDate</span></span>        | <span data-ttu-id="8da7c-120">日期</span><span class="sxs-lookup"><span data-stu-id="8da7c-120">Date</span></span>   | <span data-ttu-id="8da7c-121">多个组处于活动状态的日期。</span><span class="sxs-lookup"><span data-stu-id="8da7c-121">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="8da7c-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8da7c-122">reportPeriod</span></span>      | <span data-ttu-id="8da7c-123">String</span><span class="sxs-lookup"><span data-stu-id="8da7c-123">String</span></span> | <span data-ttu-id="8da7c-124">报告涵盖的天数。</span><span class="sxs-lookup"><span data-stu-id="8da7c-124">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="8da7c-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8da7c-125">JSON representation</span></span>

<span data-ttu-id="8da7c-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8da7c-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityGroupCounts"
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


