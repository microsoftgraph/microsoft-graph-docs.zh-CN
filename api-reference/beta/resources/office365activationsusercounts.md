---
title: office365ActivationsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 90d9d2d8616f166eb9d8b87967898daa0468db54
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048070"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="9fa8b-103">office365ActivationsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="9fa8b-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="9fa8b-104">属性</span><span class="sxs-lookup"><span data-stu-id="9fa8b-104">Properties</span></span>

| <span data-ttu-id="9fa8b-105">属性</span><span class="sxs-lookup"><span data-stu-id="9fa8b-105">Property</span></span>                 | <span data-ttu-id="9fa8b-106">类型</span><span class="sxs-lookup"><span data-stu-id="9fa8b-106">Type</span></span>   | <span data-ttu-id="9fa8b-107">说明</span><span class="sxs-lookup"><span data-stu-id="9fa8b-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="9fa8b-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="9fa8b-108">reportRefreshDate</span></span>        | <span data-ttu-id="9fa8b-109">日期</span><span class="sxs-lookup"><span data-stu-id="9fa8b-109">Date</span></span>   | <span data-ttu-id="9fa8b-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="9fa8b-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="9fa8b-111">productType</span><span class="sxs-lookup"><span data-stu-id="9fa8b-111">productType</span></span>              | <span data-ttu-id="9fa8b-112">字符串</span><span class="sxs-lookup"><span data-stu-id="9fa8b-112">String</span></span> | <span data-ttu-id="9fa8b-113">产品类型，如"Office 365 ProPlus"、"Project 客户端"或"Visio Pro for Office 365"。</span><span class="sxs-lookup"><span data-stu-id="9fa8b-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="9fa8b-114">分配</span><span class="sxs-lookup"><span data-stu-id="9fa8b-114">assigned</span></span>                 | <span data-ttu-id="9fa8b-115">Int64</span><span class="sxs-lookup"><span data-stu-id="9fa8b-115">Int64</span></span>  | <span data-ttu-id="9fa8b-116">产品许可证已分配的用户数。</span><span class="sxs-lookup"><span data-stu-id="9fa8b-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="9fa8b-117">激活</span><span class="sxs-lookup"><span data-stu-id="9fa8b-117">activated</span></span>                | <span data-ttu-id="9fa8b-118">Int64</span><span class="sxs-lookup"><span data-stu-id="9fa8b-118">Int64</span></span>  | <span data-ttu-id="9fa8b-119">已激活产品的用户数。</span><span class="sxs-lookup"><span data-stu-id="9fa8b-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="9fa8b-120">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="9fa8b-120">sharedComputerActivation</span></span> | <span data-ttu-id="9fa8b-121">Int64</span><span class="sxs-lookup"><span data-stu-id="9fa8b-121">Int64</span></span>  | <span data-ttu-id="9fa8b-122">共享计算机使用该产品的用户数。</span><span class="sxs-lookup"><span data-stu-id="9fa8b-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9fa8b-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9fa8b-123">JSON representation</span></span>

<span data-ttu-id="9fa8b-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9fa8b-124">The following is a JSON representation of the resource.</span></span>

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
