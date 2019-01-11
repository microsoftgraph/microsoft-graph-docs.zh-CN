---
title: yammerDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 0f4d543ec8a96eaa4e237a1db1367efdc625c4e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892013"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a><span data-ttu-id="fcbb4-103">yammerDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="fcbb4-103">yammerDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="fcbb4-104">属性</span><span class="sxs-lookup"><span data-stu-id="fcbb4-104">Properties</span></span>

| <span data-ttu-id="fcbb4-105">属性</span><span class="sxs-lookup"><span data-stu-id="fcbb4-105">Property</span></span>          | <span data-ttu-id="fcbb4-106">类型</span><span class="sxs-lookup"><span data-stu-id="fcbb4-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="fcbb4-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fcbb4-107">reportRefreshDate</span></span> | <span data-ttu-id="fcbb4-108">日期</span><span class="sxs-lookup"><span data-stu-id="fcbb4-108">Date</span></span>    |
| <span data-ttu-id="fcbb4-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fcbb4-109">userPrincipalName</span></span> | <span data-ttu-id="fcbb4-110">字符串</span><span class="sxs-lookup"><span data-stu-id="fcbb4-110">String</span></span>  |
| <span data-ttu-id="fcbb4-111">displayName</span><span class="sxs-lookup"><span data-stu-id="fcbb4-111">displayName</span></span>       | <span data-ttu-id="fcbb4-112">字符串</span><span class="sxs-lookup"><span data-stu-id="fcbb4-112">String</span></span>  |
| <span data-ttu-id="fcbb4-113">userState</span><span class="sxs-lookup"><span data-stu-id="fcbb4-113">userState</span></span>         | <span data-ttu-id="fcbb4-114">字符串</span><span class="sxs-lookup"><span data-stu-id="fcbb4-114">String</span></span>  |
| <span data-ttu-id="fcbb4-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="fcbb4-115">stateChangeDate</span></span>   | <span data-ttu-id="fcbb4-116">日期</span><span class="sxs-lookup"><span data-stu-id="fcbb4-116">Date</span></span>    |
| <span data-ttu-id="fcbb4-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="fcbb4-117">lastActivityDate</span></span>  | <span data-ttu-id="fcbb4-118">日期</span><span class="sxs-lookup"><span data-stu-id="fcbb4-118">Date</span></span>    |
| <span data-ttu-id="fcbb4-119">usedWeb</span><span class="sxs-lookup"><span data-stu-id="fcbb4-119">usedWeb</span></span>           | <span data-ttu-id="fcbb4-120">布尔</span><span class="sxs-lookup"><span data-stu-id="fcbb4-120">Boolean</span></span> |
| <span data-ttu-id="fcbb4-121">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="fcbb4-121">usedWindowsPhone</span></span>  | <span data-ttu-id="fcbb4-122">布尔</span><span class="sxs-lookup"><span data-stu-id="fcbb4-122">Boolean</span></span> |
| <span data-ttu-id="fcbb4-123">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="fcbb4-123">usedAndroidPhone</span></span>  | <span data-ttu-id="fcbb4-124">布尔</span><span class="sxs-lookup"><span data-stu-id="fcbb4-124">Boolean</span></span> |
| <span data-ttu-id="fcbb4-125">usediPhone</span><span class="sxs-lookup"><span data-stu-id="fcbb4-125">usediPhone</span></span>        | <span data-ttu-id="fcbb4-126">布尔</span><span class="sxs-lookup"><span data-stu-id="fcbb4-126">Boolean</span></span> |
| <span data-ttu-id="fcbb4-127">usediPad</span><span class="sxs-lookup"><span data-stu-id="fcbb4-127">usediPad</span></span>          | <span data-ttu-id="fcbb4-128">布尔</span><span class="sxs-lookup"><span data-stu-id="fcbb4-128">Boolean</span></span> |
| <span data-ttu-id="fcbb4-129">usedOthers</span><span class="sxs-lookup"><span data-stu-id="fcbb4-129">usedOthers</span></span>        | <span data-ttu-id="fcbb4-130">布尔</span><span class="sxs-lookup"><span data-stu-id="fcbb4-130">Boolean</span></span> |
| <span data-ttu-id="fcbb4-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fcbb4-131">reportPeriod</span></span>      | <span data-ttu-id="fcbb4-132">String</span><span class="sxs-lookup"><span data-stu-id="fcbb4-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="fcbb4-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fcbb4-133">JSON representation</span></span>

<span data-ttu-id="fcbb4-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fcbb4-134">The following is a JSON representation of the resource.</span></span>

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
