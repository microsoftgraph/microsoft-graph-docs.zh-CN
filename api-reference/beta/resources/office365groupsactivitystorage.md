---
title: office365GroupsActivityStorage 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 23ff4d112373f52c4c19d6631ac89bac22399b29
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048256"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="0355f-103">office365GroupsActivityStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="0355f-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="0355f-104">属性</span><span class="sxs-lookup"><span data-stu-id="0355f-104">Properties</span></span>

| <span data-ttu-id="0355f-105">属性</span><span class="sxs-lookup"><span data-stu-id="0355f-105">Property</span></span>                  | <span data-ttu-id="0355f-106">类型</span><span class="sxs-lookup"><span data-stu-id="0355f-106">Type</span></span>   | <span data-ttu-id="0355f-107">说明</span><span class="sxs-lookup"><span data-stu-id="0355f-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="0355f-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0355f-108">reportRefreshDate</span></span>         | <span data-ttu-id="0355f-109">日期</span><span class="sxs-lookup"><span data-stu-id="0355f-109">Date</span></span>   | <span data-ttu-id="0355f-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="0355f-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="0355f-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="0355f-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="0355f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="0355f-112">Int64</span></span>  | <span data-ttu-id="0355f-113">使用组邮箱中的存储。</span><span class="sxs-lookup"><span data-stu-id="0355f-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="0355f-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="0355f-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="0355f-115">Int64</span><span class="sxs-lookup"><span data-stu-id="0355f-115">Int64</span></span>  | <span data-ttu-id="0355f-116">在 SharePoint 文档库中使用的存储。</span><span class="sxs-lookup"><span data-stu-id="0355f-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="0355f-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="0355f-117">reportDate</span></span>                | <span data-ttu-id="0355f-118">日期</span><span class="sxs-lookup"><span data-stu-id="0355f-118">Date</span></span>   | <span data-ttu-id="0355f-119">Exchange 和 SharePoint 的快照日期用于存储。</span><span class="sxs-lookup"><span data-stu-id="0355f-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="0355f-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0355f-120">reportPeriod</span></span>              | <span data-ttu-id="0355f-121">字符串</span><span class="sxs-lookup"><span data-stu-id="0355f-121">String</span></span> | <span data-ttu-id="0355f-122">报告涵盖天数。</span><span class="sxs-lookup"><span data-stu-id="0355f-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="0355f-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0355f-123">JSON representation</span></span>

<span data-ttu-id="0355f-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0355f-124">The following is a JSON representation of the resource.</span></span>

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
