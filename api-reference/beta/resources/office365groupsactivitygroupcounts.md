---
title: office365GroupsActivityGroupCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: b202d5189c1edeeeaa45d447aa7cc078dd263858
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581420"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="ada03-103">office365GroupsActivityGroupCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="ada03-103">office365GroupsActivityGroupCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ada03-104">属性</span><span class="sxs-lookup"><span data-stu-id="ada03-104">Properties</span></span>

| <span data-ttu-id="ada03-105">属性</span><span class="sxs-lookup"><span data-stu-id="ada03-105">Property</span></span>          | <span data-ttu-id="ada03-106">类型</span><span class="sxs-lookup"><span data-stu-id="ada03-106">Type</span></span>   | <span data-ttu-id="ada03-107">说明</span><span class="sxs-lookup"><span data-stu-id="ada03-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="ada03-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ada03-108">reportRefreshDate</span></span> | <span data-ttu-id="ada03-109">Date</span><span class="sxs-lookup"><span data-stu-id="ada03-109">Date</span></span>   | <span data-ttu-id="ada03-110">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="ada03-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="ada03-111">total</span><span class="sxs-lookup"><span data-stu-id="ada03-111">total</span></span>             | <span data-ttu-id="ada03-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ada03-112">Int64</span></span>  | <span data-ttu-id="ada03-113">总组数。</span><span class="sxs-lookup"><span data-stu-id="ada03-113">The total number of groups.</span></span>              |
| <span data-ttu-id="ada03-114">工作</span><span class="sxs-lookup"><span data-stu-id="ada03-114">active</span></span>            | <span data-ttu-id="ada03-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ada03-115">Int64</span></span>  | <span data-ttu-id="ada03-116">活动组的数量。</span><span class="sxs-lookup"><span data-stu-id="ada03-116">The number of active groups.</span></span> <span data-ttu-id="ada03-117">如果发生以下任一情况, 则会将组视为活动的: 组邮箱收到电子邮件;用户在 SharePoint 文档库中查看、编辑、共享或同步文件;用户查看了 SharePoint 页面;用户在 Yammer 组中投递、阅读或赞了邮件。</span><span class="sxs-lookup"><span data-stu-id="ada03-117">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="ada03-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="ada03-118">reportDate</span></span>        | <span data-ttu-id="ada03-119">Date</span><span class="sxs-lookup"><span data-stu-id="ada03-119">Date</span></span>   | <span data-ttu-id="ada03-120">多个组处于活动状态的日期。</span><span class="sxs-lookup"><span data-stu-id="ada03-120">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="ada03-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ada03-121">reportPeriod</span></span>      | <span data-ttu-id="ada03-122">String</span><span class="sxs-lookup"><span data-stu-id="ada03-122">String</span></span> | <span data-ttu-id="ada03-123">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="ada03-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="ada03-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ada03-124">JSON representation</span></span>

<span data-ttu-id="ada03-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ada03-125">The following is a JSON representation of the resource.</span></span>

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
