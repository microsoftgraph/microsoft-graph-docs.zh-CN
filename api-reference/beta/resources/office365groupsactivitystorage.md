---
title: office365GroupsActivityStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 7ac9ca260e4723f7c4aeca8e15f837d4cd57b7c4
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982178"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="0f1bf-103">office365GroupsActivityStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f1bf-103">office365GroupsActivityStorage resource type</span></span>

<span data-ttu-id="0f1bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f1bf-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="0f1bf-105">属性</span><span class="sxs-lookup"><span data-stu-id="0f1bf-105">Properties</span></span>

| <span data-ttu-id="0f1bf-106">属性</span><span class="sxs-lookup"><span data-stu-id="0f1bf-106">Property</span></span>                  | <span data-ttu-id="0f1bf-107">类型</span><span class="sxs-lookup"><span data-stu-id="0f1bf-107">Type</span></span>   | <span data-ttu-id="0f1bf-108">说明</span><span class="sxs-lookup"><span data-stu-id="0f1bf-108">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="0f1bf-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0f1bf-109">reportRefreshDate</span></span>         | <span data-ttu-id="0f1bf-110">日期</span><span class="sxs-lookup"><span data-stu-id="0f1bf-110">Date</span></span>   | <span data-ttu-id="0f1bf-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="0f1bf-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="0f1bf-112">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="0f1bf-112">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="0f1bf-113">Int64</span><span class="sxs-lookup"><span data-stu-id="0f1bf-113">Int64</span></span>  | <span data-ttu-id="0f1bf-114">组邮箱中使用的存储。</span><span class="sxs-lookup"><span data-stu-id="0f1bf-114">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="0f1bf-115">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="0f1bf-115">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="0f1bf-116">Int64</span><span class="sxs-lookup"><span data-stu-id="0f1bf-116">Int64</span></span>  | <span data-ttu-id="0f1bf-117">SharePoint 文档库中使用的存储。</span><span class="sxs-lookup"><span data-stu-id="0f1bf-117">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="0f1bf-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="0f1bf-118">reportDate</span></span>                | <span data-ttu-id="0f1bf-119">日期</span><span class="sxs-lookup"><span data-stu-id="0f1bf-119">Date</span></span>   | <span data-ttu-id="0f1bf-120">Exchange 和 SharePoint 使用的存储的快照日期。</span><span class="sxs-lookup"><span data-stu-id="0f1bf-120">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="0f1bf-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0f1bf-121">reportPeriod</span></span>              | <span data-ttu-id="0f1bf-122">String</span><span class="sxs-lookup"><span data-stu-id="0f1bf-122">String</span></span> | <span data-ttu-id="0f1bf-123">报告涵盖的天数。</span><span class="sxs-lookup"><span data-stu-id="0f1bf-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="0f1bf-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f1bf-124">JSON representation</span></span>

<span data-ttu-id="0f1bf-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f1bf-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailboxStorageUsedInBytes": 1024, 
  "siteStorageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


