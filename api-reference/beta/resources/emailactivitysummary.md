---
title: emailActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9b3bb1d05c57874497d536de332f85b462335b5d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981870"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="91738-103">emailActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="91738-103">emailActivitySummary resource type</span></span>

<span data-ttu-id="91738-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91738-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="91738-105">属性</span><span class="sxs-lookup"><span data-stu-id="91738-105">Properties</span></span>

| <span data-ttu-id="91738-106">属性</span><span class="sxs-lookup"><span data-stu-id="91738-106">Property</span></span>          | <span data-ttu-id="91738-107">类型</span><span class="sxs-lookup"><span data-stu-id="91738-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="91738-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="91738-108">reportRefreshDate</span></span> | <span data-ttu-id="91738-109">日期</span><span class="sxs-lookup"><span data-stu-id="91738-109">Date</span></span>   |
| <span data-ttu-id="91738-110">发送</span><span class="sxs-lookup"><span data-stu-id="91738-110">send</span></span>              | <span data-ttu-id="91738-111">Int64</span><span class="sxs-lookup"><span data-stu-id="91738-111">Int64</span></span>  |
| <span data-ttu-id="91738-112">receive</span><span class="sxs-lookup"><span data-stu-id="91738-112">receive</span></span>           | <span data-ttu-id="91738-113">Int64</span><span class="sxs-lookup"><span data-stu-id="91738-113">Int64</span></span>  |
| <span data-ttu-id="91738-114">阅读</span><span class="sxs-lookup"><span data-stu-id="91738-114">read</span></span>              | <span data-ttu-id="91738-115">Int64</span><span class="sxs-lookup"><span data-stu-id="91738-115">Int64</span></span>  |
| <span data-ttu-id="91738-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="91738-116">reportDate</span></span>        | <span data-ttu-id="91738-117">日期</span><span class="sxs-lookup"><span data-stu-id="91738-117">Date</span></span>   |
| <span data-ttu-id="91738-118">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="91738-118">reportPeriod</span></span>      | <span data-ttu-id="91738-119">String</span><span class="sxs-lookup"><span data-stu-id="91738-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="91738-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91738-120">JSON representation</span></span>

<span data-ttu-id="91738-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91738-121">The following is a JSON representation of the resource.</span></span>

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


