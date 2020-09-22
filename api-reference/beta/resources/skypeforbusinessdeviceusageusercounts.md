---
title: skypeForBusinessDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: e568e2bc396c5b7299441f8f8c513afcdada5c16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997534"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a><span data-ttu-id="00393-103">skypeForBusinessDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="00393-103">skypeForBusinessDeviceUsageUserCounts resource type</span></span>

<span data-ttu-id="00393-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00393-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="00393-105">属性</span><span class="sxs-lookup"><span data-stu-id="00393-105">Properties</span></span>

| <span data-ttu-id="00393-106">属性</span><span class="sxs-lookup"><span data-stu-id="00393-106">Property</span></span>          | <span data-ttu-id="00393-107">类型</span><span class="sxs-lookup"><span data-stu-id="00393-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="00393-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="00393-108">reportRefreshDate</span></span> | <span data-ttu-id="00393-109">日期</span><span class="sxs-lookup"><span data-stu-id="00393-109">Date</span></span>   |
| <span data-ttu-id="00393-110">时间</span><span class="sxs-lookup"><span data-stu-id="00393-110">windows</span></span>           | <span data-ttu-id="00393-111">Int64</span><span class="sxs-lookup"><span data-stu-id="00393-111">Int64</span></span>  |
| <span data-ttu-id="00393-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="00393-112">windowsPhone</span></span>      | <span data-ttu-id="00393-113">Int64</span><span class="sxs-lookup"><span data-stu-id="00393-113">Int64</span></span>  |
| <span data-ttu-id="00393-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="00393-114">androidPhone</span></span>      | <span data-ttu-id="00393-115">Int64</span><span class="sxs-lookup"><span data-stu-id="00393-115">Int64</span></span>  |
| <span data-ttu-id="00393-116">iPhone</span><span class="sxs-lookup"><span data-stu-id="00393-116">iPhone</span></span>            | <span data-ttu-id="00393-117">Int64</span><span class="sxs-lookup"><span data-stu-id="00393-117">Int64</span></span>  |
| <span data-ttu-id="00393-118">iPad</span><span class="sxs-lookup"><span data-stu-id="00393-118">iPad</span></span>              | <span data-ttu-id="00393-119">Int64</span><span class="sxs-lookup"><span data-stu-id="00393-119">Int64</span></span>  |
| <span data-ttu-id="00393-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="00393-120">reportDate</span></span>        | <span data-ttu-id="00393-121">日期</span><span class="sxs-lookup"><span data-stu-id="00393-121">Date</span></span>   |
| <span data-ttu-id="00393-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="00393-122">reportPeriod</span></span>      | <span data-ttu-id="00393-123">String</span><span class="sxs-lookup"><span data-stu-id="00393-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="00393-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00393-124">JSON representation</span></span>

<span data-ttu-id="00393-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00393-125">The following is a JSON representation of the resource.</span></span>

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


