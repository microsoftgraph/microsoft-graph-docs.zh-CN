---
title: yammerActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 6ff2b347de77f91c96cb5f5be797eb70db0bbbee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042431"
---
# <a name="yammeractivitysummary-resource-type"></a><span data-ttu-id="17178-103">yammerActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="17178-103">yammerActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="17178-104">属性</span><span class="sxs-lookup"><span data-stu-id="17178-104">Properties</span></span>

| <span data-ttu-id="17178-105">属性</span><span class="sxs-lookup"><span data-stu-id="17178-105">Property</span></span>          | <span data-ttu-id="17178-106">类型</span><span class="sxs-lookup"><span data-stu-id="17178-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="17178-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="17178-107">reportRefreshDate</span></span> | <span data-ttu-id="17178-108">日期</span><span class="sxs-lookup"><span data-stu-id="17178-108">Date</span></span>   |
| <span data-ttu-id="17178-109">满意</span><span class="sxs-lookup"><span data-stu-id="17178-109">liked</span></span>             | <span data-ttu-id="17178-110">Int64</span><span class="sxs-lookup"><span data-stu-id="17178-110">Int64</span></span>  |
| <span data-ttu-id="17178-111">发布</span><span class="sxs-lookup"><span data-stu-id="17178-111">posted</span></span>            | <span data-ttu-id="17178-112">Int64</span><span class="sxs-lookup"><span data-stu-id="17178-112">Int64</span></span>  |
| <span data-ttu-id="17178-113">读取</span><span class="sxs-lookup"><span data-stu-id="17178-113">read</span></span>              | <span data-ttu-id="17178-114">Int64</span><span class="sxs-lookup"><span data-stu-id="17178-114">Int64</span></span>  |
| <span data-ttu-id="17178-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="17178-115">reportDate</span></span>        | <span data-ttu-id="17178-116">日期</span><span class="sxs-lookup"><span data-stu-id="17178-116">Date</span></span>   |
| <span data-ttu-id="17178-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="17178-117">reportPeriod</span></span>      | <span data-ttu-id="17178-118">String</span><span class="sxs-lookup"><span data-stu-id="17178-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="17178-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17178-119">JSON representation</span></span>

<span data-ttu-id="17178-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17178-120">The following is a JSON representation of the resource.</span></span>

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
