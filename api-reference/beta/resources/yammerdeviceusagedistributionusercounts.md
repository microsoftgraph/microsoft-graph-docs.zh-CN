---
title: yammerDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: e90cc8d9a3a3b5178a30dd485eecc10be82478b5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519020"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="279b2-103">yammerDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="279b2-103">yammerDeviceUsageDistributionUserCounts resource type</span></span>

<span data-ttu-id="279b2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="279b2-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="279b2-105">属性</span><span class="sxs-lookup"><span data-stu-id="279b2-105">Properties</span></span>

| <span data-ttu-id="279b2-106">属性</span><span class="sxs-lookup"><span data-stu-id="279b2-106">Property</span></span>          | <span data-ttu-id="279b2-107">类型</span><span class="sxs-lookup"><span data-stu-id="279b2-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="279b2-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="279b2-108">reportRefreshDate</span></span> | <span data-ttu-id="279b2-109">日期</span><span class="sxs-lookup"><span data-stu-id="279b2-109">Date</span></span>   |
| <span data-ttu-id="279b2-110">web</span><span class="sxs-lookup"><span data-stu-id="279b2-110">web</span></span>               | <span data-ttu-id="279b2-111">Int32</span><span class="sxs-lookup"><span data-stu-id="279b2-111">Int32</span></span>  |
| <span data-ttu-id="279b2-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="279b2-112">windowsPhone</span></span>      | <span data-ttu-id="279b2-113">Int32</span><span class="sxs-lookup"><span data-stu-id="279b2-113">Int32</span></span>  |
| <span data-ttu-id="279b2-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="279b2-114">androidPhone</span></span>      | <span data-ttu-id="279b2-115">Int32</span><span class="sxs-lookup"><span data-stu-id="279b2-115">Int32</span></span>  |
| <span data-ttu-id="279b2-116">iPhone</span><span class="sxs-lookup"><span data-stu-id="279b2-116">iPhone</span></span>            | <span data-ttu-id="279b2-117">Int32</span><span class="sxs-lookup"><span data-stu-id="279b2-117">Int32</span></span>  |
| <span data-ttu-id="279b2-118">iPad</span><span class="sxs-lookup"><span data-stu-id="279b2-118">iPad</span></span>              | <span data-ttu-id="279b2-119">Int32</span><span class="sxs-lookup"><span data-stu-id="279b2-119">Int32</span></span>  |
| <span data-ttu-id="279b2-120">相互</span><span class="sxs-lookup"><span data-stu-id="279b2-120">other</span></span>             | <span data-ttu-id="279b2-121">Int32</span><span class="sxs-lookup"><span data-stu-id="279b2-121">Int32</span></span>  |
| <span data-ttu-id="279b2-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="279b2-122">reportPeriod</span></span>      | <span data-ttu-id="279b2-123">String</span><span class="sxs-lookup"><span data-stu-id="279b2-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="279b2-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="279b2-124">JSON representation</span></span>

<span data-ttu-id="279b2-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="279b2-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageDistributionUserCounts"
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
  "reportPeriod": "String"
}
```
