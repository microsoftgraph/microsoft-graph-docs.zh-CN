---
title: mailboxUsageMailboxCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 7034e1f68eb1b119e0b4549e18500993a10cff04
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983550"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="2125d-103">mailboxUsageMailboxCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="2125d-103">mailboxUsageMailboxCounts resource type</span></span>

<span data-ttu-id="2125d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2125d-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="2125d-105">属性</span><span class="sxs-lookup"><span data-stu-id="2125d-105">Properties</span></span>

| <span data-ttu-id="2125d-106">属性</span><span class="sxs-lookup"><span data-stu-id="2125d-106">Property</span></span>          | <span data-ttu-id="2125d-107">类型</span><span class="sxs-lookup"><span data-stu-id="2125d-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="2125d-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2125d-108">reportRefreshDate</span></span> | <span data-ttu-id="2125d-109">日期</span><span class="sxs-lookup"><span data-stu-id="2125d-109">Date</span></span>   |
| <span data-ttu-id="2125d-110">total</span><span class="sxs-lookup"><span data-stu-id="2125d-110">total</span></span>             | <span data-ttu-id="2125d-111">Int64</span><span class="sxs-lookup"><span data-stu-id="2125d-111">Int64</span></span>  |
| <span data-ttu-id="2125d-112">active</span><span class="sxs-lookup"><span data-stu-id="2125d-112">active</span></span>            | <span data-ttu-id="2125d-113">Int64</span><span class="sxs-lookup"><span data-stu-id="2125d-113">Int64</span></span>  |
| <span data-ttu-id="2125d-114">reportDate</span><span class="sxs-lookup"><span data-stu-id="2125d-114">reportDate</span></span>        | <span data-ttu-id="2125d-115">日期</span><span class="sxs-lookup"><span data-stu-id="2125d-115">Date</span></span>   |
| <span data-ttu-id="2125d-116">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2125d-116">reportPeriod</span></span>      | <span data-ttu-id="2125d-117">String</span><span class="sxs-lookup"><span data-stu-id="2125d-117">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2125d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2125d-118">JSON representation</span></span>

<span data-ttu-id="2125d-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2125d-119">The following is a JSON representation of the resource.</span></span>

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


