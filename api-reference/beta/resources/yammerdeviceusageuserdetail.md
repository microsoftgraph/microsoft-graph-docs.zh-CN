---
title: yammerDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 2b74222c1a636fac271268e228c8140e7d1cf33f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912006"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a><span data-ttu-id="dd29f-103">yammerDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd29f-103">yammerDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="dd29f-104">属性</span><span class="sxs-lookup"><span data-stu-id="dd29f-104">Properties</span></span>

| <span data-ttu-id="dd29f-105">属性</span><span class="sxs-lookup"><span data-stu-id="dd29f-105">Property</span></span>          | <span data-ttu-id="dd29f-106">类型</span><span class="sxs-lookup"><span data-stu-id="dd29f-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="dd29f-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="dd29f-107">reportRefreshDate</span></span> | <span data-ttu-id="dd29f-108">日期</span><span class="sxs-lookup"><span data-stu-id="dd29f-108">Date</span></span>    |
| <span data-ttu-id="dd29f-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dd29f-109">userPrincipalName</span></span> | <span data-ttu-id="dd29f-110">字符串</span><span class="sxs-lookup"><span data-stu-id="dd29f-110">String</span></span>  |
| <span data-ttu-id="dd29f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="dd29f-111">displayName</span></span>       | <span data-ttu-id="dd29f-112">字符串</span><span class="sxs-lookup"><span data-stu-id="dd29f-112">String</span></span>  |
| <span data-ttu-id="dd29f-113">userState</span><span class="sxs-lookup"><span data-stu-id="dd29f-113">userState</span></span>         | <span data-ttu-id="dd29f-114">字符串</span><span class="sxs-lookup"><span data-stu-id="dd29f-114">String</span></span>  |
| <span data-ttu-id="dd29f-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="dd29f-115">stateChangeDate</span></span>   | <span data-ttu-id="dd29f-116">日期</span><span class="sxs-lookup"><span data-stu-id="dd29f-116">Date</span></span>    |
| <span data-ttu-id="dd29f-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="dd29f-117">lastActivityDate</span></span>  | <span data-ttu-id="dd29f-118">日期</span><span class="sxs-lookup"><span data-stu-id="dd29f-118">Date</span></span>    |
| <span data-ttu-id="dd29f-119">usedWeb</span><span class="sxs-lookup"><span data-stu-id="dd29f-119">usedWeb</span></span>           | <span data-ttu-id="dd29f-120">布尔</span><span class="sxs-lookup"><span data-stu-id="dd29f-120">Boolean</span></span> |
| <span data-ttu-id="dd29f-121">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="dd29f-121">usedWindowsPhone</span></span>  | <span data-ttu-id="dd29f-122">布尔</span><span class="sxs-lookup"><span data-stu-id="dd29f-122">Boolean</span></span> |
| <span data-ttu-id="dd29f-123">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="dd29f-123">usedAndroidPhone</span></span>  | <span data-ttu-id="dd29f-124">布尔</span><span class="sxs-lookup"><span data-stu-id="dd29f-124">Boolean</span></span> |
| <span data-ttu-id="dd29f-125">usediPhone</span><span class="sxs-lookup"><span data-stu-id="dd29f-125">usediPhone</span></span>        | <span data-ttu-id="dd29f-126">布尔</span><span class="sxs-lookup"><span data-stu-id="dd29f-126">Boolean</span></span> |
| <span data-ttu-id="dd29f-127">usediPad</span><span class="sxs-lookup"><span data-stu-id="dd29f-127">usediPad</span></span>          | <span data-ttu-id="dd29f-128">布尔</span><span class="sxs-lookup"><span data-stu-id="dd29f-128">Boolean</span></span> |
| <span data-ttu-id="dd29f-129">usedOthers</span><span class="sxs-lookup"><span data-stu-id="dd29f-129">usedOthers</span></span>        | <span data-ttu-id="dd29f-130">布尔</span><span class="sxs-lookup"><span data-stu-id="dd29f-130">Boolean</span></span> |
| <span data-ttu-id="dd29f-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="dd29f-131">reportPeriod</span></span>      | <span data-ttu-id="dd29f-132">String</span><span class="sxs-lookup"><span data-stu-id="dd29f-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="dd29f-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd29f-133">JSON representation</span></span>

<span data-ttu-id="dd29f-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd29f-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "usedOthers": true, 
  "reportPeriod": "String"
}
```
