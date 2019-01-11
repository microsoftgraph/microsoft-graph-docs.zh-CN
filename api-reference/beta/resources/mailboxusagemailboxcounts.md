---
title: mailboxUsageMailboxCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 4e18993590d6de893b78db511037eb28ec1cc0cb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814810"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="d7bc1-103">mailboxUsageMailboxCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7bc1-103">mailboxUsageMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d7bc1-104">属性</span><span class="sxs-lookup"><span data-stu-id="d7bc1-104">Properties</span></span>

| <span data-ttu-id="d7bc1-105">属性</span><span class="sxs-lookup"><span data-stu-id="d7bc1-105">Property</span></span>          | <span data-ttu-id="d7bc1-106">类型</span><span class="sxs-lookup"><span data-stu-id="d7bc1-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="d7bc1-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d7bc1-107">reportRefreshDate</span></span> | <span data-ttu-id="d7bc1-108">日期</span><span class="sxs-lookup"><span data-stu-id="d7bc1-108">Date</span></span>   |
| <span data-ttu-id="d7bc1-109">total</span><span class="sxs-lookup"><span data-stu-id="d7bc1-109">total</span></span>             | <span data-ttu-id="d7bc1-110">Int64</span><span class="sxs-lookup"><span data-stu-id="d7bc1-110">Int64</span></span>  |
| <span data-ttu-id="d7bc1-111">活动</span><span class="sxs-lookup"><span data-stu-id="d7bc1-111">active</span></span>            | <span data-ttu-id="d7bc1-112">Int64</span><span class="sxs-lookup"><span data-stu-id="d7bc1-112">Int64</span></span>  |
| <span data-ttu-id="d7bc1-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="d7bc1-113">reportDate</span></span>        | <span data-ttu-id="d7bc1-114">日期</span><span class="sxs-lookup"><span data-stu-id="d7bc1-114">Date</span></span>   |
| <span data-ttu-id="d7bc1-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d7bc1-115">reportPeriod</span></span>      | <span data-ttu-id="d7bc1-116">String</span><span class="sxs-lookup"><span data-stu-id="d7bc1-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d7bc1-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7bc1-117">JSON representation</span></span>

<span data-ttu-id="d7bc1-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7bc1-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageMailboxCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
