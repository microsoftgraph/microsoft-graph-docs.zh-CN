---
title: office365ActivationsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0d5ed2af02f429f5fd4d6e92b408d2e8e420f4d0
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574542"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="d26c8-103">office365ActivationsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="d26c8-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d26c8-104">属性</span><span class="sxs-lookup"><span data-stu-id="d26c8-104">Properties</span></span>

| <span data-ttu-id="d26c8-105">属性</span><span class="sxs-lookup"><span data-stu-id="d26c8-105">Property</span></span>                 | <span data-ttu-id="d26c8-106">类型</span><span class="sxs-lookup"><span data-stu-id="d26c8-106">Type</span></span>   | <span data-ttu-id="d26c8-107">说明</span><span class="sxs-lookup"><span data-stu-id="d26c8-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="d26c8-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d26c8-108">reportRefreshDate</span></span>        | <span data-ttu-id="d26c8-109">Date</span><span class="sxs-lookup"><span data-stu-id="d26c8-109">Date</span></span>   | <span data-ttu-id="d26c8-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="d26c8-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="d26c8-111">productType</span><span class="sxs-lookup"><span data-stu-id="d26c8-111">productType</span></span>              | <span data-ttu-id="d26c8-112">String</span><span class="sxs-lookup"><span data-stu-id="d26c8-112">String</span></span> | <span data-ttu-id="d26c8-113">产品类型，如"Office 365 ProPlus"、"Project 客户端"或"Visio Pro for Office 365"。</span><span class="sxs-lookup"><span data-stu-id="d26c8-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="d26c8-114">分配</span><span class="sxs-lookup"><span data-stu-id="d26c8-114">assigned</span></span>                 | <span data-ttu-id="d26c8-115">Int64</span><span class="sxs-lookup"><span data-stu-id="d26c8-115">Int64</span></span>  | <span data-ttu-id="d26c8-116">产品许可证已分配的用户数。</span><span class="sxs-lookup"><span data-stu-id="d26c8-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="d26c8-117">激活</span><span class="sxs-lookup"><span data-stu-id="d26c8-117">activated</span></span>                | <span data-ttu-id="d26c8-118">Int64</span><span class="sxs-lookup"><span data-stu-id="d26c8-118">Int64</span></span>  | <span data-ttu-id="d26c8-119">已激活产品的用户数。</span><span class="sxs-lookup"><span data-stu-id="d26c8-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="d26c8-120">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="d26c8-120">sharedComputerActivation</span></span> | <span data-ttu-id="d26c8-121">Int64</span><span class="sxs-lookup"><span data-stu-id="d26c8-121">Int64</span></span>  | <span data-ttu-id="d26c8-122">共享计算机使用该产品的用户数。</span><span class="sxs-lookup"><span data-stu-id="d26c8-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d26c8-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d26c8-123">JSON representation</span></span>

<span data-ttu-id="d26c8-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d26c8-124">The following is a JSON representation of the resource.</span></span>

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
