---
title: skypeForBusinessDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: c0134bedc15de07d89709a623b6a31a8f53ac5fe
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808611"
---
# <a name="skypeforbusinessdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="5ea33-103">skypeForBusinessDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="5ea33-103">skypeForBusinessDeviceUsageDistributionUserCounts resource type</span></span>

<span data-ttu-id="5ea33-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ea33-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="5ea33-105">属性</span><span class="sxs-lookup"><span data-stu-id="5ea33-105">Properties</span></span>

| <span data-ttu-id="5ea33-106">属性</span><span class="sxs-lookup"><span data-stu-id="5ea33-106">Property</span></span>          | <span data-ttu-id="5ea33-107">类型</span><span class="sxs-lookup"><span data-stu-id="5ea33-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5ea33-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5ea33-108">reportRefreshDate</span></span> | <span data-ttu-id="5ea33-109">日期</span><span class="sxs-lookup"><span data-stu-id="5ea33-109">Date</span></span>   |
| <span data-ttu-id="5ea33-110">时间</span><span class="sxs-lookup"><span data-stu-id="5ea33-110">windows</span></span>           | <span data-ttu-id="5ea33-111">Int64</span><span class="sxs-lookup"><span data-stu-id="5ea33-111">Int64</span></span>  |
| <span data-ttu-id="5ea33-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="5ea33-112">windowsPhone</span></span>      | <span data-ttu-id="5ea33-113">Int64</span><span class="sxs-lookup"><span data-stu-id="5ea33-113">Int64</span></span>  |
| <span data-ttu-id="5ea33-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="5ea33-114">androidPhone</span></span>      | <span data-ttu-id="5ea33-115">Int64</span><span class="sxs-lookup"><span data-stu-id="5ea33-115">Int64</span></span>  |
| <span data-ttu-id="5ea33-116">iPhone</span><span class="sxs-lookup"><span data-stu-id="5ea33-116">iPhone</span></span>            | <span data-ttu-id="5ea33-117">Int64</span><span class="sxs-lookup"><span data-stu-id="5ea33-117">Int64</span></span>  |
| <span data-ttu-id="5ea33-118">iPad</span><span class="sxs-lookup"><span data-stu-id="5ea33-118">iPad</span></span>              | <span data-ttu-id="5ea33-119">Int64</span><span class="sxs-lookup"><span data-stu-id="5ea33-119">Int64</span></span>  |
| <span data-ttu-id="5ea33-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5ea33-120">reportPeriod</span></span>      | <span data-ttu-id="5ea33-121">String</span><span class="sxs-lookup"><span data-stu-id="5ea33-121">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5ea33-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5ea33-122">JSON representation</span></span>

<span data-ttu-id="5ea33-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ea33-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date",
  "windows": 1024,
  "windowsPhone": 1024,
  "androidPhone": 1024,
  "iPhone": 1024,
  "iPad": 1024,
  "reportPeriod": "String"
}
```
