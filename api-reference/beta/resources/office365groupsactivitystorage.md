---
title: office365GroupsActivityStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 0b14e6981a193ad1698303d2762d0321de430b73
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092389"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="59a90-103">office365GroupsActivityStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="59a90-103">office365GroupsActivityStorage resource type</span></span>

<span data-ttu-id="59a90-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59a90-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="59a90-105">属性</span><span class="sxs-lookup"><span data-stu-id="59a90-105">Properties</span></span>

| <span data-ttu-id="59a90-106">属性</span><span class="sxs-lookup"><span data-stu-id="59a90-106">Property</span></span>                  | <span data-ttu-id="59a90-107">类型</span><span class="sxs-lookup"><span data-stu-id="59a90-107">Type</span></span>   | <span data-ttu-id="59a90-108">说明</span><span class="sxs-lookup"><span data-stu-id="59a90-108">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="59a90-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="59a90-109">reportRefreshDate</span></span>         | <span data-ttu-id="59a90-110">日期</span><span class="sxs-lookup"><span data-stu-id="59a90-110">Date</span></span>   | <span data-ttu-id="59a90-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="59a90-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="59a90-112">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="59a90-112">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="59a90-113">Int64</span><span class="sxs-lookup"><span data-stu-id="59a90-113">Int64</span></span>  | <span data-ttu-id="59a90-114">组邮箱中使用的存储。</span><span class="sxs-lookup"><span data-stu-id="59a90-114">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="59a90-115">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="59a90-115">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="59a90-116">Int64</span><span class="sxs-lookup"><span data-stu-id="59a90-116">Int64</span></span>  | <span data-ttu-id="59a90-117">SharePoint 文档库中使用的存储区。</span><span class="sxs-lookup"><span data-stu-id="59a90-117">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="59a90-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="59a90-118">reportDate</span></span>                | <span data-ttu-id="59a90-119">日期</span><span class="sxs-lookup"><span data-stu-id="59a90-119">Date</span></span>   | <span data-ttu-id="59a90-120">Exchange 和 SharePoint 使用的存储的快照日期。</span><span class="sxs-lookup"><span data-stu-id="59a90-120">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="59a90-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="59a90-121">reportPeriod</span></span>              | <span data-ttu-id="59a90-122">字符串</span><span class="sxs-lookup"><span data-stu-id="59a90-122">String</span></span> | <span data-ttu-id="59a90-123">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="59a90-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="59a90-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="59a90-124">JSON representation</span></span>

<span data-ttu-id="59a90-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59a90-125">The following is a JSON representation of the resource.</span></span>

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


