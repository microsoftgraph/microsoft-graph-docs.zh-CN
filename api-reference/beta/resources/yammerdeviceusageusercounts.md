---
title: yammerDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: ca8a1eaee94f7f125e2d2eb039561286737d58c6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519006"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a><span data-ttu-id="09cce-103">yammerDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="09cce-103">yammerDeviceUsageUserCounts resource type</span></span>

<span data-ttu-id="09cce-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="09cce-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="09cce-105">属性</span><span class="sxs-lookup"><span data-stu-id="09cce-105">Properties</span></span>

| <span data-ttu-id="09cce-106">属性</span><span class="sxs-lookup"><span data-stu-id="09cce-106">Property</span></span>          | <span data-ttu-id="09cce-107">类型</span><span class="sxs-lookup"><span data-stu-id="09cce-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="09cce-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="09cce-108">reportRefreshDate</span></span> | <span data-ttu-id="09cce-109">日期</span><span class="sxs-lookup"><span data-stu-id="09cce-109">Date</span></span>   |
| <span data-ttu-id="09cce-110">web</span><span class="sxs-lookup"><span data-stu-id="09cce-110">web</span></span>               | <span data-ttu-id="09cce-111">Int32</span><span class="sxs-lookup"><span data-stu-id="09cce-111">Int32</span></span>  |
| <span data-ttu-id="09cce-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="09cce-112">windowsPhone</span></span>      | <span data-ttu-id="09cce-113">Int32</span><span class="sxs-lookup"><span data-stu-id="09cce-113">Int32</span></span>  |
| <span data-ttu-id="09cce-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="09cce-114">androidPhone</span></span>      | <span data-ttu-id="09cce-115">Int32</span><span class="sxs-lookup"><span data-stu-id="09cce-115">Int32</span></span>  |
| <span data-ttu-id="09cce-116">iPhone</span><span class="sxs-lookup"><span data-stu-id="09cce-116">iPhone</span></span>            | <span data-ttu-id="09cce-117">Int32</span><span class="sxs-lookup"><span data-stu-id="09cce-117">Int32</span></span>  |
| <span data-ttu-id="09cce-118">iPad</span><span class="sxs-lookup"><span data-stu-id="09cce-118">iPad</span></span>              | <span data-ttu-id="09cce-119">Int32</span><span class="sxs-lookup"><span data-stu-id="09cce-119">Int32</span></span>  |
| <span data-ttu-id="09cce-120">相互</span><span class="sxs-lookup"><span data-stu-id="09cce-120">other</span></span>             | <span data-ttu-id="09cce-121">Int32</span><span class="sxs-lookup"><span data-stu-id="09cce-121">Int32</span></span>  |
| <span data-ttu-id="09cce-122">reportDate</span><span class="sxs-lookup"><span data-stu-id="09cce-122">reportDate</span></span>        | <span data-ttu-id="09cce-123">日期</span><span class="sxs-lookup"><span data-stu-id="09cce-123">Date</span></span>   |
| <span data-ttu-id="09cce-124">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="09cce-124">reportPeriod</span></span>      | <span data-ttu-id="09cce-125">String</span><span class="sxs-lookup"><span data-stu-id="09cce-125">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="09cce-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09cce-126">JSON representation</span></span>

<span data-ttu-id="09cce-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09cce-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "other": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
