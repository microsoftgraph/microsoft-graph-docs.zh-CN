---
title: emailActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 84958874af09b31aafed694c1a62d080a5c798ce
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506669"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="485dc-103">emailActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="485dc-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="485dc-104">属性</span><span class="sxs-lookup"><span data-stu-id="485dc-104">Properties</span></span>

| <span data-ttu-id="485dc-105">属性</span><span class="sxs-lookup"><span data-stu-id="485dc-105">Property</span></span>          | <span data-ttu-id="485dc-106">类型</span><span class="sxs-lookup"><span data-stu-id="485dc-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="485dc-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="485dc-107">reportRefreshDate</span></span> | <span data-ttu-id="485dc-108">Date</span><span class="sxs-lookup"><span data-stu-id="485dc-108">Date</span></span>   |
| <span data-ttu-id="485dc-109">发送</span><span class="sxs-lookup"><span data-stu-id="485dc-109">send</span></span>              | <span data-ttu-id="485dc-110">Int64</span><span class="sxs-lookup"><span data-stu-id="485dc-110">Int64</span></span>  |
| <span data-ttu-id="485dc-111">享受</span><span class="sxs-lookup"><span data-stu-id="485dc-111">receive</span></span>           | <span data-ttu-id="485dc-112">Int64</span><span class="sxs-lookup"><span data-stu-id="485dc-112">Int64</span></span>  |
| <span data-ttu-id="485dc-113">自述</span><span class="sxs-lookup"><span data-stu-id="485dc-113">read</span></span>              | <span data-ttu-id="485dc-114">Int64</span><span class="sxs-lookup"><span data-stu-id="485dc-114">Int64</span></span>  |
| <span data-ttu-id="485dc-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="485dc-115">reportDate</span></span>        | <span data-ttu-id="485dc-116">Date</span><span class="sxs-lookup"><span data-stu-id="485dc-116">Date</span></span>   |
| <span data-ttu-id="485dc-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="485dc-117">reportPeriod</span></span>      | <span data-ttu-id="485dc-118">字符串</span><span class="sxs-lookup"><span data-stu-id="485dc-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="485dc-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="485dc-119">JSON representation</span></span>

<span data-ttu-id="485dc-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="485dc-120">The following is a JSON representation of the resource.</span></span>

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
