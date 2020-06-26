---
title: office365ActivationsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: b8746d58b03b15a3118e8fc51a42e61e3c22cb78
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896803"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="dd9b9-103">office365ActivationsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd9b9-103">office365ActivationsUserCounts resource type</span></span>

<span data-ttu-id="dd9b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd9b9-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="dd9b9-105">属性</span><span class="sxs-lookup"><span data-stu-id="dd9b9-105">Properties</span></span>

| <span data-ttu-id="dd9b9-106">属性</span><span class="sxs-lookup"><span data-stu-id="dd9b9-106">Property</span></span>                 | <span data-ttu-id="dd9b9-107">类型</span><span class="sxs-lookup"><span data-stu-id="dd9b9-107">Type</span></span>   | <span data-ttu-id="dd9b9-108">说明</span><span class="sxs-lookup"><span data-stu-id="dd9b9-108">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="dd9b9-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="dd9b9-109">reportRefreshDate</span></span>        | <span data-ttu-id="dd9b9-110">日期</span><span class="sxs-lookup"><span data-stu-id="dd9b9-110">Date</span></span>   | <span data-ttu-id="dd9b9-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="dd9b9-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="dd9b9-112">productType</span><span class="sxs-lookup"><span data-stu-id="dd9b9-112">productType</span></span>              | <span data-ttu-id="dd9b9-113">String</span><span class="sxs-lookup"><span data-stu-id="dd9b9-113">String</span></span> | <span data-ttu-id="dd9b9-114">产品类型，如 "Microsoft 365 专业增强版" 或 "Project Client"。</span><span class="sxs-lookup"><span data-stu-id="dd9b9-114">The product type such as "Microsoft 365 ProPlus" or "Project Client".</span></span> |
| <span data-ttu-id="dd9b9-115">赋予</span><span class="sxs-lookup"><span data-stu-id="dd9b9-115">assigned</span></span>                 | <span data-ttu-id="dd9b9-116">Int64</span><span class="sxs-lookup"><span data-stu-id="dd9b9-116">Int64</span></span>  | <span data-ttu-id="dd9b9-117">已为产品许可证分配了用户数量。</span><span class="sxs-lookup"><span data-stu-id="dd9b9-117">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="dd9b9-118">已</span><span class="sxs-lookup"><span data-stu-id="dd9b9-118">activated</span></span>                | <span data-ttu-id="dd9b9-119">Int64</span><span class="sxs-lookup"><span data-stu-id="dd9b9-119">Int64</span></span>  | <span data-ttu-id="dd9b9-120">激活产品的用户数。</span><span class="sxs-lookup"><span data-stu-id="dd9b9-120">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="dd9b9-121">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="dd9b9-121">sharedComputerActivation</span></span> | <span data-ttu-id="dd9b9-122">Int64</span><span class="sxs-lookup"><span data-stu-id="dd9b9-122">Int64</span></span>  | <span data-ttu-id="dd9b9-123">在共享计算机上使用该产品的用户数。</span><span class="sxs-lookup"><span data-stu-id="dd9b9-123">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dd9b9-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd9b9-124">JSON representation</span></span>

<span data-ttu-id="dd9b9-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd9b9-125">The following is a JSON representation of the resource.</span></span>

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
