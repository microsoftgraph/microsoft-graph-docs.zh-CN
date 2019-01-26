---
title: office365GroupsActivityGroupCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: b202d5189c1edeeeaa45d447aa7cc078dd263858
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572484"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="cd326-103">office365GroupsActivityGroupCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd326-103">office365GroupsActivityGroupCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="cd326-104">属性</span><span class="sxs-lookup"><span data-stu-id="cd326-104">Properties</span></span>

| <span data-ttu-id="cd326-105">属性</span><span class="sxs-lookup"><span data-stu-id="cd326-105">Property</span></span>          | <span data-ttu-id="cd326-106">类型</span><span class="sxs-lookup"><span data-stu-id="cd326-106">Type</span></span>   | <span data-ttu-id="cd326-107">说明</span><span class="sxs-lookup"><span data-stu-id="cd326-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="cd326-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="cd326-108">reportRefreshDate</span></span> | <span data-ttu-id="cd326-109">Date</span><span class="sxs-lookup"><span data-stu-id="cd326-109">Date</span></span>   | <span data-ttu-id="cd326-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="cd326-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="cd326-111">total</span><span class="sxs-lookup"><span data-stu-id="cd326-111">total</span></span>             | <span data-ttu-id="cd326-112">Int64</span><span class="sxs-lookup"><span data-stu-id="cd326-112">Int64</span></span>  | <span data-ttu-id="cd326-113">组的总数。</span><span class="sxs-lookup"><span data-stu-id="cd326-113">The total number of groups.</span></span>              |
| <span data-ttu-id="cd326-114">活动</span><span class="sxs-lookup"><span data-stu-id="cd326-114">active</span></span>            | <span data-ttu-id="cd326-115">Int64</span><span class="sxs-lookup"><span data-stu-id="cd326-115">Int64</span></span>  | <span data-ttu-id="cd326-116">活动的组的数目。</span><span class="sxs-lookup"><span data-stu-id="cd326-116">The number of active groups.</span></span> <span data-ttu-id="cd326-117">组被视为活动发生以下任一： 组邮箱收到电子邮件;用户可以查看、 编辑、 共享，或同步中 SharePoint 文档库; 文件用户查看 SharePoint 页面; 例如：用户发布、 读取或喜欢 Yammer 组中的邮件。</span><span class="sxs-lookup"><span data-stu-id="cd326-117">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="cd326-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="cd326-118">reportDate</span></span>        | <span data-ttu-id="cd326-119">Date</span><span class="sxs-lookup"><span data-stu-id="cd326-119">Date</span></span>   | <span data-ttu-id="cd326-120">在其的组数处于活动状态日期。</span><span class="sxs-lookup"><span data-stu-id="cd326-120">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="cd326-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="cd326-121">reportPeriod</span></span>      | <span data-ttu-id="cd326-122">String</span><span class="sxs-lookup"><span data-stu-id="cd326-122">String</span></span> | <span data-ttu-id="cd326-123">报告涵盖天数。</span><span class="sxs-lookup"><span data-stu-id="cd326-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="cd326-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd326-124">JSON representation</span></span>

<span data-ttu-id="cd326-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd326-125">The following is a JSON representation of the resource.</span></span>

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
