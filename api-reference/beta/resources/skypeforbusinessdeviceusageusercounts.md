---
title: skypeForBusinessDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 3ae63d942ef21152e54f3bf5234d1b9d8df9649b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043113"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a><span data-ttu-id="2314d-103">skypeForBusinessDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="2314d-103">skypeForBusinessDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2314d-104">属性</span><span class="sxs-lookup"><span data-stu-id="2314d-104">Properties</span></span>

| <span data-ttu-id="2314d-105">属性</span><span class="sxs-lookup"><span data-stu-id="2314d-105">Property</span></span>          | <span data-ttu-id="2314d-106">类型</span><span class="sxs-lookup"><span data-stu-id="2314d-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="2314d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2314d-107">reportRefreshDate</span></span> | <span data-ttu-id="2314d-108">日期</span><span class="sxs-lookup"><span data-stu-id="2314d-108">Date</span></span>   |
| <span data-ttu-id="2314d-109">windows</span><span class="sxs-lookup"><span data-stu-id="2314d-109">windows</span></span>           | <span data-ttu-id="2314d-110">Int64</span><span class="sxs-lookup"><span data-stu-id="2314d-110">Int64</span></span>  |
| <span data-ttu-id="2314d-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="2314d-111">windowsPhone</span></span>      | <span data-ttu-id="2314d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2314d-112">Int64</span></span>  |
| <span data-ttu-id="2314d-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="2314d-113">androidPhone</span></span>      | <span data-ttu-id="2314d-114">Int64</span><span class="sxs-lookup"><span data-stu-id="2314d-114">Int64</span></span>  |
| <span data-ttu-id="2314d-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="2314d-115">iPhone</span></span>            | <span data-ttu-id="2314d-116">Int64</span><span class="sxs-lookup"><span data-stu-id="2314d-116">Int64</span></span>  |
| <span data-ttu-id="2314d-117">iPad</span><span class="sxs-lookup"><span data-stu-id="2314d-117">iPad</span></span>              | <span data-ttu-id="2314d-118">Int64</span><span class="sxs-lookup"><span data-stu-id="2314d-118">Int64</span></span>  |
| <span data-ttu-id="2314d-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="2314d-119">reportDate</span></span>        | <span data-ttu-id="2314d-120">日期</span><span class="sxs-lookup"><span data-stu-id="2314d-120">Date</span></span>   |
| <span data-ttu-id="2314d-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2314d-121">reportPeriod</span></span>      | <span data-ttu-id="2314d-122">String</span><span class="sxs-lookup"><span data-stu-id="2314d-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2314d-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2314d-123">JSON representation</span></span>

<span data-ttu-id="2314d-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2314d-124">The following is a JSON representation of the resource.</span></span>

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
