---
title: office365GroupsActivityFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: adff009d9047aa147c8042059fbdab8491288fb7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972556"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="ca390-103">office365GroupsActivityFileCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca390-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ca390-104">属性</span><span class="sxs-lookup"><span data-stu-id="ca390-104">Properties</span></span>

| <span data-ttu-id="ca390-105">属性</span><span class="sxs-lookup"><span data-stu-id="ca390-105">Property</span></span>          | <span data-ttu-id="ca390-106">类型</span><span class="sxs-lookup"><span data-stu-id="ca390-106">Type</span></span>   | <span data-ttu-id="ca390-107">说明</span><span class="sxs-lookup"><span data-stu-id="ca390-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="ca390-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ca390-108">reportRefreshDate</span></span> | <span data-ttu-id="ca390-109">日期</span><span class="sxs-lookup"><span data-stu-id="ca390-109">Date</span></span>   | <span data-ttu-id="ca390-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="ca390-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="ca390-111">total</span><span class="sxs-lookup"><span data-stu-id="ca390-111">total</span></span>             | <span data-ttu-id="ca390-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ca390-112">Int64</span></span>  | <span data-ttu-id="ca390-113">组的 SharePoint 文档库中的文件总数。</span><span class="sxs-lookup"><span data-stu-id="ca390-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="ca390-114">活动</span><span class="sxs-lookup"><span data-stu-id="ca390-114">active</span></span>            | <span data-ttu-id="ca390-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ca390-115">Int64</span></span>  | <span data-ttu-id="ca390-116">查看过的文件数编辑、 共享，或组的 SharePoint 文档库同步。</span><span class="sxs-lookup"><span data-stu-id="ca390-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="ca390-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="ca390-117">reportDate</span></span>        | <span data-ttu-id="ca390-118">日期</span><span class="sxs-lookup"><span data-stu-id="ca390-118">Date</span></span>   | <span data-ttu-id="ca390-119">在其的文件数处于活动状态的组的 SharePoint 网站中的日期。</span><span class="sxs-lookup"><span data-stu-id="ca390-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="ca390-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ca390-120">reportPeriod</span></span>      | <span data-ttu-id="ca390-121">字符串</span><span class="sxs-lookup"><span data-stu-id="ca390-121">String</span></span> | <span data-ttu-id="ca390-122">报告涵盖天数。</span><span class="sxs-lookup"><span data-stu-id="ca390-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="ca390-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca390-123">JSON representation</span></span>

<span data-ttu-id="ca390-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca390-124">The following is a JSON representation of the resource.</span></span>

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
