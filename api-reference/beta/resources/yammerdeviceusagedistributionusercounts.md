---
title: yammerDeviceUsageDistributionUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 6dcfef0f86913ee1afe98681b71f9210216dd416
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006975"
---
# <a name="yammerdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="6c245-103">yammerDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c245-103">yammerDeviceUsageDistributionUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6c245-104">属性</span><span class="sxs-lookup"><span data-stu-id="6c245-104">Properties</span></span>

| <span data-ttu-id="6c245-105">属性</span><span class="sxs-lookup"><span data-stu-id="6c245-105">Property</span></span>          | <span data-ttu-id="6c245-106">类型</span><span class="sxs-lookup"><span data-stu-id="6c245-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="6c245-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6c245-107">reportRefreshDate</span></span> | <span data-ttu-id="6c245-108">日期</span><span class="sxs-lookup"><span data-stu-id="6c245-108">Date</span></span>   |
| <span data-ttu-id="6c245-109">web</span><span class="sxs-lookup"><span data-stu-id="6c245-109">web</span></span>               | <span data-ttu-id="6c245-110">Int32</span><span class="sxs-lookup"><span data-stu-id="6c245-110">Int32</span></span>  |
| <span data-ttu-id="6c245-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="6c245-111">windowsPhone</span></span>      | <span data-ttu-id="6c245-112">Int32</span><span class="sxs-lookup"><span data-stu-id="6c245-112">Int32</span></span>  |
| <span data-ttu-id="6c245-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="6c245-113">androidPhone</span></span>      | <span data-ttu-id="6c245-114">Int32</span><span class="sxs-lookup"><span data-stu-id="6c245-114">Int32</span></span>  |
| <span data-ttu-id="6c245-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="6c245-115">iPhone</span></span>            | <span data-ttu-id="6c245-116">Int32</span><span class="sxs-lookup"><span data-stu-id="6c245-116">Int32</span></span>  |
| <span data-ttu-id="6c245-117">iPad</span><span class="sxs-lookup"><span data-stu-id="6c245-117">iPad</span></span>              | <span data-ttu-id="6c245-118">Int32</span><span class="sxs-lookup"><span data-stu-id="6c245-118">Int32</span></span>  |
| <span data-ttu-id="6c245-119">相互</span><span class="sxs-lookup"><span data-stu-id="6c245-119">other</span></span>             | <span data-ttu-id="6c245-120">Int32</span><span class="sxs-lookup"><span data-stu-id="6c245-120">Int32</span></span>  |
| <span data-ttu-id="6c245-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6c245-121">reportPeriod</span></span>      | <span data-ttu-id="6c245-122">String</span><span class="sxs-lookup"><span data-stu-id="6c245-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6c245-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c245-123">JSON representation</span></span>

<span data-ttu-id="6c245-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c245-124">The following is a JSON representation of the resource.</span></span>

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
