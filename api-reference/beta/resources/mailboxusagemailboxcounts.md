---
title: mailboxUsageMailboxCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e9da6a72c3c2d79323041e683702a7af2e4699c8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941308"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="6494a-103">mailboxUsageMailboxCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="6494a-103">mailboxUsageMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6494a-104">属性</span><span class="sxs-lookup"><span data-stu-id="6494a-104">Properties</span></span>

| <span data-ttu-id="6494a-105">属性</span><span class="sxs-lookup"><span data-stu-id="6494a-105">Property</span></span>          | <span data-ttu-id="6494a-106">类型</span><span class="sxs-lookup"><span data-stu-id="6494a-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="6494a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6494a-107">reportRefreshDate</span></span> | <span data-ttu-id="6494a-108">日期</span><span class="sxs-lookup"><span data-stu-id="6494a-108">Date</span></span>   |
| <span data-ttu-id="6494a-109">total</span><span class="sxs-lookup"><span data-stu-id="6494a-109">total</span></span>             | <span data-ttu-id="6494a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="6494a-110">Int64</span></span>  |
| <span data-ttu-id="6494a-111">活动</span><span class="sxs-lookup"><span data-stu-id="6494a-111">active</span></span>            | <span data-ttu-id="6494a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6494a-112">Int64</span></span>  |
| <span data-ttu-id="6494a-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="6494a-113">reportDate</span></span>        | <span data-ttu-id="6494a-114">日期</span><span class="sxs-lookup"><span data-stu-id="6494a-114">Date</span></span>   |
| <span data-ttu-id="6494a-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6494a-115">reportPeriod</span></span>      | <span data-ttu-id="6494a-116">String</span><span class="sxs-lookup"><span data-stu-id="6494a-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6494a-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6494a-117">JSON representation</span></span>

<span data-ttu-id="6494a-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6494a-118">The following is a JSON representation of the resource.</span></span>

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
