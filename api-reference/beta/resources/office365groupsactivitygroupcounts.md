---
title: office365GroupsActivityGroupCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: c249123a01cde2fe952f5111affe645415ddc6cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092382"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="b1aea-103">office365GroupsActivityGroupCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="b1aea-103">office365GroupsActivityGroupCounts resource type</span></span>

<span data-ttu-id="b1aea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1aea-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="b1aea-105">属性</span><span class="sxs-lookup"><span data-stu-id="b1aea-105">Properties</span></span>

| <span data-ttu-id="b1aea-106">属性</span><span class="sxs-lookup"><span data-stu-id="b1aea-106">Property</span></span>          | <span data-ttu-id="b1aea-107">类型</span><span class="sxs-lookup"><span data-stu-id="b1aea-107">Type</span></span>   | <span data-ttu-id="b1aea-108">说明</span><span class="sxs-lookup"><span data-stu-id="b1aea-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="b1aea-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b1aea-109">reportRefreshDate</span></span> | <span data-ttu-id="b1aea-110">日期</span><span class="sxs-lookup"><span data-stu-id="b1aea-110">Date</span></span>   | <span data-ttu-id="b1aea-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="b1aea-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="b1aea-112">total</span><span class="sxs-lookup"><span data-stu-id="b1aea-112">total</span></span>             | <span data-ttu-id="b1aea-113">Int64</span><span class="sxs-lookup"><span data-stu-id="b1aea-113">Int64</span></span>  | <span data-ttu-id="b1aea-114">总组数。</span><span class="sxs-lookup"><span data-stu-id="b1aea-114">The total number of groups.</span></span>              |
| <span data-ttu-id="b1aea-115">工作</span><span class="sxs-lookup"><span data-stu-id="b1aea-115">active</span></span>            | <span data-ttu-id="b1aea-116">Int64</span><span class="sxs-lookup"><span data-stu-id="b1aea-116">Int64</span></span>  | <span data-ttu-id="b1aea-117">活动组的数量。</span><span class="sxs-lookup"><span data-stu-id="b1aea-117">The number of active groups.</span></span> <span data-ttu-id="b1aea-118">如果发生以下任一情况，则会将组视为活动的：组邮箱收到电子邮件;用户在 SharePoint 文档库中查看、编辑、共享或同步文件;用户查看了 SharePoint 页面;用户在 Yammer 组中投递、阅读或赞了邮件。</span><span class="sxs-lookup"><span data-stu-id="b1aea-118">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="b1aea-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="b1aea-119">reportDate</span></span>        | <span data-ttu-id="b1aea-120">日期</span><span class="sxs-lookup"><span data-stu-id="b1aea-120">Date</span></span>   | <span data-ttu-id="b1aea-121">多个组处于活动状态的日期。</span><span class="sxs-lookup"><span data-stu-id="b1aea-121">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="b1aea-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b1aea-122">reportPeriod</span></span>      | <span data-ttu-id="b1aea-123">字符串</span><span class="sxs-lookup"><span data-stu-id="b1aea-123">String</span></span> | <span data-ttu-id="b1aea-124">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="b1aea-124">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="b1aea-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1aea-125">JSON representation</span></span>

<span data-ttu-id="b1aea-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1aea-126">The following is a JSON representation of the resource.</span></span>

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


