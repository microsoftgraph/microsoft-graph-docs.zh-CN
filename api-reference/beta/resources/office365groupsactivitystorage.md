---
title: office365GroupsActivityStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0485fd95046bc83350983bc1333dba83c79139d6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505548"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="b31e3-103">office365GroupsActivityStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="b31e3-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b31e3-104">属性</span><span class="sxs-lookup"><span data-stu-id="b31e3-104">Properties</span></span>

| <span data-ttu-id="b31e3-105">属性</span><span class="sxs-lookup"><span data-stu-id="b31e3-105">Property</span></span>                  | <span data-ttu-id="b31e3-106">类型</span><span class="sxs-lookup"><span data-stu-id="b31e3-106">Type</span></span>   | <span data-ttu-id="b31e3-107">说明</span><span class="sxs-lookup"><span data-stu-id="b31e3-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="b31e3-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b31e3-108">reportRefreshDate</span></span>         | <span data-ttu-id="b31e3-109">Date</span><span class="sxs-lookup"><span data-stu-id="b31e3-109">Date</span></span>   | <span data-ttu-id="b31e3-110">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="b31e3-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="b31e3-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="b31e3-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="b31e3-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b31e3-112">Int64</span></span>  | <span data-ttu-id="b31e3-113">组邮箱中使用的存储。</span><span class="sxs-lookup"><span data-stu-id="b31e3-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="b31e3-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="b31e3-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="b31e3-115">Int64</span><span class="sxs-lookup"><span data-stu-id="b31e3-115">Int64</span></span>  | <span data-ttu-id="b31e3-116">SharePoint 文档库中使用的存储区。</span><span class="sxs-lookup"><span data-stu-id="b31e3-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="b31e3-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="b31e3-117">reportDate</span></span>                | <span data-ttu-id="b31e3-118">Date</span><span class="sxs-lookup"><span data-stu-id="b31e3-118">Date</span></span>   | <span data-ttu-id="b31e3-119">Exchange 和 SharePoint 使用的存储的快照日期。</span><span class="sxs-lookup"><span data-stu-id="b31e3-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="b31e3-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b31e3-120">reportPeriod</span></span>              | <span data-ttu-id="b31e3-121">字符串</span><span class="sxs-lookup"><span data-stu-id="b31e3-121">String</span></span> | <span data-ttu-id="b31e3-122">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="b31e3-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="b31e3-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b31e3-123">JSON representation</span></span>

<span data-ttu-id="b31e3-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b31e3-124">The following is a JSON representation of the resource.</span></span>

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
