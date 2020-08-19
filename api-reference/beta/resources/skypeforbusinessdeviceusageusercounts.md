---
title: skypeForBusinessDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 01867d92037f3bf80a7db2c25cc96a967ac560cd
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808709"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a><span data-ttu-id="816bd-103">skypeForBusinessDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="816bd-103">skypeForBusinessDeviceUsageUserCounts resource type</span></span>

<span data-ttu-id="816bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="816bd-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="816bd-105">属性</span><span class="sxs-lookup"><span data-stu-id="816bd-105">Properties</span></span>

| <span data-ttu-id="816bd-106">属性</span><span class="sxs-lookup"><span data-stu-id="816bd-106">Property</span></span>          | <span data-ttu-id="816bd-107">类型</span><span class="sxs-lookup"><span data-stu-id="816bd-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="816bd-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="816bd-108">reportRefreshDate</span></span> | <span data-ttu-id="816bd-109">日期</span><span class="sxs-lookup"><span data-stu-id="816bd-109">Date</span></span>   |
| <span data-ttu-id="816bd-110">时间</span><span class="sxs-lookup"><span data-stu-id="816bd-110">windows</span></span>           | <span data-ttu-id="816bd-111">Int64</span><span class="sxs-lookup"><span data-stu-id="816bd-111">Int64</span></span>  |
| <span data-ttu-id="816bd-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="816bd-112">windowsPhone</span></span>      | <span data-ttu-id="816bd-113">Int64</span><span class="sxs-lookup"><span data-stu-id="816bd-113">Int64</span></span>  |
| <span data-ttu-id="816bd-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="816bd-114">androidPhone</span></span>      | <span data-ttu-id="816bd-115">Int64</span><span class="sxs-lookup"><span data-stu-id="816bd-115">Int64</span></span>  |
| <span data-ttu-id="816bd-116">iPhone</span><span class="sxs-lookup"><span data-stu-id="816bd-116">iPhone</span></span>            | <span data-ttu-id="816bd-117">Int64</span><span class="sxs-lookup"><span data-stu-id="816bd-117">Int64</span></span>  |
| <span data-ttu-id="816bd-118">iPad</span><span class="sxs-lookup"><span data-stu-id="816bd-118">iPad</span></span>              | <span data-ttu-id="816bd-119">Int64</span><span class="sxs-lookup"><span data-stu-id="816bd-119">Int64</span></span>  |
| <span data-ttu-id="816bd-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="816bd-120">reportDate</span></span>        | <span data-ttu-id="816bd-121">日期</span><span class="sxs-lookup"><span data-stu-id="816bd-121">Date</span></span>   |
| <span data-ttu-id="816bd-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="816bd-122">reportPeriod</span></span>      | <span data-ttu-id="816bd-123">String</span><span class="sxs-lookup"><span data-stu-id="816bd-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="816bd-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="816bd-124">JSON representation</span></span>

<span data-ttu-id="816bd-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="816bd-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date",
  "windows": 1024,
  "windowsPhone": 1024,
  "androidPhone": 1024,
  "iPhone": 1024,
  "iPad": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```
