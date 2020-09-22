---
title: office365ActivationsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 21e18b35dc4e4ff639087617d679ae1583516026
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021222"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="7a2f6-103">office365ActivationsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a2f6-103">office365ActivationsUserCounts resource type</span></span>

<span data-ttu-id="7a2f6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a2f6-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="7a2f6-105">属性</span><span class="sxs-lookup"><span data-stu-id="7a2f6-105">Properties</span></span>

| <span data-ttu-id="7a2f6-106">属性</span><span class="sxs-lookup"><span data-stu-id="7a2f6-106">Property</span></span>                 | <span data-ttu-id="7a2f6-107">类型</span><span class="sxs-lookup"><span data-stu-id="7a2f6-107">Type</span></span>   | <span data-ttu-id="7a2f6-108">说明</span><span class="sxs-lookup"><span data-stu-id="7a2f6-108">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="7a2f6-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7a2f6-109">reportRefreshDate</span></span>        | <span data-ttu-id="7a2f6-110">日期</span><span class="sxs-lookup"><span data-stu-id="7a2f6-110">Date</span></span>   | <span data-ttu-id="7a2f6-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="7a2f6-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="7a2f6-112">productType</span><span class="sxs-lookup"><span data-stu-id="7a2f6-112">productType</span></span>              | <span data-ttu-id="7a2f6-113">String</span><span class="sxs-lookup"><span data-stu-id="7a2f6-113">String</span></span> | <span data-ttu-id="7a2f6-114">产品类型，如 "Microsoft 365 专业增强版" 或 "Project Client"。</span><span class="sxs-lookup"><span data-stu-id="7a2f6-114">The product type such as "Microsoft 365 ProPlus" or "Project Client".</span></span> |
| <span data-ttu-id="7a2f6-115">赋予</span><span class="sxs-lookup"><span data-stu-id="7a2f6-115">assigned</span></span>                 | <span data-ttu-id="7a2f6-116">Int64</span><span class="sxs-lookup"><span data-stu-id="7a2f6-116">Int64</span></span>  | <span data-ttu-id="7a2f6-117">已为产品许可证分配了用户数量。</span><span class="sxs-lookup"><span data-stu-id="7a2f6-117">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="7a2f6-118">已</span><span class="sxs-lookup"><span data-stu-id="7a2f6-118">activated</span></span>                | <span data-ttu-id="7a2f6-119">Int64</span><span class="sxs-lookup"><span data-stu-id="7a2f6-119">Int64</span></span>  | <span data-ttu-id="7a2f6-120">激活产品的用户数。</span><span class="sxs-lookup"><span data-stu-id="7a2f6-120">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="7a2f6-121">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="7a2f6-121">sharedComputerActivation</span></span> | <span data-ttu-id="7a2f6-122">Int64</span><span class="sxs-lookup"><span data-stu-id="7a2f6-122">Int64</span></span>  | <span data-ttu-id="7a2f6-123">在共享计算机上使用该产品的用户数。</span><span class="sxs-lookup"><span data-stu-id="7a2f6-123">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7a2f6-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a2f6-124">JSON representation</span></span>

<span data-ttu-id="7a2f6-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a2f6-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "assigned": 1024, 
  "activated": 1024,
  "sharedComputerActivation": 1024
}
```


