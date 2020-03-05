---
title: office365ActivationsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 78c21f33352e5f6357638de8dacc4b628b6ef93b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522482"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="19054-103">office365ActivationsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="19054-103">office365ActivationsUserCounts resource type</span></span>

<span data-ttu-id="19054-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="19054-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="19054-105">属性</span><span class="sxs-lookup"><span data-stu-id="19054-105">Properties</span></span>

| <span data-ttu-id="19054-106">属性</span><span class="sxs-lookup"><span data-stu-id="19054-106">Property</span></span>                 | <span data-ttu-id="19054-107">类型</span><span class="sxs-lookup"><span data-stu-id="19054-107">Type</span></span>   | <span data-ttu-id="19054-108">说明</span><span class="sxs-lookup"><span data-stu-id="19054-108">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="19054-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="19054-109">reportRefreshDate</span></span>        | <span data-ttu-id="19054-110">日期</span><span class="sxs-lookup"><span data-stu-id="19054-110">Date</span></span>   | <span data-ttu-id="19054-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="19054-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="19054-112">productType</span><span class="sxs-lookup"><span data-stu-id="19054-112">productType</span></span>              | <span data-ttu-id="19054-113">String</span><span class="sxs-lookup"><span data-stu-id="19054-113">String</span></span> | <span data-ttu-id="19054-114">产品类型，如 "Office 365 专业增强版"、"Project Client" 或 "Visio Pro for Office 365"。</span><span class="sxs-lookup"><span data-stu-id="19054-114">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="19054-115">赋予</span><span class="sxs-lookup"><span data-stu-id="19054-115">assigned</span></span>                 | <span data-ttu-id="19054-116">Int64</span><span class="sxs-lookup"><span data-stu-id="19054-116">Int64</span></span>  | <span data-ttu-id="19054-117">已为产品许可证分配了用户数量。</span><span class="sxs-lookup"><span data-stu-id="19054-117">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="19054-118">已</span><span class="sxs-lookup"><span data-stu-id="19054-118">activated</span></span>                | <span data-ttu-id="19054-119">Int64</span><span class="sxs-lookup"><span data-stu-id="19054-119">Int64</span></span>  | <span data-ttu-id="19054-120">激活产品的用户数。</span><span class="sxs-lookup"><span data-stu-id="19054-120">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="19054-121">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="19054-121">sharedComputerActivation</span></span> | <span data-ttu-id="19054-122">Int64</span><span class="sxs-lookup"><span data-stu-id="19054-122">Int64</span></span>  | <span data-ttu-id="19054-123">在共享计算机上使用该产品的用户数。</span><span class="sxs-lookup"><span data-stu-id="19054-123">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="19054-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19054-124">JSON representation</span></span>

<span data-ttu-id="19054-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19054-125">The following is a JSON representation of the resource.</span></span>

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
