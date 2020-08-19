---
title: skypeForBusinessDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 50f37fdfd3441c256241b76ebcc6b144eb1486d7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811047"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="dd493-103">skypeForBusinessDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd493-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

<span data-ttu-id="dd493-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd493-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="dd493-105">属性</span><span class="sxs-lookup"><span data-stu-id="dd493-105">Properties</span></span>

| <span data-ttu-id="dd493-106">属性</span><span class="sxs-lookup"><span data-stu-id="dd493-106">Property</span></span>          | <span data-ttu-id="dd493-107">类型</span><span class="sxs-lookup"><span data-stu-id="dd493-107">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="dd493-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="dd493-108">reportRefreshDate</span></span> | <span data-ttu-id="dd493-109">日期</span><span class="sxs-lookup"><span data-stu-id="dd493-109">Date</span></span>    |
| <span data-ttu-id="dd493-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dd493-110">userPrincipalName</span></span> | <span data-ttu-id="dd493-111">String</span><span class="sxs-lookup"><span data-stu-id="dd493-111">String</span></span>  |
| <span data-ttu-id="dd493-112">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="dd493-112">lastActivityDate</span></span>  | <span data-ttu-id="dd493-113">日期</span><span class="sxs-lookup"><span data-stu-id="dd493-113">Date</span></span>    |
| <span data-ttu-id="dd493-114">usedWindows</span><span class="sxs-lookup"><span data-stu-id="dd493-114">usedWindows</span></span>       | <span data-ttu-id="dd493-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="dd493-115">Boolean</span></span> |
| <span data-ttu-id="dd493-116">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="dd493-116">usedWindowsPhone</span></span>  | <span data-ttu-id="dd493-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="dd493-117">Boolean</span></span> |
| <span data-ttu-id="dd493-118">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="dd493-118">usedAndroidPhone</span></span>  | <span data-ttu-id="dd493-119">布尔值</span><span class="sxs-lookup"><span data-stu-id="dd493-119">Boolean</span></span> |
| <span data-ttu-id="dd493-120">usediPhone</span><span class="sxs-lookup"><span data-stu-id="dd493-120">usediPhone</span></span>        | <span data-ttu-id="dd493-121">布尔值</span><span class="sxs-lookup"><span data-stu-id="dd493-121">Boolean</span></span> |
| <span data-ttu-id="dd493-122">usediPad</span><span class="sxs-lookup"><span data-stu-id="dd493-122">usediPad</span></span>          | <span data-ttu-id="dd493-123">布尔值</span><span class="sxs-lookup"><span data-stu-id="dd493-123">Boolean</span></span> |
| <span data-ttu-id="dd493-124">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="dd493-124">reportPeriod</span></span>      | <span data-ttu-id="dd493-125">String</span><span class="sxs-lookup"><span data-stu-id="dd493-125">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="dd493-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd493-126">JSON representation</span></span>

<span data-ttu-id="dd493-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd493-127">The following is a JSON representation of the resource.</span></span>

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
