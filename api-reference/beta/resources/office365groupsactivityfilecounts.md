---
title: office365GroupsActivityFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 8154f24fe36f2c11f3926412c3fcc062be04b5ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966522"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="b4742-103">office365GroupsActivityFileCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="b4742-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b4742-104">属性</span><span class="sxs-lookup"><span data-stu-id="b4742-104">Properties</span></span>

| <span data-ttu-id="b4742-105">属性</span><span class="sxs-lookup"><span data-stu-id="b4742-105">Property</span></span>          | <span data-ttu-id="b4742-106">类型</span><span class="sxs-lookup"><span data-stu-id="b4742-106">Type</span></span>   | <span data-ttu-id="b4742-107">说明</span><span class="sxs-lookup"><span data-stu-id="b4742-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="b4742-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b4742-108">reportRefreshDate</span></span> | <span data-ttu-id="b4742-109">日期</span><span class="sxs-lookup"><span data-stu-id="b4742-109">Date</span></span>   | <span data-ttu-id="b4742-110">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="b4742-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="b4742-111">total</span><span class="sxs-lookup"><span data-stu-id="b4742-111">total</span></span>             | <span data-ttu-id="b4742-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b4742-112">Int64</span></span>  | <span data-ttu-id="b4742-113">组的 SharePoint 文档库中的总文件数。</span><span class="sxs-lookup"><span data-stu-id="b4742-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="b4742-114">工作</span><span class="sxs-lookup"><span data-stu-id="b4742-114">active</span></span>            | <span data-ttu-id="b4742-115">Int64</span><span class="sxs-lookup"><span data-stu-id="b4742-115">Int64</span></span>  | <span data-ttu-id="b4742-116">在组的 SharePoint 文档库中查看、编辑、共享或同步的文件数。</span><span class="sxs-lookup"><span data-stu-id="b4742-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="b4742-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="b4742-117">reportDate</span></span>        | <span data-ttu-id="b4742-118">日期</span><span class="sxs-lookup"><span data-stu-id="b4742-118">Date</span></span>   | <span data-ttu-id="b4742-119">组的 SharePoint 网站中处于活动状态的多个文件的日期。</span><span class="sxs-lookup"><span data-stu-id="b4742-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="b4742-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b4742-120">reportPeriod</span></span>      | <span data-ttu-id="b4742-121">String</span><span class="sxs-lookup"><span data-stu-id="b4742-121">String</span></span> | <span data-ttu-id="b4742-122">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="b4742-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="b4742-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4742-123">JSON representation</span></span>

<span data-ttu-id="b4742-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4742-124">The following is a JSON representation of the resource.</span></span>

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
