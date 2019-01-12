---
title: office365GroupsActivityGroupCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d3c1272f9bd99c3e7ee0f29a4c303e1c8ca95525
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975881"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="6d4f4-103">office365GroupsActivityGroupCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d4f4-103">office365GroupsActivityGroupCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6d4f4-104">属性</span><span class="sxs-lookup"><span data-stu-id="6d4f4-104">Properties</span></span>

| <span data-ttu-id="6d4f4-105">属性</span><span class="sxs-lookup"><span data-stu-id="6d4f4-105">Property</span></span>          | <span data-ttu-id="6d4f4-106">类型</span><span class="sxs-lookup"><span data-stu-id="6d4f4-106">Type</span></span>   | <span data-ttu-id="6d4f4-107">说明</span><span class="sxs-lookup"><span data-stu-id="6d4f4-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="6d4f4-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6d4f4-108">reportRefreshDate</span></span> | <span data-ttu-id="6d4f4-109">日期</span><span class="sxs-lookup"><span data-stu-id="6d4f4-109">Date</span></span>   | <span data-ttu-id="6d4f4-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="6d4f4-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="6d4f4-111">total</span><span class="sxs-lookup"><span data-stu-id="6d4f4-111">total</span></span>             | <span data-ttu-id="6d4f4-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6d4f4-112">Int64</span></span>  | <span data-ttu-id="6d4f4-113">组的总数。</span><span class="sxs-lookup"><span data-stu-id="6d4f4-113">The total number of groups.</span></span>              |
| <span data-ttu-id="6d4f4-114">活动</span><span class="sxs-lookup"><span data-stu-id="6d4f4-114">active</span></span>            | <span data-ttu-id="6d4f4-115">Int64</span><span class="sxs-lookup"><span data-stu-id="6d4f4-115">Int64</span></span>  | <span data-ttu-id="6d4f4-116">活动的组的数目。</span><span class="sxs-lookup"><span data-stu-id="6d4f4-116">The number of active groups.</span></span> <span data-ttu-id="6d4f4-117">组被视为活动发生以下任一： 组邮箱收到电子邮件;用户可以查看、 编辑、 共享，或同步中 SharePoint 文档库; 文件用户查看 SharePoint 页面; 例如：用户发布、 读取或喜欢 Yammer 组中的邮件。</span><span class="sxs-lookup"><span data-stu-id="6d4f4-117">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="6d4f4-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="6d4f4-118">reportDate</span></span>        | <span data-ttu-id="6d4f4-119">日期</span><span class="sxs-lookup"><span data-stu-id="6d4f4-119">Date</span></span>   | <span data-ttu-id="6d4f4-120">在其的组数处于活动状态日期。</span><span class="sxs-lookup"><span data-stu-id="6d4f4-120">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="6d4f4-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6d4f4-121">reportPeriod</span></span>      | <span data-ttu-id="6d4f4-122">字符串</span><span class="sxs-lookup"><span data-stu-id="6d4f4-122">String</span></span> | <span data-ttu-id="6d4f4-123">报告涵盖天数。</span><span class="sxs-lookup"><span data-stu-id="6d4f4-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="6d4f4-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d4f4-124">JSON representation</span></span>

<span data-ttu-id="6d4f4-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d4f4-125">The following is a JSON representation of the resource.</span></span>

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
