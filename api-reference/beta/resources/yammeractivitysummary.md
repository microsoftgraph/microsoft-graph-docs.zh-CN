---
title: yammerActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c220ce211c9c6b61d41aa5773e3bcc01697f4e31
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574164"
---
# <a name="yammeractivitysummary-resource-type"></a><span data-ttu-id="dfda3-103">yammerActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="dfda3-103">yammerActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="dfda3-104">属性</span><span class="sxs-lookup"><span data-stu-id="dfda3-104">Properties</span></span>

| <span data-ttu-id="dfda3-105">属性</span><span class="sxs-lookup"><span data-stu-id="dfda3-105">Property</span></span>          | <span data-ttu-id="dfda3-106">类型</span><span class="sxs-lookup"><span data-stu-id="dfda3-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="dfda3-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="dfda3-107">reportRefreshDate</span></span> | <span data-ttu-id="dfda3-108">Date</span><span class="sxs-lookup"><span data-stu-id="dfda3-108">Date</span></span>   |
| <span data-ttu-id="dfda3-109">满意</span><span class="sxs-lookup"><span data-stu-id="dfda3-109">liked</span></span>             | <span data-ttu-id="dfda3-110">Int64</span><span class="sxs-lookup"><span data-stu-id="dfda3-110">Int64</span></span>  |
| <span data-ttu-id="dfda3-111">发布</span><span class="sxs-lookup"><span data-stu-id="dfda3-111">posted</span></span>            | <span data-ttu-id="dfda3-112">Int64</span><span class="sxs-lookup"><span data-stu-id="dfda3-112">Int64</span></span>  |
| <span data-ttu-id="dfda3-113">读取</span><span class="sxs-lookup"><span data-stu-id="dfda3-113">read</span></span>              | <span data-ttu-id="dfda3-114">Int64</span><span class="sxs-lookup"><span data-stu-id="dfda3-114">Int64</span></span>  |
| <span data-ttu-id="dfda3-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="dfda3-115">reportDate</span></span>        | <span data-ttu-id="dfda3-116">Date</span><span class="sxs-lookup"><span data-stu-id="dfda3-116">Date</span></span>   |
| <span data-ttu-id="dfda3-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="dfda3-117">reportPeriod</span></span>      | <span data-ttu-id="dfda3-118">String</span><span class="sxs-lookup"><span data-stu-id="dfda3-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dfda3-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dfda3-119">JSON representation</span></span>

<span data-ttu-id="dfda3-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfda3-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "liked": 1024, 
  "posted": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
