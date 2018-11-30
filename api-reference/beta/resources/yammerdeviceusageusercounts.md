---
title: yammerDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 7faec83d113da3f412c913177a717fdc69504310
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044969"
---
# <a name="yammerdeviceusageusercounts-resource-type"></a><span data-ttu-id="8ff69-103">yammerDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ff69-103">yammerDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8ff69-104">属性</span><span class="sxs-lookup"><span data-stu-id="8ff69-104">Properties</span></span>

| <span data-ttu-id="8ff69-105">属性</span><span class="sxs-lookup"><span data-stu-id="8ff69-105">Property</span></span>          | <span data-ttu-id="8ff69-106">类型</span><span class="sxs-lookup"><span data-stu-id="8ff69-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="8ff69-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8ff69-107">reportRefreshDate</span></span> | <span data-ttu-id="8ff69-108">日期</span><span class="sxs-lookup"><span data-stu-id="8ff69-108">Date</span></span>   |
| <span data-ttu-id="8ff69-109">web</span><span class="sxs-lookup"><span data-stu-id="8ff69-109">web</span></span>               | <span data-ttu-id="8ff69-110">Int32</span><span class="sxs-lookup"><span data-stu-id="8ff69-110">Int32</span></span>  |
| <span data-ttu-id="8ff69-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="8ff69-111">windowsPhone</span></span>      | <span data-ttu-id="8ff69-112">Int32</span><span class="sxs-lookup"><span data-stu-id="8ff69-112">Int32</span></span>  |
| <span data-ttu-id="8ff69-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="8ff69-113">androidPhone</span></span>      | <span data-ttu-id="8ff69-114">Int32</span><span class="sxs-lookup"><span data-stu-id="8ff69-114">Int32</span></span>  |
| <span data-ttu-id="8ff69-115">iPhone</span><span class="sxs-lookup"><span data-stu-id="8ff69-115">iPhone</span></span>            | <span data-ttu-id="8ff69-116">Int32</span><span class="sxs-lookup"><span data-stu-id="8ff69-116">Int32</span></span>  |
| <span data-ttu-id="8ff69-117">iPad</span><span class="sxs-lookup"><span data-stu-id="8ff69-117">iPad</span></span>              | <span data-ttu-id="8ff69-118">Int32</span><span class="sxs-lookup"><span data-stu-id="8ff69-118">Int32</span></span>  |
| <span data-ttu-id="8ff69-119">其他</span><span class="sxs-lookup"><span data-stu-id="8ff69-119">other</span></span>             | <span data-ttu-id="8ff69-120">Int32</span><span class="sxs-lookup"><span data-stu-id="8ff69-120">Int32</span></span>  |
| <span data-ttu-id="8ff69-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="8ff69-121">reportDate</span></span>        | <span data-ttu-id="8ff69-122">日期</span><span class="sxs-lookup"><span data-stu-id="8ff69-122">Date</span></span>   |
| <span data-ttu-id="8ff69-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8ff69-123">reportPeriod</span></span>      | <span data-ttu-id="8ff69-124">String</span><span class="sxs-lookup"><span data-stu-id="8ff69-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8ff69-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ff69-125">JSON representation</span></span>

<span data-ttu-id="8ff69-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ff69-126">The following is a JSON representation of the resource.</span></span>

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
