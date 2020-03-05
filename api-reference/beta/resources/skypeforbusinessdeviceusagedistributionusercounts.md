---
title: skypeForBusinessDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d7b6639b810507d7bee0c0a54f98cefae8d51677
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520420"
---
# <a name="skypeforbusinessdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="ca688-103">skypeForBusinessDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca688-103">skypeForBusinessDeviceUsageDistributionUserCounts resource type</span></span>

<span data-ttu-id="ca688-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ca688-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="ca688-105">属性</span><span class="sxs-lookup"><span data-stu-id="ca688-105">Properties</span></span>

| <span data-ttu-id="ca688-106">属性</span><span class="sxs-lookup"><span data-stu-id="ca688-106">Property</span></span>          | <span data-ttu-id="ca688-107">类型</span><span class="sxs-lookup"><span data-stu-id="ca688-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="ca688-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ca688-108">reportRefreshDate</span></span> | <span data-ttu-id="ca688-109">日期</span><span class="sxs-lookup"><span data-stu-id="ca688-109">Date</span></span>   |
| <span data-ttu-id="ca688-110">时间</span><span class="sxs-lookup"><span data-stu-id="ca688-110">windows</span></span>           | <span data-ttu-id="ca688-111">Int64</span><span class="sxs-lookup"><span data-stu-id="ca688-111">Int64</span></span>  |
| <span data-ttu-id="ca688-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="ca688-112">windowsPhone</span></span>      | <span data-ttu-id="ca688-113">Int64</span><span class="sxs-lookup"><span data-stu-id="ca688-113">Int64</span></span>  |
| <span data-ttu-id="ca688-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="ca688-114">androidPhone</span></span>      | <span data-ttu-id="ca688-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ca688-115">Int64</span></span>  |
| <span data-ttu-id="ca688-116">iPhone</span><span class="sxs-lookup"><span data-stu-id="ca688-116">iPhone</span></span>            | <span data-ttu-id="ca688-117">Int64</span><span class="sxs-lookup"><span data-stu-id="ca688-117">Int64</span></span>  |
| <span data-ttu-id="ca688-118">iPad</span><span class="sxs-lookup"><span data-stu-id="ca688-118">iPad</span></span>              | <span data-ttu-id="ca688-119">Int64</span><span class="sxs-lookup"><span data-stu-id="ca688-119">Int64</span></span>  |
| <span data-ttu-id="ca688-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ca688-120">reportPeriod</span></span>      | <span data-ttu-id="ca688-121">String</span><span class="sxs-lookup"><span data-stu-id="ca688-121">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ca688-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca688-122">JSON representation</span></span>

<span data-ttu-id="ca688-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca688-123">The following is a JSON representation of the resource.</span></span>

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
