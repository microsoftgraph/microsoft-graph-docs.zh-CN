---
title: office365GroupsActivityStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: a3168ad417f246017ba1018aca265ec0363c951e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009459"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="ae62d-103">office365GroupsActivityStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="ae62d-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ae62d-104">属性</span><span class="sxs-lookup"><span data-stu-id="ae62d-104">Properties</span></span>

| <span data-ttu-id="ae62d-105">属性</span><span class="sxs-lookup"><span data-stu-id="ae62d-105">Property</span></span>                  | <span data-ttu-id="ae62d-106">类型</span><span class="sxs-lookup"><span data-stu-id="ae62d-106">Type</span></span>   | <span data-ttu-id="ae62d-107">说明</span><span class="sxs-lookup"><span data-stu-id="ae62d-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="ae62d-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ae62d-108">reportRefreshDate</span></span>         | <span data-ttu-id="ae62d-109">日期</span><span class="sxs-lookup"><span data-stu-id="ae62d-109">Date</span></span>   | <span data-ttu-id="ae62d-110">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="ae62d-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="ae62d-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="ae62d-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="ae62d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ae62d-112">Int64</span></span>  | <span data-ttu-id="ae62d-113">组邮箱中使用的存储。</span><span class="sxs-lookup"><span data-stu-id="ae62d-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="ae62d-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="ae62d-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="ae62d-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ae62d-115">Int64</span></span>  | <span data-ttu-id="ae62d-116">SharePoint 文档库中使用的存储区。</span><span class="sxs-lookup"><span data-stu-id="ae62d-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="ae62d-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="ae62d-117">reportDate</span></span>                | <span data-ttu-id="ae62d-118">日期</span><span class="sxs-lookup"><span data-stu-id="ae62d-118">Date</span></span>   | <span data-ttu-id="ae62d-119">Exchange 和 SharePoint 使用的存储的快照日期。</span><span class="sxs-lookup"><span data-stu-id="ae62d-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="ae62d-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ae62d-120">reportPeriod</span></span>              | <span data-ttu-id="ae62d-121">String</span><span class="sxs-lookup"><span data-stu-id="ae62d-121">String</span></span> | <span data-ttu-id="ae62d-122">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="ae62d-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="ae62d-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae62d-123">JSON representation</span></span>

<span data-ttu-id="ae62d-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae62d-124">The following is a JSON representation of the resource.</span></span>

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
