---
title: emailActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6a8b6fd714b506404e7788a067fc655197f22ccc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440574"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="7c49a-103">emailActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c49a-103">emailActivitySummary resource type</span></span>

<span data-ttu-id="7c49a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c49a-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="7c49a-105">属性</span><span class="sxs-lookup"><span data-stu-id="7c49a-105">Properties</span></span>

| <span data-ttu-id="7c49a-106">属性</span><span class="sxs-lookup"><span data-stu-id="7c49a-106">Property</span></span>          | <span data-ttu-id="7c49a-107">类型</span><span class="sxs-lookup"><span data-stu-id="7c49a-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="7c49a-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7c49a-108">reportRefreshDate</span></span> | <span data-ttu-id="7c49a-109">日期</span><span class="sxs-lookup"><span data-stu-id="7c49a-109">Date</span></span>   |
| <span data-ttu-id="7c49a-110">发送</span><span class="sxs-lookup"><span data-stu-id="7c49a-110">send</span></span>              | <span data-ttu-id="7c49a-111">Int64</span><span class="sxs-lookup"><span data-stu-id="7c49a-111">Int64</span></span>  |
| <span data-ttu-id="7c49a-112">享受</span><span class="sxs-lookup"><span data-stu-id="7c49a-112">receive</span></span>           | <span data-ttu-id="7c49a-113">Int64</span><span class="sxs-lookup"><span data-stu-id="7c49a-113">Int64</span></span>  |
| <span data-ttu-id="7c49a-114">自述</span><span class="sxs-lookup"><span data-stu-id="7c49a-114">read</span></span>              | <span data-ttu-id="7c49a-115">Int64</span><span class="sxs-lookup"><span data-stu-id="7c49a-115">Int64</span></span>  |
| <span data-ttu-id="7c49a-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="7c49a-116">reportDate</span></span>        | <span data-ttu-id="7c49a-117">日期</span><span class="sxs-lookup"><span data-stu-id="7c49a-117">Date</span></span>   |
| <span data-ttu-id="7c49a-118">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7c49a-118">reportPeriod</span></span>      | <span data-ttu-id="7c49a-119">String</span><span class="sxs-lookup"><span data-stu-id="7c49a-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7c49a-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c49a-120">JSON representation</span></span>

<span data-ttu-id="7c49a-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c49a-121">The following is a JSON representation of the resource.</span></span>

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
