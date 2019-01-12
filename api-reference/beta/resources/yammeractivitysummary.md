---
title: yammerActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 974e234db31a7942b2b1dcbfff469288c32b6749
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974719"
---
# <a name="yammeractivitysummary-resource-type"></a><span data-ttu-id="810b4-103">yammerActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="810b4-103">yammerActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="810b4-104">属性</span><span class="sxs-lookup"><span data-stu-id="810b4-104">Properties</span></span>

| <span data-ttu-id="810b4-105">属性</span><span class="sxs-lookup"><span data-stu-id="810b4-105">Property</span></span>          | <span data-ttu-id="810b4-106">类型</span><span class="sxs-lookup"><span data-stu-id="810b4-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="810b4-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="810b4-107">reportRefreshDate</span></span> | <span data-ttu-id="810b4-108">日期</span><span class="sxs-lookup"><span data-stu-id="810b4-108">Date</span></span>   |
| <span data-ttu-id="810b4-109">满意</span><span class="sxs-lookup"><span data-stu-id="810b4-109">liked</span></span>             | <span data-ttu-id="810b4-110">Int64</span><span class="sxs-lookup"><span data-stu-id="810b4-110">Int64</span></span>  |
| <span data-ttu-id="810b4-111">发布</span><span class="sxs-lookup"><span data-stu-id="810b4-111">posted</span></span>            | <span data-ttu-id="810b4-112">Int64</span><span class="sxs-lookup"><span data-stu-id="810b4-112">Int64</span></span>  |
| <span data-ttu-id="810b4-113">读取</span><span class="sxs-lookup"><span data-stu-id="810b4-113">read</span></span>              | <span data-ttu-id="810b4-114">Int64</span><span class="sxs-lookup"><span data-stu-id="810b4-114">Int64</span></span>  |
| <span data-ttu-id="810b4-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="810b4-115">reportDate</span></span>        | <span data-ttu-id="810b4-116">日期</span><span class="sxs-lookup"><span data-stu-id="810b4-116">Date</span></span>   |
| <span data-ttu-id="810b4-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="810b4-117">reportPeriod</span></span>      | <span data-ttu-id="810b4-118">String</span><span class="sxs-lookup"><span data-stu-id="810b4-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="810b4-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="810b4-119">JSON representation</span></span>

<span data-ttu-id="810b4-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="810b4-120">The following is a JSON representation of the resource.</span></span>

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
