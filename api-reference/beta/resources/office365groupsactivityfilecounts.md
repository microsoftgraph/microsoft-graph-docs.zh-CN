---
title: office365GroupsActivityFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 89ac23b89730ec98515d6d0d3c06867e57b19ed1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457072"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="48fed-103">office365GroupsActivityFileCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="48fed-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="48fed-104">属性</span><span class="sxs-lookup"><span data-stu-id="48fed-104">Properties</span></span>

| <span data-ttu-id="48fed-105">属性</span><span class="sxs-lookup"><span data-stu-id="48fed-105">Property</span></span>          | <span data-ttu-id="48fed-106">类型</span><span class="sxs-lookup"><span data-stu-id="48fed-106">Type</span></span>   | <span data-ttu-id="48fed-107">描述</span><span class="sxs-lookup"><span data-stu-id="48fed-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="48fed-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="48fed-108">reportRefreshDate</span></span> | <span data-ttu-id="48fed-109">日期</span><span class="sxs-lookup"><span data-stu-id="48fed-109">Date</span></span>   | <span data-ttu-id="48fed-110">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="48fed-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="48fed-111">total</span><span class="sxs-lookup"><span data-stu-id="48fed-111">total</span></span>             | <span data-ttu-id="48fed-112">Int64</span><span class="sxs-lookup"><span data-stu-id="48fed-112">Int64</span></span>  | <span data-ttu-id="48fed-113">组的 SharePoint 文档库中的总文件数。</span><span class="sxs-lookup"><span data-stu-id="48fed-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="48fed-114">工作</span><span class="sxs-lookup"><span data-stu-id="48fed-114">active</span></span>            | <span data-ttu-id="48fed-115">Int64</span><span class="sxs-lookup"><span data-stu-id="48fed-115">Int64</span></span>  | <span data-ttu-id="48fed-116">在组的 SharePoint 文档库中查看、编辑、共享或同步的文件数。</span><span class="sxs-lookup"><span data-stu-id="48fed-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="48fed-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="48fed-117">reportDate</span></span>        | <span data-ttu-id="48fed-118">日期</span><span class="sxs-lookup"><span data-stu-id="48fed-118">Date</span></span>   | <span data-ttu-id="48fed-119">组的 SharePoint 网站中处于活动状态的多个文件的日期。</span><span class="sxs-lookup"><span data-stu-id="48fed-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="48fed-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="48fed-120">reportPeriod</span></span>      | <span data-ttu-id="48fed-121">字符串</span><span class="sxs-lookup"><span data-stu-id="48fed-121">String</span></span> | <span data-ttu-id="48fed-122">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="48fed-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="48fed-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48fed-123">JSON representation</span></span>

<span data-ttu-id="48fed-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48fed-124">The following is a JSON representation of the resource.</span></span>

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
