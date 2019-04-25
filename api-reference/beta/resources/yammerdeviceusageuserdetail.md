---
title: yammerDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5fe3aa7fa9da243c9cc8f9b015ee85d779b84eb3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551426"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a><span data-ttu-id="ef1de-103">yammerDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="ef1de-103">yammerDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ef1de-104">属性</span><span class="sxs-lookup"><span data-stu-id="ef1de-104">Properties</span></span>

| <span data-ttu-id="ef1de-105">属性</span><span class="sxs-lookup"><span data-stu-id="ef1de-105">Property</span></span>          | <span data-ttu-id="ef1de-106">类型</span><span class="sxs-lookup"><span data-stu-id="ef1de-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="ef1de-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ef1de-107">reportRefreshDate</span></span> | <span data-ttu-id="ef1de-108">Date</span><span class="sxs-lookup"><span data-stu-id="ef1de-108">Date</span></span>    |
| <span data-ttu-id="ef1de-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ef1de-109">userPrincipalName</span></span> | <span data-ttu-id="ef1de-110">String</span><span class="sxs-lookup"><span data-stu-id="ef1de-110">String</span></span>  |
| <span data-ttu-id="ef1de-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ef1de-111">displayName</span></span>       | <span data-ttu-id="ef1de-112">String</span><span class="sxs-lookup"><span data-stu-id="ef1de-112">String</span></span>  |
| <span data-ttu-id="ef1de-113">userState</span><span class="sxs-lookup"><span data-stu-id="ef1de-113">userState</span></span>         | <span data-ttu-id="ef1de-114">String</span><span class="sxs-lookup"><span data-stu-id="ef1de-114">String</span></span>  |
| <span data-ttu-id="ef1de-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="ef1de-115">stateChangeDate</span></span>   | <span data-ttu-id="ef1de-116">Date</span><span class="sxs-lookup"><span data-stu-id="ef1de-116">Date</span></span>    |
| <span data-ttu-id="ef1de-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="ef1de-117">lastActivityDate</span></span>  | <span data-ttu-id="ef1de-118">Date</span><span class="sxs-lookup"><span data-stu-id="ef1de-118">Date</span></span>    |
| <span data-ttu-id="ef1de-119">usedWeb</span><span class="sxs-lookup"><span data-stu-id="ef1de-119">usedWeb</span></span>           | <span data-ttu-id="ef1de-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="ef1de-120">Boolean</span></span> |
| <span data-ttu-id="ef1de-121">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="ef1de-121">usedWindowsPhone</span></span>  | <span data-ttu-id="ef1de-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="ef1de-122">Boolean</span></span> |
| <span data-ttu-id="ef1de-123">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="ef1de-123">usedAndroidPhone</span></span>  | <span data-ttu-id="ef1de-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="ef1de-124">Boolean</span></span> |
| <span data-ttu-id="ef1de-125">usediPhone</span><span class="sxs-lookup"><span data-stu-id="ef1de-125">usediPhone</span></span>        | <span data-ttu-id="ef1de-126">布尔值</span><span class="sxs-lookup"><span data-stu-id="ef1de-126">Boolean</span></span> |
| <span data-ttu-id="ef1de-127">usediPad</span><span class="sxs-lookup"><span data-stu-id="ef1de-127">usediPad</span></span>          | <span data-ttu-id="ef1de-128">布尔值</span><span class="sxs-lookup"><span data-stu-id="ef1de-128">Boolean</span></span> |
| <span data-ttu-id="ef1de-129">usedOthers</span><span class="sxs-lookup"><span data-stu-id="ef1de-129">usedOthers</span></span>        | <span data-ttu-id="ef1de-130">布尔值</span><span class="sxs-lookup"><span data-stu-id="ef1de-130">Boolean</span></span> |
| <span data-ttu-id="ef1de-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ef1de-131">reportPeriod</span></span>      | <span data-ttu-id="ef1de-132">String</span><span class="sxs-lookup"><span data-stu-id="ef1de-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="ef1de-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ef1de-133">JSON representation</span></span>

<span data-ttu-id="ef1de-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef1de-134">The following is a JSON representation of the resource.</span></span>

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
