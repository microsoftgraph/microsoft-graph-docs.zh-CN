---
title: office365GroupsActivityGroupCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: bf84a0dcd2fc542735398e0aec2c6eb710d3f2f6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522433"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="95100-103">office365GroupsActivityGroupCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="95100-103">office365GroupsActivityGroupCounts resource type</span></span>

<span data-ttu-id="95100-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="95100-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="95100-105">属性</span><span class="sxs-lookup"><span data-stu-id="95100-105">Properties</span></span>

| <span data-ttu-id="95100-106">属性</span><span class="sxs-lookup"><span data-stu-id="95100-106">Property</span></span>          | <span data-ttu-id="95100-107">类型</span><span class="sxs-lookup"><span data-stu-id="95100-107">Type</span></span>   | <span data-ttu-id="95100-108">说明</span><span class="sxs-lookup"><span data-stu-id="95100-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="95100-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="95100-109">reportRefreshDate</span></span> | <span data-ttu-id="95100-110">日期</span><span class="sxs-lookup"><span data-stu-id="95100-110">Date</span></span>   | <span data-ttu-id="95100-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="95100-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="95100-112">total</span><span class="sxs-lookup"><span data-stu-id="95100-112">total</span></span>             | <span data-ttu-id="95100-113">Int64</span><span class="sxs-lookup"><span data-stu-id="95100-113">Int64</span></span>  | <span data-ttu-id="95100-114">总组数。</span><span class="sxs-lookup"><span data-stu-id="95100-114">The total number of groups.</span></span>              |
| <span data-ttu-id="95100-115">工作</span><span class="sxs-lookup"><span data-stu-id="95100-115">active</span></span>            | <span data-ttu-id="95100-116">Int64</span><span class="sxs-lookup"><span data-stu-id="95100-116">Int64</span></span>  | <span data-ttu-id="95100-117">活动组的数量。</span><span class="sxs-lookup"><span data-stu-id="95100-117">The number of active groups.</span></span> <span data-ttu-id="95100-118">如果发生以下任一情况，则会将组视为活动的：组邮箱收到电子邮件;用户在 SharePoint 文档库中查看、编辑、共享或同步文件;用户查看了 SharePoint 页面;用户在 Yammer 组中投递、阅读或赞了邮件。</span><span class="sxs-lookup"><span data-stu-id="95100-118">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="95100-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="95100-119">reportDate</span></span>        | <span data-ttu-id="95100-120">日期</span><span class="sxs-lookup"><span data-stu-id="95100-120">Date</span></span>   | <span data-ttu-id="95100-121">多个组处于活动状态的日期。</span><span class="sxs-lookup"><span data-stu-id="95100-121">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="95100-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="95100-122">reportPeriod</span></span>      | <span data-ttu-id="95100-123">String</span><span class="sxs-lookup"><span data-stu-id="95100-123">String</span></span> | <span data-ttu-id="95100-124">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="95100-124">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="95100-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95100-125">JSON representation</span></span>

<span data-ttu-id="95100-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95100-126">The following is a JSON representation of the resource.</span></span>

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
