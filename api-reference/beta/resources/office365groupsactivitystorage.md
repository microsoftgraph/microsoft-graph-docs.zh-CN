---
title: office365GroupsActivityStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: ba81621a819bb38f2d5d48e118729fc4476b5806
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522426"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="b80f9-103">office365GroupsActivityStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="b80f9-103">office365GroupsActivityStorage resource type</span></span>

<span data-ttu-id="b80f9-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b80f9-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="b80f9-105">属性</span><span class="sxs-lookup"><span data-stu-id="b80f9-105">Properties</span></span>

| <span data-ttu-id="b80f9-106">属性</span><span class="sxs-lookup"><span data-stu-id="b80f9-106">Property</span></span>                  | <span data-ttu-id="b80f9-107">类型</span><span class="sxs-lookup"><span data-stu-id="b80f9-107">Type</span></span>   | <span data-ttu-id="b80f9-108">说明</span><span class="sxs-lookup"><span data-stu-id="b80f9-108">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="b80f9-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b80f9-109">reportRefreshDate</span></span>         | <span data-ttu-id="b80f9-110">日期</span><span class="sxs-lookup"><span data-stu-id="b80f9-110">Date</span></span>   | <span data-ttu-id="b80f9-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="b80f9-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="b80f9-112">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="b80f9-112">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="b80f9-113">Int64</span><span class="sxs-lookup"><span data-stu-id="b80f9-113">Int64</span></span>  | <span data-ttu-id="b80f9-114">组邮箱中使用的存储。</span><span class="sxs-lookup"><span data-stu-id="b80f9-114">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="b80f9-115">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="b80f9-115">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="b80f9-116">Int64</span><span class="sxs-lookup"><span data-stu-id="b80f9-116">Int64</span></span>  | <span data-ttu-id="b80f9-117">SharePoint 文档库中使用的存储区。</span><span class="sxs-lookup"><span data-stu-id="b80f9-117">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="b80f9-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="b80f9-118">reportDate</span></span>                | <span data-ttu-id="b80f9-119">日期</span><span class="sxs-lookup"><span data-stu-id="b80f9-119">Date</span></span>   | <span data-ttu-id="b80f9-120">Exchange 和 SharePoint 使用的存储的快照日期。</span><span class="sxs-lookup"><span data-stu-id="b80f9-120">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="b80f9-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b80f9-121">reportPeriod</span></span>              | <span data-ttu-id="b80f9-122">String</span><span class="sxs-lookup"><span data-stu-id="b80f9-122">String</span></span> | <span data-ttu-id="b80f9-123">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="b80f9-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="b80f9-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b80f9-124">JSON representation</span></span>

<span data-ttu-id="b80f9-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b80f9-125">The following is a JSON representation of the resource.</span></span>

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
