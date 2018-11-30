---
title: skypeForBusinessDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 1534051455d805cf3bc9fabbb301ffde5be85ad9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049495"
---
# <a name="skypeforbusinessdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="4a316-103">skypeForBusinessDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a316-103">skypeForBusinessDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4a316-104">属性</span><span class="sxs-lookup"><span data-stu-id="4a316-104">Properties</span></span>

| <span data-ttu-id="4a316-105">属性</span><span class="sxs-lookup"><span data-stu-id="4a316-105">Property</span></span>          | <span data-ttu-id="4a316-106">类型</span><span class="sxs-lookup"><span data-stu-id="4a316-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="4a316-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4a316-107">reportRefreshDate</span></span> | <span data-ttu-id="4a316-108">日期</span><span class="sxs-lookup"><span data-stu-id="4a316-108">Date</span></span>   |
| <span data-ttu-id="4a316-109">windows</span><span class="sxs-lookup"><span data-stu-id="4a316-109">windows</span></span>           | <span data-ttu-id="4a316-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4a316-110">Int64</span></span>  |
| <span data-ttu-id="4a316-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="4a316-111">windowsPhone</span></span>      | <span data-ttu-id="4a316-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4a316-112">Int64</span></span>  |
| <span data-ttu-id="4a316-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="4a316-113">androidPhone</span></span>      | <span data-ttu-id="4a316-114">Int64</span><span class="sxs-lookup"><span data-stu-id="4a316-114">Int64</span></span>  |
| <span data-ttu-id="4a316-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="4a316-115">iPhone</span></span>            | <span data-ttu-id="4a316-116">Int64</span><span class="sxs-lookup"><span data-stu-id="4a316-116">Int64</span></span>  |
| <span data-ttu-id="4a316-117">iPad</span><span class="sxs-lookup"><span data-stu-id="4a316-117">iPad</span></span>              | <span data-ttu-id="4a316-118">Int64</span><span class="sxs-lookup"><span data-stu-id="4a316-118">Int64</span></span>  |
| <span data-ttu-id="4a316-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4a316-119">reportPeriod</span></span>      | <span data-ttu-id="4a316-120">String</span><span class="sxs-lookup"><span data-stu-id="4a316-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4a316-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a316-121">JSON representation</span></span>

<span data-ttu-id="4a316-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a316-122">The following is a JSON representation of the resource.</span></span>

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
