---
title: yammerDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 878fe76fa65d5f8b12be382a161ace9271c6e415
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981537"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a><span data-ttu-id="df000-103">yammerDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="df000-103">yammerDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="df000-104">属性</span><span class="sxs-lookup"><span data-stu-id="df000-104">Properties</span></span>

| <span data-ttu-id="df000-105">属性</span><span class="sxs-lookup"><span data-stu-id="df000-105">Property</span></span>          | <span data-ttu-id="df000-106">类型</span><span class="sxs-lookup"><span data-stu-id="df000-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="df000-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="df000-107">reportRefreshDate</span></span> | <span data-ttu-id="df000-108">日期</span><span class="sxs-lookup"><span data-stu-id="df000-108">Date</span></span>   |
| <span data-ttu-id="df000-109">web</span><span class="sxs-lookup"><span data-stu-id="df000-109">web</span></span>               | <span data-ttu-id="df000-110">Int32</span><span class="sxs-lookup"><span data-stu-id="df000-110">Int32</span></span>  |
| <span data-ttu-id="df000-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="df000-111">windowsPhone</span></span>      | <span data-ttu-id="df000-112">Int32</span><span class="sxs-lookup"><span data-stu-id="df000-112">Int32</span></span>  |
| <span data-ttu-id="df000-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="df000-113">androidPhone</span></span>      | <span data-ttu-id="df000-114">Int32</span><span class="sxs-lookup"><span data-stu-id="df000-114">Int32</span></span>  |
| <span data-ttu-id="df000-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="df000-115">iPhone</span></span>            | <span data-ttu-id="df000-116">Int32</span><span class="sxs-lookup"><span data-stu-id="df000-116">Int32</span></span>  |
| <span data-ttu-id="df000-117">iPad</span><span class="sxs-lookup"><span data-stu-id="df000-117">iPad</span></span>              | <span data-ttu-id="df000-118">Int32</span><span class="sxs-lookup"><span data-stu-id="df000-118">Int32</span></span>  |
| <span data-ttu-id="df000-119">其他</span><span class="sxs-lookup"><span data-stu-id="df000-119">other</span></span>             | <span data-ttu-id="df000-120">Int32</span><span class="sxs-lookup"><span data-stu-id="df000-120">Int32</span></span>  |
| <span data-ttu-id="df000-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="df000-121">reportDate</span></span>        | <span data-ttu-id="df000-122">日期</span><span class="sxs-lookup"><span data-stu-id="df000-122">Date</span></span>   |
| <span data-ttu-id="df000-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="df000-123">reportPeriod</span></span>      | <span data-ttu-id="df000-124">String</span><span class="sxs-lookup"><span data-stu-id="df000-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="df000-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df000-125">JSON representation</span></span>

<span data-ttu-id="df000-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df000-126">The following is a JSON representation of the resource.</span></span>

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
