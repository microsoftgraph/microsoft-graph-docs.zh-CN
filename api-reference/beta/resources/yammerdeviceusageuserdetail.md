---
title: yammerDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5fe3aa7fa9da243c9cc8f9b015ee85d779b84eb3
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574150"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a><span data-ttu-id="f8910-103">yammerDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="f8910-103">yammerDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f8910-104">属性</span><span class="sxs-lookup"><span data-stu-id="f8910-104">Properties</span></span>

| <span data-ttu-id="f8910-105">属性</span><span class="sxs-lookup"><span data-stu-id="f8910-105">Property</span></span>          | <span data-ttu-id="f8910-106">类型</span><span class="sxs-lookup"><span data-stu-id="f8910-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="f8910-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f8910-107">reportRefreshDate</span></span> | <span data-ttu-id="f8910-108">Date</span><span class="sxs-lookup"><span data-stu-id="f8910-108">Date</span></span>    |
| <span data-ttu-id="f8910-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f8910-109">userPrincipalName</span></span> | <span data-ttu-id="f8910-110">String</span><span class="sxs-lookup"><span data-stu-id="f8910-110">String</span></span>  |
| <span data-ttu-id="f8910-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f8910-111">displayName</span></span>       | <span data-ttu-id="f8910-112">String</span><span class="sxs-lookup"><span data-stu-id="f8910-112">String</span></span>  |
| <span data-ttu-id="f8910-113">userState</span><span class="sxs-lookup"><span data-stu-id="f8910-113">userState</span></span>         | <span data-ttu-id="f8910-114">String</span><span class="sxs-lookup"><span data-stu-id="f8910-114">String</span></span>  |
| <span data-ttu-id="f8910-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="f8910-115">stateChangeDate</span></span>   | <span data-ttu-id="f8910-116">Date</span><span class="sxs-lookup"><span data-stu-id="f8910-116">Date</span></span>    |
| <span data-ttu-id="f8910-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="f8910-117">lastActivityDate</span></span>  | <span data-ttu-id="f8910-118">Date</span><span class="sxs-lookup"><span data-stu-id="f8910-118">Date</span></span>    |
| <span data-ttu-id="f8910-119">usedWeb</span><span class="sxs-lookup"><span data-stu-id="f8910-119">usedWeb</span></span>           | <span data-ttu-id="f8910-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="f8910-120">Boolean</span></span> |
| <span data-ttu-id="f8910-121">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="f8910-121">usedWindowsPhone</span></span>  | <span data-ttu-id="f8910-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="f8910-122">Boolean</span></span> |
| <span data-ttu-id="f8910-123">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="f8910-123">usedAndroidPhone</span></span>  | <span data-ttu-id="f8910-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="f8910-124">Boolean</span></span> |
| <span data-ttu-id="f8910-125">usediPhone</span><span class="sxs-lookup"><span data-stu-id="f8910-125">usediPhone</span></span>        | <span data-ttu-id="f8910-126">布尔值</span><span class="sxs-lookup"><span data-stu-id="f8910-126">Boolean</span></span> |
| <span data-ttu-id="f8910-127">usediPad</span><span class="sxs-lookup"><span data-stu-id="f8910-127">usediPad</span></span>          | <span data-ttu-id="f8910-128">布尔值</span><span class="sxs-lookup"><span data-stu-id="f8910-128">Boolean</span></span> |
| <span data-ttu-id="f8910-129">usedOthers</span><span class="sxs-lookup"><span data-stu-id="f8910-129">usedOthers</span></span>        | <span data-ttu-id="f8910-130">布尔值</span><span class="sxs-lookup"><span data-stu-id="f8910-130">Boolean</span></span> |
| <span data-ttu-id="f8910-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f8910-131">reportPeriod</span></span>      | <span data-ttu-id="f8910-132">String</span><span class="sxs-lookup"><span data-stu-id="f8910-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="f8910-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8910-133">JSON representation</span></span>

<span data-ttu-id="f8910-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8910-134">The following is a JSON representation of the resource.</span></span>

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
