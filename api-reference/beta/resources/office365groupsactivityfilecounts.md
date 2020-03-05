---
title: office365GroupsActivityFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: dff3266aa268f2d26ca15492c72fa25a5f562a29
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522440"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="28682-103">office365GroupsActivityFileCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="28682-103">office365GroupsActivityFileCounts resource type</span></span>

<span data-ttu-id="28682-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="28682-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="28682-105">属性</span><span class="sxs-lookup"><span data-stu-id="28682-105">Properties</span></span>

| <span data-ttu-id="28682-106">属性</span><span class="sxs-lookup"><span data-stu-id="28682-106">Property</span></span>          | <span data-ttu-id="28682-107">类型</span><span class="sxs-lookup"><span data-stu-id="28682-107">Type</span></span>   | <span data-ttu-id="28682-108">说明</span><span class="sxs-lookup"><span data-stu-id="28682-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="28682-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="28682-109">reportRefreshDate</span></span> | <span data-ttu-id="28682-110">日期</span><span class="sxs-lookup"><span data-stu-id="28682-110">Date</span></span>   | <span data-ttu-id="28682-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="28682-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="28682-112">total</span><span class="sxs-lookup"><span data-stu-id="28682-112">total</span></span>             | <span data-ttu-id="28682-113">Int64</span><span class="sxs-lookup"><span data-stu-id="28682-113">Int64</span></span>  | <span data-ttu-id="28682-114">组的 SharePoint 文档库中的总文件数。</span><span class="sxs-lookup"><span data-stu-id="28682-114">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="28682-115">工作</span><span class="sxs-lookup"><span data-stu-id="28682-115">active</span></span>            | <span data-ttu-id="28682-116">Int64</span><span class="sxs-lookup"><span data-stu-id="28682-116">Int64</span></span>  | <span data-ttu-id="28682-117">在组的 SharePoint 文档库中查看、编辑、共享或同步的文件数。</span><span class="sxs-lookup"><span data-stu-id="28682-117">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="28682-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="28682-118">reportDate</span></span>        | <span data-ttu-id="28682-119">日期</span><span class="sxs-lookup"><span data-stu-id="28682-119">Date</span></span>   | <span data-ttu-id="28682-120">组的 SharePoint 网站中处于活动状态的多个文件的日期。</span><span class="sxs-lookup"><span data-stu-id="28682-120">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="28682-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="28682-121">reportPeriod</span></span>      | <span data-ttu-id="28682-122">String</span><span class="sxs-lookup"><span data-stu-id="28682-122">String</span></span> | <span data-ttu-id="28682-123">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="28682-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="28682-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28682-124">JSON representation</span></span>

<span data-ttu-id="28682-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28682-125">The following is a JSON representation of the resource.</span></span>

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
