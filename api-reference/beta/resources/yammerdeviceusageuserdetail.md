---
title: yammerDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 982ebfc0de39bd956a4223e7bb0665ac73c42402
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518999"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a><span data-ttu-id="383db-103">yammerDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="383db-103">yammerDeviceUsageUserDetail resource type</span></span>

<span data-ttu-id="383db-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="383db-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="383db-105">属性</span><span class="sxs-lookup"><span data-stu-id="383db-105">Properties</span></span>

| <span data-ttu-id="383db-106">属性</span><span class="sxs-lookup"><span data-stu-id="383db-106">Property</span></span>          | <span data-ttu-id="383db-107">类型</span><span class="sxs-lookup"><span data-stu-id="383db-107">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="383db-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="383db-108">reportRefreshDate</span></span> | <span data-ttu-id="383db-109">日期</span><span class="sxs-lookup"><span data-stu-id="383db-109">Date</span></span>    |
| <span data-ttu-id="383db-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="383db-110">userPrincipalName</span></span> | <span data-ttu-id="383db-111">String</span><span class="sxs-lookup"><span data-stu-id="383db-111">String</span></span>  |
| <span data-ttu-id="383db-112">displayName</span><span class="sxs-lookup"><span data-stu-id="383db-112">displayName</span></span>       | <span data-ttu-id="383db-113">String</span><span class="sxs-lookup"><span data-stu-id="383db-113">String</span></span>  |
| <span data-ttu-id="383db-114">userState</span><span class="sxs-lookup"><span data-stu-id="383db-114">userState</span></span>         | <span data-ttu-id="383db-115">String</span><span class="sxs-lookup"><span data-stu-id="383db-115">String</span></span>  |
| <span data-ttu-id="383db-116">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="383db-116">stateChangeDate</span></span>   | <span data-ttu-id="383db-117">日期</span><span class="sxs-lookup"><span data-stu-id="383db-117">Date</span></span>    |
| <span data-ttu-id="383db-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="383db-118">lastActivityDate</span></span>  | <span data-ttu-id="383db-119">日期</span><span class="sxs-lookup"><span data-stu-id="383db-119">Date</span></span>    |
| <span data-ttu-id="383db-120">usedWeb</span><span class="sxs-lookup"><span data-stu-id="383db-120">usedWeb</span></span>           | <span data-ttu-id="383db-121">布尔</span><span class="sxs-lookup"><span data-stu-id="383db-121">Boolean</span></span> |
| <span data-ttu-id="383db-122">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="383db-122">usedWindowsPhone</span></span>  | <span data-ttu-id="383db-123">布尔</span><span class="sxs-lookup"><span data-stu-id="383db-123">Boolean</span></span> |
| <span data-ttu-id="383db-124">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="383db-124">usedAndroidPhone</span></span>  | <span data-ttu-id="383db-125">布尔</span><span class="sxs-lookup"><span data-stu-id="383db-125">Boolean</span></span> |
| <span data-ttu-id="383db-126">usediPhone</span><span class="sxs-lookup"><span data-stu-id="383db-126">usediPhone</span></span>        | <span data-ttu-id="383db-127">布尔</span><span class="sxs-lookup"><span data-stu-id="383db-127">Boolean</span></span> |
| <span data-ttu-id="383db-128">usediPad</span><span class="sxs-lookup"><span data-stu-id="383db-128">usediPad</span></span>          | <span data-ttu-id="383db-129">布尔</span><span class="sxs-lookup"><span data-stu-id="383db-129">Boolean</span></span> |
| <span data-ttu-id="383db-130">usedOthers</span><span class="sxs-lookup"><span data-stu-id="383db-130">usedOthers</span></span>        | <span data-ttu-id="383db-131">布尔</span><span class="sxs-lookup"><span data-stu-id="383db-131">Boolean</span></span> |
| <span data-ttu-id="383db-132">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="383db-132">reportPeriod</span></span>      | <span data-ttu-id="383db-133">String</span><span class="sxs-lookup"><span data-stu-id="383db-133">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="383db-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="383db-134">JSON representation</span></span>

<span data-ttu-id="383db-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="383db-135">The following is a JSON representation of the resource.</span></span>

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
