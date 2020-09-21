---
title: emailActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 78853954ef7c6fe4a191cbccefca350e628db210
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989589"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="c0146-103">emailActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="c0146-103">emailActivitySummary resource type</span></span>

<span data-ttu-id="c0146-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0146-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="c0146-105">属性</span><span class="sxs-lookup"><span data-stu-id="c0146-105">Properties</span></span>

| <span data-ttu-id="c0146-106">属性</span><span class="sxs-lookup"><span data-stu-id="c0146-106">Property</span></span>          | <span data-ttu-id="c0146-107">类型</span><span class="sxs-lookup"><span data-stu-id="c0146-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="c0146-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c0146-108">reportRefreshDate</span></span> | <span data-ttu-id="c0146-109">日期</span><span class="sxs-lookup"><span data-stu-id="c0146-109">Date</span></span>   |
| <span data-ttu-id="c0146-110">发送</span><span class="sxs-lookup"><span data-stu-id="c0146-110">send</span></span>              | <span data-ttu-id="c0146-111">Int64</span><span class="sxs-lookup"><span data-stu-id="c0146-111">Int64</span></span>  |
| <span data-ttu-id="c0146-112">享受</span><span class="sxs-lookup"><span data-stu-id="c0146-112">receive</span></span>           | <span data-ttu-id="c0146-113">Int64</span><span class="sxs-lookup"><span data-stu-id="c0146-113">Int64</span></span>  |
| <span data-ttu-id="c0146-114">阅读</span><span class="sxs-lookup"><span data-stu-id="c0146-114">read</span></span>              | <span data-ttu-id="c0146-115">Int64</span><span class="sxs-lookup"><span data-stu-id="c0146-115">Int64</span></span>  |
| <span data-ttu-id="c0146-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="c0146-116">reportDate</span></span>        | <span data-ttu-id="c0146-117">日期</span><span class="sxs-lookup"><span data-stu-id="c0146-117">Date</span></span>   |
| <span data-ttu-id="c0146-118">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c0146-118">reportPeriod</span></span>      | <span data-ttu-id="c0146-119">String</span><span class="sxs-lookup"><span data-stu-id="c0146-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c0146-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c0146-120">JSON representation</span></span>

<span data-ttu-id="c0146-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0146-121">The following is a JSON representation of the resource.</span></span>

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


