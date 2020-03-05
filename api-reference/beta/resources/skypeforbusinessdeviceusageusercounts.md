---
title: skypeForBusinessDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5a5149b3a247d4245f95d05f5e3f6b3e4be59e3d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520497"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a><span data-ttu-id="df385-103">skypeForBusinessDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="df385-103">skypeForBusinessDeviceUsageUserCounts resource type</span></span>

<span data-ttu-id="df385-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="df385-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="df385-105">属性</span><span class="sxs-lookup"><span data-stu-id="df385-105">Properties</span></span>

| <span data-ttu-id="df385-106">属性</span><span class="sxs-lookup"><span data-stu-id="df385-106">Property</span></span>          | <span data-ttu-id="df385-107">类型</span><span class="sxs-lookup"><span data-stu-id="df385-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="df385-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="df385-108">reportRefreshDate</span></span> | <span data-ttu-id="df385-109">日期</span><span class="sxs-lookup"><span data-stu-id="df385-109">Date</span></span>   |
| <span data-ttu-id="df385-110">时间</span><span class="sxs-lookup"><span data-stu-id="df385-110">windows</span></span>           | <span data-ttu-id="df385-111">Int64</span><span class="sxs-lookup"><span data-stu-id="df385-111">Int64</span></span>  |
| <span data-ttu-id="df385-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="df385-112">windowsPhone</span></span>      | <span data-ttu-id="df385-113">Int64</span><span class="sxs-lookup"><span data-stu-id="df385-113">Int64</span></span>  |
| <span data-ttu-id="df385-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="df385-114">androidPhone</span></span>      | <span data-ttu-id="df385-115">Int64</span><span class="sxs-lookup"><span data-stu-id="df385-115">Int64</span></span>  |
| <span data-ttu-id="df385-116">iPhone</span><span class="sxs-lookup"><span data-stu-id="df385-116">iPhone</span></span>            | <span data-ttu-id="df385-117">Int64</span><span class="sxs-lookup"><span data-stu-id="df385-117">Int64</span></span>  |
| <span data-ttu-id="df385-118">iPad</span><span class="sxs-lookup"><span data-stu-id="df385-118">iPad</span></span>              | <span data-ttu-id="df385-119">Int64</span><span class="sxs-lookup"><span data-stu-id="df385-119">Int64</span></span>  |
| <span data-ttu-id="df385-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="df385-120">reportDate</span></span>        | <span data-ttu-id="df385-121">日期</span><span class="sxs-lookup"><span data-stu-id="df385-121">Date</span></span>   |
| <span data-ttu-id="df385-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="df385-122">reportPeriod</span></span>      | <span data-ttu-id="df385-123">String</span><span class="sxs-lookup"><span data-stu-id="df385-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="df385-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df385-124">JSON representation</span></span>

<span data-ttu-id="df385-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df385-125">The following is a JSON representation of the resource.</span></span>

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
