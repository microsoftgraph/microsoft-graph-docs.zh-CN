---
title: office365ActivationsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0d5ed2af02f429f5fd4d6e92b408d2e8e420f4d0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581511"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="77a81-103">office365ActivationsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="77a81-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="77a81-104">属性</span><span class="sxs-lookup"><span data-stu-id="77a81-104">Properties</span></span>

| <span data-ttu-id="77a81-105">属性</span><span class="sxs-lookup"><span data-stu-id="77a81-105">Property</span></span>                 | <span data-ttu-id="77a81-106">类型</span><span class="sxs-lookup"><span data-stu-id="77a81-106">Type</span></span>   | <span data-ttu-id="77a81-107">说明</span><span class="sxs-lookup"><span data-stu-id="77a81-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="77a81-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="77a81-108">reportRefreshDate</span></span>        | <span data-ttu-id="77a81-109">Date</span><span class="sxs-lookup"><span data-stu-id="77a81-109">Date</span></span>   | <span data-ttu-id="77a81-110">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="77a81-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="77a81-111">productType</span><span class="sxs-lookup"><span data-stu-id="77a81-111">productType</span></span>              | <span data-ttu-id="77a81-112">String</span><span class="sxs-lookup"><span data-stu-id="77a81-112">String</span></span> | <span data-ttu-id="77a81-113">产品类型, 如 "Office 365 专业增强版"、"Project Client" 或 "Visio Pro for Office 365"。</span><span class="sxs-lookup"><span data-stu-id="77a81-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="77a81-114">赋予</span><span class="sxs-lookup"><span data-stu-id="77a81-114">assigned</span></span>                 | <span data-ttu-id="77a81-115">Int64</span><span class="sxs-lookup"><span data-stu-id="77a81-115">Int64</span></span>  | <span data-ttu-id="77a81-116">已为产品许可证分配了用户数量。</span><span class="sxs-lookup"><span data-stu-id="77a81-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="77a81-117">已</span><span class="sxs-lookup"><span data-stu-id="77a81-117">activated</span></span>                | <span data-ttu-id="77a81-118">Int64</span><span class="sxs-lookup"><span data-stu-id="77a81-118">Int64</span></span>  | <span data-ttu-id="77a81-119">激活产品的用户数。</span><span class="sxs-lookup"><span data-stu-id="77a81-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="77a81-120">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="77a81-120">sharedComputerActivation</span></span> | <span data-ttu-id="77a81-121">Int64</span><span class="sxs-lookup"><span data-stu-id="77a81-121">Int64</span></span>  | <span data-ttu-id="77a81-122">在共享计算机上使用该产品的用户数。</span><span class="sxs-lookup"><span data-stu-id="77a81-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="77a81-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77a81-123">JSON representation</span></span>

<span data-ttu-id="77a81-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77a81-124">The following is a JSON representation of the resource.</span></span>

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
