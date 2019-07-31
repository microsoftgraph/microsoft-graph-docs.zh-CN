---
title: office365ActivationsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 33339578f498460aacd24481f166ab717138f8fa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966564"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="5d291-103">office365ActivationsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="5d291-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5d291-104">属性</span><span class="sxs-lookup"><span data-stu-id="5d291-104">Properties</span></span>

| <span data-ttu-id="5d291-105">属性</span><span class="sxs-lookup"><span data-stu-id="5d291-105">Property</span></span>                 | <span data-ttu-id="5d291-106">类型</span><span class="sxs-lookup"><span data-stu-id="5d291-106">Type</span></span>   | <span data-ttu-id="5d291-107">说明</span><span class="sxs-lookup"><span data-stu-id="5d291-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="5d291-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5d291-108">reportRefreshDate</span></span>        | <span data-ttu-id="5d291-109">日期</span><span class="sxs-lookup"><span data-stu-id="5d291-109">Date</span></span>   | <span data-ttu-id="5d291-110">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="5d291-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="5d291-111">productType</span><span class="sxs-lookup"><span data-stu-id="5d291-111">productType</span></span>              | <span data-ttu-id="5d291-112">String</span><span class="sxs-lookup"><span data-stu-id="5d291-112">String</span></span> | <span data-ttu-id="5d291-113">产品类型, 如 "Office 365 专业增强版"、"Project Client" 或 "Visio Pro for Office 365"。</span><span class="sxs-lookup"><span data-stu-id="5d291-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="5d291-114">赋予</span><span class="sxs-lookup"><span data-stu-id="5d291-114">assigned</span></span>                 | <span data-ttu-id="5d291-115">Int64</span><span class="sxs-lookup"><span data-stu-id="5d291-115">Int64</span></span>  | <span data-ttu-id="5d291-116">已为产品许可证分配了用户数量。</span><span class="sxs-lookup"><span data-stu-id="5d291-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="5d291-117">已</span><span class="sxs-lookup"><span data-stu-id="5d291-117">activated</span></span>                | <span data-ttu-id="5d291-118">Int64</span><span class="sxs-lookup"><span data-stu-id="5d291-118">Int64</span></span>  | <span data-ttu-id="5d291-119">激活产品的用户数。</span><span class="sxs-lookup"><span data-stu-id="5d291-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="5d291-120">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="5d291-120">sharedComputerActivation</span></span> | <span data-ttu-id="5d291-121">Int64</span><span class="sxs-lookup"><span data-stu-id="5d291-121">Int64</span></span>  | <span data-ttu-id="5d291-122">在共享计算机上使用该产品的用户数。</span><span class="sxs-lookup"><span data-stu-id="5d291-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5d291-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5d291-123">JSON representation</span></span>

<span data-ttu-id="5d291-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d291-124">The following is a JSON representation of the resource.</span></span>

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
