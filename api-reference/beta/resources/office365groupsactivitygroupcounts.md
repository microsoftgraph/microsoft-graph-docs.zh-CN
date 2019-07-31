---
title: office365GroupsActivityGroupCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 3f49ddaf6f62367c5e8ebbffae669bf3cc1d86f8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009480"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="27c9b-103">office365GroupsActivityGroupCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="27c9b-103">office365GroupsActivityGroupCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="27c9b-104">属性</span><span class="sxs-lookup"><span data-stu-id="27c9b-104">Properties</span></span>

| <span data-ttu-id="27c9b-105">属性</span><span class="sxs-lookup"><span data-stu-id="27c9b-105">Property</span></span>          | <span data-ttu-id="27c9b-106">类型</span><span class="sxs-lookup"><span data-stu-id="27c9b-106">Type</span></span>   | <span data-ttu-id="27c9b-107">说明</span><span class="sxs-lookup"><span data-stu-id="27c9b-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="27c9b-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="27c9b-108">reportRefreshDate</span></span> | <span data-ttu-id="27c9b-109">日期</span><span class="sxs-lookup"><span data-stu-id="27c9b-109">Date</span></span>   | <span data-ttu-id="27c9b-110">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="27c9b-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="27c9b-111">total</span><span class="sxs-lookup"><span data-stu-id="27c9b-111">total</span></span>             | <span data-ttu-id="27c9b-112">Int64</span><span class="sxs-lookup"><span data-stu-id="27c9b-112">Int64</span></span>  | <span data-ttu-id="27c9b-113">总组数。</span><span class="sxs-lookup"><span data-stu-id="27c9b-113">The total number of groups.</span></span>              |
| <span data-ttu-id="27c9b-114">工作</span><span class="sxs-lookup"><span data-stu-id="27c9b-114">active</span></span>            | <span data-ttu-id="27c9b-115">Int64</span><span class="sxs-lookup"><span data-stu-id="27c9b-115">Int64</span></span>  | <span data-ttu-id="27c9b-116">活动组的数量。</span><span class="sxs-lookup"><span data-stu-id="27c9b-116">The number of active groups.</span></span> <span data-ttu-id="27c9b-117">如果发生以下任一情况, 则会将组视为活动的: 组邮箱收到电子邮件;用户在 SharePoint 文档库中查看、编辑、共享或同步文件;用户查看了 SharePoint 页面;用户在 Yammer 组中投递、阅读或赞了邮件。</span><span class="sxs-lookup"><span data-stu-id="27c9b-117">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="27c9b-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="27c9b-118">reportDate</span></span>        | <span data-ttu-id="27c9b-119">日期</span><span class="sxs-lookup"><span data-stu-id="27c9b-119">Date</span></span>   | <span data-ttu-id="27c9b-120">多个组处于活动状态的日期。</span><span class="sxs-lookup"><span data-stu-id="27c9b-120">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="27c9b-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="27c9b-121">reportPeriod</span></span>      | <span data-ttu-id="27c9b-122">String</span><span class="sxs-lookup"><span data-stu-id="27c9b-122">String</span></span> | <span data-ttu-id="27c9b-123">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="27c9b-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="27c9b-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="27c9b-124">JSON representation</span></span>

<span data-ttu-id="27c9b-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27c9b-125">The following is a JSON representation of the resource.</span></span>

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
