---
title: emailActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 64c9468d79a93b6f82fff0f04206a0fb6e95e4fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972220"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="5f15f-103">emailActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f15f-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5f15f-104">属性</span><span class="sxs-lookup"><span data-stu-id="5f15f-104">Properties</span></span>

| <span data-ttu-id="5f15f-105">属性</span><span class="sxs-lookup"><span data-stu-id="5f15f-105">Property</span></span>          | <span data-ttu-id="5f15f-106">类型</span><span class="sxs-lookup"><span data-stu-id="5f15f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5f15f-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5f15f-107">reportRefreshDate</span></span> | <span data-ttu-id="5f15f-108">日期</span><span class="sxs-lookup"><span data-stu-id="5f15f-108">Date</span></span>   |
| <span data-ttu-id="5f15f-109">发送</span><span class="sxs-lookup"><span data-stu-id="5f15f-109">send</span></span>              | <span data-ttu-id="5f15f-110">Int64</span><span class="sxs-lookup"><span data-stu-id="5f15f-110">Int64</span></span>  |
| <span data-ttu-id="5f15f-111">享受</span><span class="sxs-lookup"><span data-stu-id="5f15f-111">receive</span></span>           | <span data-ttu-id="5f15f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5f15f-112">Int64</span></span>  |
| <span data-ttu-id="5f15f-113">自述</span><span class="sxs-lookup"><span data-stu-id="5f15f-113">read</span></span>              | <span data-ttu-id="5f15f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="5f15f-114">Int64</span></span>  |
| <span data-ttu-id="5f15f-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="5f15f-115">reportDate</span></span>        | <span data-ttu-id="5f15f-116">日期</span><span class="sxs-lookup"><span data-stu-id="5f15f-116">Date</span></span>   |
| <span data-ttu-id="5f15f-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5f15f-117">reportPeriod</span></span>      | <span data-ttu-id="5f15f-118">String</span><span class="sxs-lookup"><span data-stu-id="5f15f-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5f15f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f15f-119">JSON representation</span></span>

<span data-ttu-id="5f15f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f15f-120">The following is a JSON representation of the resource.</span></span>

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
