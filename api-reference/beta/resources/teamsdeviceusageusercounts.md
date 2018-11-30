---
title: teamsDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 9640af67efc18f0a70c636673169e884ce82d971
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048763"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="de755-103">teamsDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="de755-103">teamsDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="de755-104">属性</span><span class="sxs-lookup"><span data-stu-id="de755-104">Properties</span></span>

| <span data-ttu-id="de755-105">属性</span><span class="sxs-lookup"><span data-stu-id="de755-105">Property</span></span>          | <span data-ttu-id="de755-106">类型</span><span class="sxs-lookup"><span data-stu-id="de755-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="de755-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="de755-107">reportRefreshDate</span></span> | <span data-ttu-id="de755-108">日期</span><span class="sxs-lookup"><span data-stu-id="de755-108">Date</span></span>   |
| <span data-ttu-id="de755-109">web</span><span class="sxs-lookup"><span data-stu-id="de755-109">web</span></span>               | <span data-ttu-id="de755-110">Int64</span><span class="sxs-lookup"><span data-stu-id="de755-110">Int64</span></span>  |
| <span data-ttu-id="de755-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="de755-111">windowsPhone</span></span>      | <span data-ttu-id="de755-112">Int64</span><span class="sxs-lookup"><span data-stu-id="de755-112">Int64</span></span>  |
| <span data-ttu-id="de755-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="de755-113">androidPhone</span></span>      | <span data-ttu-id="de755-114">Int64</span><span class="sxs-lookup"><span data-stu-id="de755-114">Int64</span></span>  |
| <span data-ttu-id="de755-115">ios</span><span class="sxs-lookup"><span data-stu-id="de755-115">ios</span></span>               | <span data-ttu-id="de755-116">Int64</span><span class="sxs-lookup"><span data-stu-id="de755-116">Int64</span></span>  |
| <span data-ttu-id="de755-117">mac</span><span class="sxs-lookup"><span data-stu-id="de755-117">mac</span></span>               | <span data-ttu-id="de755-118">Int64</span><span class="sxs-lookup"><span data-stu-id="de755-118">Int64</span></span>  |
| <span data-ttu-id="de755-119">windows</span><span class="sxs-lookup"><span data-stu-id="de755-119">windows</span></span>           | <span data-ttu-id="de755-120">Int64</span><span class="sxs-lookup"><span data-stu-id="de755-120">Int64</span></span>  |
| <span data-ttu-id="de755-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="de755-121">reportDate</span></span>        | <span data-ttu-id="de755-122">日期</span><span class="sxs-lookup"><span data-stu-id="de755-122">Date</span></span>   |
| <span data-ttu-id="de755-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="de755-123">reportPeriod</span></span>      | <span data-ttu-id="de755-124">String</span><span class="sxs-lookup"><span data-stu-id="de755-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="de755-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de755-125">JSON representation</span></span>

<span data-ttu-id="de755-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de755-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
