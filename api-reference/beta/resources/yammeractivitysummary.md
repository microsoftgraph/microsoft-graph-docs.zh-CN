---
title: yammerActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: fc7fc9679de3a655e76b6182f218010de7e39997
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519034"
---
# <a name="yammeractivitysummary-resource-type"></a><span data-ttu-id="85547-103">yammerActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="85547-103">yammerActivitySummary resource type</span></span>

<span data-ttu-id="85547-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="85547-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="85547-105">属性</span><span class="sxs-lookup"><span data-stu-id="85547-105">Properties</span></span>

| <span data-ttu-id="85547-106">属性</span><span class="sxs-lookup"><span data-stu-id="85547-106">Property</span></span>          | <span data-ttu-id="85547-107">类型</span><span class="sxs-lookup"><span data-stu-id="85547-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="85547-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="85547-108">reportRefreshDate</span></span> | <span data-ttu-id="85547-109">日期</span><span class="sxs-lookup"><span data-stu-id="85547-109">Date</span></span>   |
| <span data-ttu-id="85547-110">人</span><span class="sxs-lookup"><span data-stu-id="85547-110">liked</span></span>             | <span data-ttu-id="85547-111">Int64</span><span class="sxs-lookup"><span data-stu-id="85547-111">Int64</span></span>  |
| <span data-ttu-id="85547-112">发布</span><span class="sxs-lookup"><span data-stu-id="85547-112">posted</span></span>            | <span data-ttu-id="85547-113">Int64</span><span class="sxs-lookup"><span data-stu-id="85547-113">Int64</span></span>  |
| <span data-ttu-id="85547-114">自述</span><span class="sxs-lookup"><span data-stu-id="85547-114">read</span></span>              | <span data-ttu-id="85547-115">Int64</span><span class="sxs-lookup"><span data-stu-id="85547-115">Int64</span></span>  |
| <span data-ttu-id="85547-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="85547-116">reportDate</span></span>        | <span data-ttu-id="85547-117">日期</span><span class="sxs-lookup"><span data-stu-id="85547-117">Date</span></span>   |
| <span data-ttu-id="85547-118">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="85547-118">reportPeriod</span></span>      | <span data-ttu-id="85547-119">String</span><span class="sxs-lookup"><span data-stu-id="85547-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="85547-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85547-120">JSON representation</span></span>

<span data-ttu-id="85547-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85547-121">The following is a JSON representation of the resource.</span></span>

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
