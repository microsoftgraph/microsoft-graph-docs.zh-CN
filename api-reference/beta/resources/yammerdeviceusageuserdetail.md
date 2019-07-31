---
title: yammerDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 083ace4b10b24e8e5de5d287ddf418d93658c879
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006976"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a><span data-ttu-id="7ba69-103">yammerDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ba69-103">yammerDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7ba69-104">属性</span><span class="sxs-lookup"><span data-stu-id="7ba69-104">Properties</span></span>

| <span data-ttu-id="7ba69-105">属性</span><span class="sxs-lookup"><span data-stu-id="7ba69-105">Property</span></span>          | <span data-ttu-id="7ba69-106">类型</span><span class="sxs-lookup"><span data-stu-id="7ba69-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="7ba69-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7ba69-107">reportRefreshDate</span></span> | <span data-ttu-id="7ba69-108">日期</span><span class="sxs-lookup"><span data-stu-id="7ba69-108">Date</span></span>    |
| <span data-ttu-id="7ba69-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7ba69-109">userPrincipalName</span></span> | <span data-ttu-id="7ba69-110">String</span><span class="sxs-lookup"><span data-stu-id="7ba69-110">String</span></span>  |
| <span data-ttu-id="7ba69-111">displayName</span><span class="sxs-lookup"><span data-stu-id="7ba69-111">displayName</span></span>       | <span data-ttu-id="7ba69-112">String</span><span class="sxs-lookup"><span data-stu-id="7ba69-112">String</span></span>  |
| <span data-ttu-id="7ba69-113">userState</span><span class="sxs-lookup"><span data-stu-id="7ba69-113">userState</span></span>         | <span data-ttu-id="7ba69-114">String</span><span class="sxs-lookup"><span data-stu-id="7ba69-114">String</span></span>  |
| <span data-ttu-id="7ba69-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="7ba69-115">stateChangeDate</span></span>   | <span data-ttu-id="7ba69-116">日期</span><span class="sxs-lookup"><span data-stu-id="7ba69-116">Date</span></span>    |
| <span data-ttu-id="7ba69-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="7ba69-117">lastActivityDate</span></span>  | <span data-ttu-id="7ba69-118">日期</span><span class="sxs-lookup"><span data-stu-id="7ba69-118">Date</span></span>    |
| <span data-ttu-id="7ba69-119">usedWeb</span><span class="sxs-lookup"><span data-stu-id="7ba69-119">usedWeb</span></span>           | <span data-ttu-id="7ba69-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ba69-120">Boolean</span></span> |
| <span data-ttu-id="7ba69-121">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="7ba69-121">usedWindowsPhone</span></span>  | <span data-ttu-id="7ba69-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ba69-122">Boolean</span></span> |
| <span data-ttu-id="7ba69-123">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="7ba69-123">usedAndroidPhone</span></span>  | <span data-ttu-id="7ba69-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ba69-124">Boolean</span></span> |
| <span data-ttu-id="7ba69-125">usediPhone</span><span class="sxs-lookup"><span data-stu-id="7ba69-125">usediPhone</span></span>        | <span data-ttu-id="7ba69-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ba69-126">Boolean</span></span> |
| <span data-ttu-id="7ba69-127">usediPad</span><span class="sxs-lookup"><span data-stu-id="7ba69-127">usediPad</span></span>          | <span data-ttu-id="7ba69-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ba69-128">Boolean</span></span> |
| <span data-ttu-id="7ba69-129">usedOthers</span><span class="sxs-lookup"><span data-stu-id="7ba69-129">usedOthers</span></span>        | <span data-ttu-id="7ba69-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ba69-130">Boolean</span></span> |
| <span data-ttu-id="7ba69-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7ba69-131">reportPeriod</span></span>      | <span data-ttu-id="7ba69-132">String</span><span class="sxs-lookup"><span data-stu-id="7ba69-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="7ba69-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ba69-133">JSON representation</span></span>

<span data-ttu-id="7ba69-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ba69-134">The following is a JSON representation of the resource.</span></span>

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
