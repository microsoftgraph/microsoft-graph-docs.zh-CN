---
title: office365GroupsActivityFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: c887ecb526d9c4215c1d8586bcbcb799c9e2c476
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092403"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="39d32-103">office365GroupsActivityFileCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="39d32-103">office365GroupsActivityFileCounts resource type</span></span>

<span data-ttu-id="39d32-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39d32-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="39d32-105">属性</span><span class="sxs-lookup"><span data-stu-id="39d32-105">Properties</span></span>

| <span data-ttu-id="39d32-106">属性</span><span class="sxs-lookup"><span data-stu-id="39d32-106">Property</span></span>          | <span data-ttu-id="39d32-107">类型</span><span class="sxs-lookup"><span data-stu-id="39d32-107">Type</span></span>   | <span data-ttu-id="39d32-108">说明</span><span class="sxs-lookup"><span data-stu-id="39d32-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="39d32-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="39d32-109">reportRefreshDate</span></span> | <span data-ttu-id="39d32-110">日期</span><span class="sxs-lookup"><span data-stu-id="39d32-110">Date</span></span>   | <span data-ttu-id="39d32-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="39d32-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="39d32-112">total</span><span class="sxs-lookup"><span data-stu-id="39d32-112">total</span></span>             | <span data-ttu-id="39d32-113">Int64</span><span class="sxs-lookup"><span data-stu-id="39d32-113">Int64</span></span>  | <span data-ttu-id="39d32-114">组的 SharePoint 文档库中的总文件数。</span><span class="sxs-lookup"><span data-stu-id="39d32-114">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="39d32-115">工作</span><span class="sxs-lookup"><span data-stu-id="39d32-115">active</span></span>            | <span data-ttu-id="39d32-116">Int64</span><span class="sxs-lookup"><span data-stu-id="39d32-116">Int64</span></span>  | <span data-ttu-id="39d32-117">在组的 SharePoint 文档库中查看、编辑、共享或同步的文件数。</span><span class="sxs-lookup"><span data-stu-id="39d32-117">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="39d32-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="39d32-118">reportDate</span></span>        | <span data-ttu-id="39d32-119">日期</span><span class="sxs-lookup"><span data-stu-id="39d32-119">Date</span></span>   | <span data-ttu-id="39d32-120">组的 SharePoint 网站中处于活动状态的多个文件的日期。</span><span class="sxs-lookup"><span data-stu-id="39d32-120">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="39d32-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="39d32-121">reportPeriod</span></span>      | <span data-ttu-id="39d32-122">字符串</span><span class="sxs-lookup"><span data-stu-id="39d32-122">String</span></span> | <span data-ttu-id="39d32-123">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="39d32-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="39d32-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39d32-124">JSON representation</span></span>

<span data-ttu-id="39d32-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39d32-125">The following is a JSON representation of the resource.</span></span>

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


