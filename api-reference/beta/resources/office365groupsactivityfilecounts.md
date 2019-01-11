---
title: office365GroupsActivityFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 856bb4c74c8af35775b6fe71cb75d89935440bdb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819183"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="df772-103">office365GroupsActivityFileCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="df772-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="df772-104">属性</span><span class="sxs-lookup"><span data-stu-id="df772-104">Properties</span></span>

| <span data-ttu-id="df772-105">属性</span><span class="sxs-lookup"><span data-stu-id="df772-105">Property</span></span>          | <span data-ttu-id="df772-106">类型</span><span class="sxs-lookup"><span data-stu-id="df772-106">Type</span></span>   | <span data-ttu-id="df772-107">Description</span><span class="sxs-lookup"><span data-stu-id="df772-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="df772-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="df772-108">reportRefreshDate</span></span> | <span data-ttu-id="df772-109">日期</span><span class="sxs-lookup"><span data-stu-id="df772-109">Date</span></span>   | <span data-ttu-id="df772-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="df772-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="df772-111">total</span><span class="sxs-lookup"><span data-stu-id="df772-111">total</span></span>             | <span data-ttu-id="df772-112">Int64</span><span class="sxs-lookup"><span data-stu-id="df772-112">Int64</span></span>  | <span data-ttu-id="df772-113">组的 SharePoint 文档库中的文件总数。</span><span class="sxs-lookup"><span data-stu-id="df772-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="df772-114">活动</span><span class="sxs-lookup"><span data-stu-id="df772-114">active</span></span>            | <span data-ttu-id="df772-115">Int64</span><span class="sxs-lookup"><span data-stu-id="df772-115">Int64</span></span>  | <span data-ttu-id="df772-116">查看过的文件数编辑、 共享，或组的 SharePoint 文档库同步。</span><span class="sxs-lookup"><span data-stu-id="df772-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="df772-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="df772-117">reportDate</span></span>        | <span data-ttu-id="df772-118">日期</span><span class="sxs-lookup"><span data-stu-id="df772-118">Date</span></span>   | <span data-ttu-id="df772-119">在其的文件数处于活动状态的组的 SharePoint 网站中的日期。</span><span class="sxs-lookup"><span data-stu-id="df772-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="df772-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="df772-120">reportPeriod</span></span>      | <span data-ttu-id="df772-121">字符串</span><span class="sxs-lookup"><span data-stu-id="df772-121">String</span></span> | <span data-ttu-id="df772-122">报告涵盖天数。</span><span class="sxs-lookup"><span data-stu-id="df772-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="df772-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df772-123">JSON representation</span></span>

<span data-ttu-id="df772-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df772-124">The following is a JSON representation of the resource.</span></span>

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
