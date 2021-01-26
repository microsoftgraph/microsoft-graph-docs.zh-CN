---
title: yammerDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: b7a6617b82c16fb297b684801e11876cf8178b0d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982353"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a><span data-ttu-id="9d396-103">yammerDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d396-103">yammerDeviceUsageUserDetail resource type</span></span>

<span data-ttu-id="9d396-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d396-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="9d396-105">属性</span><span class="sxs-lookup"><span data-stu-id="9d396-105">Properties</span></span>

| <span data-ttu-id="9d396-106">属性</span><span class="sxs-lookup"><span data-stu-id="9d396-106">Property</span></span>          | <span data-ttu-id="9d396-107">类型</span><span class="sxs-lookup"><span data-stu-id="9d396-107">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="9d396-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="9d396-108">reportRefreshDate</span></span> | <span data-ttu-id="9d396-109">日期</span><span class="sxs-lookup"><span data-stu-id="9d396-109">Date</span></span>    |
| <span data-ttu-id="9d396-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9d396-110">userPrincipalName</span></span> | <span data-ttu-id="9d396-111">String</span><span class="sxs-lookup"><span data-stu-id="9d396-111">String</span></span>  |
| <span data-ttu-id="9d396-112">displayName</span><span class="sxs-lookup"><span data-stu-id="9d396-112">displayName</span></span>       | <span data-ttu-id="9d396-113">String</span><span class="sxs-lookup"><span data-stu-id="9d396-113">String</span></span>  |
| <span data-ttu-id="9d396-114">userState</span><span class="sxs-lookup"><span data-stu-id="9d396-114">userState</span></span>         | <span data-ttu-id="9d396-115">String</span><span class="sxs-lookup"><span data-stu-id="9d396-115">String</span></span>  |
| <span data-ttu-id="9d396-116">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="9d396-116">stateChangeDate</span></span>   | <span data-ttu-id="9d396-117">日期</span><span class="sxs-lookup"><span data-stu-id="9d396-117">Date</span></span>    |
| <span data-ttu-id="9d396-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="9d396-118">lastActivityDate</span></span>  | <span data-ttu-id="9d396-119">日期</span><span class="sxs-lookup"><span data-stu-id="9d396-119">Date</span></span>    |
| <span data-ttu-id="9d396-120">usedWeb</span><span class="sxs-lookup"><span data-stu-id="9d396-120">usedWeb</span></span>           | <span data-ttu-id="9d396-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d396-121">Boolean</span></span> |
| <span data-ttu-id="9d396-122">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="9d396-122">usedWindowsPhone</span></span>  | <span data-ttu-id="9d396-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d396-123">Boolean</span></span> |
| <span data-ttu-id="9d396-124">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="9d396-124">usedAndroidPhone</span></span>  | <span data-ttu-id="9d396-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d396-125">Boolean</span></span> |
| <span data-ttu-id="9d396-126">usediPhone</span><span class="sxs-lookup"><span data-stu-id="9d396-126">usediPhone</span></span>        | <span data-ttu-id="9d396-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d396-127">Boolean</span></span> |
| <span data-ttu-id="9d396-128">usediPad</span><span class="sxs-lookup"><span data-stu-id="9d396-128">usediPad</span></span>          | <span data-ttu-id="9d396-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d396-129">Boolean</span></span> |
| <span data-ttu-id="9d396-130">usedOthers</span><span class="sxs-lookup"><span data-stu-id="9d396-130">usedOthers</span></span>        | <span data-ttu-id="9d396-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d396-131">Boolean</span></span> |
| <span data-ttu-id="9d396-132">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="9d396-132">reportPeriod</span></span>      | <span data-ttu-id="9d396-133">String</span><span class="sxs-lookup"><span data-stu-id="9d396-133">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="9d396-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d396-134">JSON representation</span></span>

<span data-ttu-id="9d396-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d396-135">The following is a JSON representation of the resource.</span></span>

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


