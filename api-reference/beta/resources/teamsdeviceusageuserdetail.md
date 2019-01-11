---
title: teamsDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 06e2cea1154c608b61642b07adbd96aae1710903
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807103"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="a784e-103">teamsDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="a784e-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a784e-104">属性</span><span class="sxs-lookup"><span data-stu-id="a784e-104">Properties</span></span>

| <span data-ttu-id="a784e-105">属性</span><span class="sxs-lookup"><span data-stu-id="a784e-105">Property</span></span>          | <span data-ttu-id="a784e-106">类型</span><span class="sxs-lookup"><span data-stu-id="a784e-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="a784e-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a784e-107">reportRefreshDate</span></span> | <span data-ttu-id="a784e-108">日期</span><span class="sxs-lookup"><span data-stu-id="a784e-108">Date</span></span>    |
| <span data-ttu-id="a784e-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a784e-109">userPrincipalName</span></span> | <span data-ttu-id="a784e-110">字符串</span><span class="sxs-lookup"><span data-stu-id="a784e-110">String</span></span>  |
| <span data-ttu-id="a784e-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="a784e-111">lastActivityDate</span></span>  | <span data-ttu-id="a784e-112">日期</span><span class="sxs-lookup"><span data-stu-id="a784e-112">Date</span></span>    |
| <span data-ttu-id="a784e-113">被</span><span class="sxs-lookup"><span data-stu-id="a784e-113">isDeleted</span></span>         | <span data-ttu-id="a784e-114">布尔</span><span class="sxs-lookup"><span data-stu-id="a784e-114">Boolean</span></span> |
| <span data-ttu-id="a784e-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="a784e-115">deletedDate</span></span>       | <span data-ttu-id="a784e-116">日期</span><span class="sxs-lookup"><span data-stu-id="a784e-116">Date</span></span>    |
| <span data-ttu-id="a784e-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="a784e-117">usedWeb</span></span>           | <span data-ttu-id="a784e-118">布尔</span><span class="sxs-lookup"><span data-stu-id="a784e-118">Boolean</span></span> |
| <span data-ttu-id="a784e-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="a784e-119">usedWindowsPhone</span></span>  | <span data-ttu-id="a784e-120">布尔</span><span class="sxs-lookup"><span data-stu-id="a784e-120">Boolean</span></span> |
| <span data-ttu-id="a784e-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="a784e-121">usediOS</span></span>           | <span data-ttu-id="a784e-122">布尔</span><span class="sxs-lookup"><span data-stu-id="a784e-122">Boolean</span></span> |
| <span data-ttu-id="a784e-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="a784e-123">usedMac</span></span>           | <span data-ttu-id="a784e-124">布尔</span><span class="sxs-lookup"><span data-stu-id="a784e-124">Boolean</span></span> |
| <span data-ttu-id="a784e-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="a784e-125">usedAndroidPhone</span></span>  | <span data-ttu-id="a784e-126">布尔</span><span class="sxs-lookup"><span data-stu-id="a784e-126">Boolean</span></span> |
| <span data-ttu-id="a784e-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="a784e-127">usedWindows</span></span>       | <span data-ttu-id="a784e-128">布尔</span><span class="sxs-lookup"><span data-stu-id="a784e-128">Boolean</span></span> |
| <span data-ttu-id="a784e-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a784e-129">reportPeriod</span></span>      | <span data-ttu-id="a784e-130">String</span><span class="sxs-lookup"><span data-stu-id="a784e-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="a784e-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a784e-131">JSON representation</span></span>

<span data-ttu-id="a784e-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a784e-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usediOS": true, 
  "usedMac": true, 
  "usedAndroidPhone": true, 
  "usedWindows": true, 
  "reportPeriod": "String"
}
```
