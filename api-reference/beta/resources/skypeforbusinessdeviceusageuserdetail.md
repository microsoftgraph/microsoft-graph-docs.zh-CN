---
title: skypeForBusinessDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 36cd6aba954206b60317520534284cd17f8d42e8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997527"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="20ae9-103">skypeForBusinessDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="20ae9-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

<span data-ttu-id="20ae9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20ae9-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="20ae9-105">属性</span><span class="sxs-lookup"><span data-stu-id="20ae9-105">Properties</span></span>

| <span data-ttu-id="20ae9-106">属性</span><span class="sxs-lookup"><span data-stu-id="20ae9-106">Property</span></span>          | <span data-ttu-id="20ae9-107">类型</span><span class="sxs-lookup"><span data-stu-id="20ae9-107">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="20ae9-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="20ae9-108">reportRefreshDate</span></span> | <span data-ttu-id="20ae9-109">日期</span><span class="sxs-lookup"><span data-stu-id="20ae9-109">Date</span></span>    |
| <span data-ttu-id="20ae9-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="20ae9-110">userPrincipalName</span></span> | <span data-ttu-id="20ae9-111">String</span><span class="sxs-lookup"><span data-stu-id="20ae9-111">String</span></span>  |
| <span data-ttu-id="20ae9-112">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="20ae9-112">lastActivityDate</span></span>  | <span data-ttu-id="20ae9-113">日期</span><span class="sxs-lookup"><span data-stu-id="20ae9-113">Date</span></span>    |
| <span data-ttu-id="20ae9-114">usedWindows</span><span class="sxs-lookup"><span data-stu-id="20ae9-114">usedWindows</span></span>       | <span data-ttu-id="20ae9-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="20ae9-115">Boolean</span></span> |
| <span data-ttu-id="20ae9-116">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="20ae9-116">usedWindowsPhone</span></span>  | <span data-ttu-id="20ae9-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="20ae9-117">Boolean</span></span> |
| <span data-ttu-id="20ae9-118">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="20ae9-118">usedAndroidPhone</span></span>  | <span data-ttu-id="20ae9-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="20ae9-119">Boolean</span></span> |
| <span data-ttu-id="20ae9-120">usediPhone</span><span class="sxs-lookup"><span data-stu-id="20ae9-120">usediPhone</span></span>        | <span data-ttu-id="20ae9-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="20ae9-121">Boolean</span></span> |
| <span data-ttu-id="20ae9-122">usediPad</span><span class="sxs-lookup"><span data-stu-id="20ae9-122">usediPad</span></span>          | <span data-ttu-id="20ae9-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="20ae9-123">Boolean</span></span> |
| <span data-ttu-id="20ae9-124">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="20ae9-124">reportPeriod</span></span>      | <span data-ttu-id="20ae9-125">String</span><span class="sxs-lookup"><span data-stu-id="20ae9-125">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="20ae9-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20ae9-126">JSON representation</span></span>

<span data-ttu-id="20ae9-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20ae9-127">The following is a JSON representation of the resource.</span></span>

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


