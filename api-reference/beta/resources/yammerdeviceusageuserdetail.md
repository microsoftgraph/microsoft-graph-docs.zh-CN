---
title: yammerDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 8812b61d974815fd1cdf1bbe1549a21193e5a2f4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048765"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a><span data-ttu-id="370cd-103">yammerDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="370cd-103">yammerDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="370cd-104">属性</span><span class="sxs-lookup"><span data-stu-id="370cd-104">Properties</span></span>

| <span data-ttu-id="370cd-105">属性</span><span class="sxs-lookup"><span data-stu-id="370cd-105">Property</span></span>          | <span data-ttu-id="370cd-106">类型</span><span class="sxs-lookup"><span data-stu-id="370cd-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="370cd-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="370cd-107">reportRefreshDate</span></span> | <span data-ttu-id="370cd-108">日期</span><span class="sxs-lookup"><span data-stu-id="370cd-108">Date</span></span>    |
| <span data-ttu-id="370cd-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="370cd-109">userPrincipalName</span></span> | <span data-ttu-id="370cd-110">字符串</span><span class="sxs-lookup"><span data-stu-id="370cd-110">String</span></span>  |
| <span data-ttu-id="370cd-111">displayName</span><span class="sxs-lookup"><span data-stu-id="370cd-111">displayName</span></span>       | <span data-ttu-id="370cd-112">字符串</span><span class="sxs-lookup"><span data-stu-id="370cd-112">String</span></span>  |
| <span data-ttu-id="370cd-113">userState</span><span class="sxs-lookup"><span data-stu-id="370cd-113">userState</span></span>         | <span data-ttu-id="370cd-114">字符串</span><span class="sxs-lookup"><span data-stu-id="370cd-114">String</span></span>  |
| <span data-ttu-id="370cd-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="370cd-115">stateChangeDate</span></span>   | <span data-ttu-id="370cd-116">日期</span><span class="sxs-lookup"><span data-stu-id="370cd-116">Date</span></span>    |
| <span data-ttu-id="370cd-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="370cd-117">lastActivityDate</span></span>  | <span data-ttu-id="370cd-118">日期</span><span class="sxs-lookup"><span data-stu-id="370cd-118">Date</span></span>    |
| <span data-ttu-id="370cd-119">usedWeb</span><span class="sxs-lookup"><span data-stu-id="370cd-119">usedWeb</span></span>           | <span data-ttu-id="370cd-120">布尔</span><span class="sxs-lookup"><span data-stu-id="370cd-120">Boolean</span></span> |
| <span data-ttu-id="370cd-121">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="370cd-121">usedWindowsPhone</span></span>  | <span data-ttu-id="370cd-122">布尔</span><span class="sxs-lookup"><span data-stu-id="370cd-122">Boolean</span></span> |
| <span data-ttu-id="370cd-123">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="370cd-123">usedAndroidPhone</span></span>  | <span data-ttu-id="370cd-124">布尔</span><span class="sxs-lookup"><span data-stu-id="370cd-124">Boolean</span></span> |
| <span data-ttu-id="370cd-125">usediPhone</span><span class="sxs-lookup"><span data-stu-id="370cd-125">usediPhone</span></span>        | <span data-ttu-id="370cd-126">布尔</span><span class="sxs-lookup"><span data-stu-id="370cd-126">Boolean</span></span> |
| <span data-ttu-id="370cd-127">usediPad</span><span class="sxs-lookup"><span data-stu-id="370cd-127">usediPad</span></span>          | <span data-ttu-id="370cd-128">布尔</span><span class="sxs-lookup"><span data-stu-id="370cd-128">Boolean</span></span> |
| <span data-ttu-id="370cd-129">usedOthers</span><span class="sxs-lookup"><span data-stu-id="370cd-129">usedOthers</span></span>        | <span data-ttu-id="370cd-130">布尔</span><span class="sxs-lookup"><span data-stu-id="370cd-130">Boolean</span></span> |
| <span data-ttu-id="370cd-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="370cd-131">reportPeriod</span></span>      | <span data-ttu-id="370cd-132">String</span><span class="sxs-lookup"><span data-stu-id="370cd-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="370cd-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="370cd-133">JSON representation</span></span>

<span data-ttu-id="370cd-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="370cd-134">The following is a JSON representation of the resource.</span></span>

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
