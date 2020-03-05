---
title: skypeForBusinessDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 582c3483d4292f634385461508bf579834dfd12e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520406"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="7e1cb-103">skypeForBusinessDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e1cb-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

<span data-ttu-id="7e1cb-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7e1cb-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="7e1cb-105">属性</span><span class="sxs-lookup"><span data-stu-id="7e1cb-105">Properties</span></span>

| <span data-ttu-id="7e1cb-106">属性</span><span class="sxs-lookup"><span data-stu-id="7e1cb-106">Property</span></span>          | <span data-ttu-id="7e1cb-107">类型</span><span class="sxs-lookup"><span data-stu-id="7e1cb-107">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="7e1cb-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7e1cb-108">reportRefreshDate</span></span> | <span data-ttu-id="7e1cb-109">日期</span><span class="sxs-lookup"><span data-stu-id="7e1cb-109">Date</span></span>    |
| <span data-ttu-id="7e1cb-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7e1cb-110">userPrincipalName</span></span> | <span data-ttu-id="7e1cb-111">String</span><span class="sxs-lookup"><span data-stu-id="7e1cb-111">String</span></span>  |
| <span data-ttu-id="7e1cb-112">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="7e1cb-112">lastActivityDate</span></span>  | <span data-ttu-id="7e1cb-113">日期</span><span class="sxs-lookup"><span data-stu-id="7e1cb-113">Date</span></span>    |
| <span data-ttu-id="7e1cb-114">usedWindows</span><span class="sxs-lookup"><span data-stu-id="7e1cb-114">usedWindows</span></span>       | <span data-ttu-id="7e1cb-115">布尔</span><span class="sxs-lookup"><span data-stu-id="7e1cb-115">Boolean</span></span> |
| <span data-ttu-id="7e1cb-116">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="7e1cb-116">usedWindowsPhone</span></span>  | <span data-ttu-id="7e1cb-117">布尔</span><span class="sxs-lookup"><span data-stu-id="7e1cb-117">Boolean</span></span> |
| <span data-ttu-id="7e1cb-118">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="7e1cb-118">usedAndroidPhone</span></span>  | <span data-ttu-id="7e1cb-119">布尔</span><span class="sxs-lookup"><span data-stu-id="7e1cb-119">Boolean</span></span> |
| <span data-ttu-id="7e1cb-120">usediPhone</span><span class="sxs-lookup"><span data-stu-id="7e1cb-120">usediPhone</span></span>        | <span data-ttu-id="7e1cb-121">布尔</span><span class="sxs-lookup"><span data-stu-id="7e1cb-121">Boolean</span></span> |
| <span data-ttu-id="7e1cb-122">usediPad</span><span class="sxs-lookup"><span data-stu-id="7e1cb-122">usediPad</span></span>          | <span data-ttu-id="7e1cb-123">布尔</span><span class="sxs-lookup"><span data-stu-id="7e1cb-123">Boolean</span></span> |
| <span data-ttu-id="7e1cb-124">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7e1cb-124">reportPeriod</span></span>      | <span data-ttu-id="7e1cb-125">String</span><span class="sxs-lookup"><span data-stu-id="7e1cb-125">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="7e1cb-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e1cb-126">JSON representation</span></span>

<span data-ttu-id="7e1cb-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e1cb-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "usedWindows": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "reportPeriod": "String"
}
```
