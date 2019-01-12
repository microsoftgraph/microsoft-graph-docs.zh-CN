---
title: emailActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 84958874af09b31aafed694c1a62d080a5c798ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990087"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="d1c5d-103">emailActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1c5d-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d1c5d-104">属性</span><span class="sxs-lookup"><span data-stu-id="d1c5d-104">Properties</span></span>

| <span data-ttu-id="d1c5d-105">属性</span><span class="sxs-lookup"><span data-stu-id="d1c5d-105">Property</span></span>          | <span data-ttu-id="d1c5d-106">类型</span><span class="sxs-lookup"><span data-stu-id="d1c5d-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="d1c5d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d1c5d-107">reportRefreshDate</span></span> | <span data-ttu-id="d1c5d-108">日期</span><span class="sxs-lookup"><span data-stu-id="d1c5d-108">Date</span></span>   |
| <span data-ttu-id="d1c5d-109">发送</span><span class="sxs-lookup"><span data-stu-id="d1c5d-109">send</span></span>              | <span data-ttu-id="d1c5d-110">Int64</span><span class="sxs-lookup"><span data-stu-id="d1c5d-110">Int64</span></span>  |
| <span data-ttu-id="d1c5d-111">接收</span><span class="sxs-lookup"><span data-stu-id="d1c5d-111">receive</span></span>           | <span data-ttu-id="d1c5d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="d1c5d-112">Int64</span></span>  |
| <span data-ttu-id="d1c5d-113">读取</span><span class="sxs-lookup"><span data-stu-id="d1c5d-113">read</span></span>              | <span data-ttu-id="d1c5d-114">Int64</span><span class="sxs-lookup"><span data-stu-id="d1c5d-114">Int64</span></span>  |
| <span data-ttu-id="d1c5d-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="d1c5d-115">reportDate</span></span>        | <span data-ttu-id="d1c5d-116">日期</span><span class="sxs-lookup"><span data-stu-id="d1c5d-116">Date</span></span>   |
| <span data-ttu-id="d1c5d-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d1c5d-117">reportPeriod</span></span>      | <span data-ttu-id="d1c5d-118">String</span><span class="sxs-lookup"><span data-stu-id="d1c5d-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d1c5d-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1c5d-119">JSON representation</span></span>

<span data-ttu-id="d1c5d-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1c5d-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "send": 1024, 
  "receive": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
