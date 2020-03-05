---
title: teamsDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c5c3815b2418f414aa552f211bbeed5f643eb0d4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519860"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="3f677-103">teamsDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f677-103">teamsDeviceUsageUserDetail resource type</span></span>

<span data-ttu-id="3f677-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3f677-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="3f677-105">属性</span><span class="sxs-lookup"><span data-stu-id="3f677-105">Properties</span></span>

| <span data-ttu-id="3f677-106">属性</span><span class="sxs-lookup"><span data-stu-id="3f677-106">Property</span></span>          | <span data-ttu-id="3f677-107">类型</span><span class="sxs-lookup"><span data-stu-id="3f677-107">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="3f677-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3f677-108">reportRefreshDate</span></span> | <span data-ttu-id="3f677-109">日期</span><span class="sxs-lookup"><span data-stu-id="3f677-109">Date</span></span>    |
| <span data-ttu-id="3f677-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3f677-110">userPrincipalName</span></span> | <span data-ttu-id="3f677-111">String</span><span class="sxs-lookup"><span data-stu-id="3f677-111">String</span></span>  |
| <span data-ttu-id="3f677-112">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="3f677-112">lastActivityDate</span></span>  | <span data-ttu-id="3f677-113">日期</span><span class="sxs-lookup"><span data-stu-id="3f677-113">Date</span></span>    |
| <span data-ttu-id="3f677-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="3f677-114">isDeleted</span></span>         | <span data-ttu-id="3f677-115">布尔</span><span class="sxs-lookup"><span data-stu-id="3f677-115">Boolean</span></span> |
| <span data-ttu-id="3f677-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="3f677-116">deletedDate</span></span>       | <span data-ttu-id="3f677-117">日期</span><span class="sxs-lookup"><span data-stu-id="3f677-117">Date</span></span>    |
| <span data-ttu-id="3f677-118">usedWeb</span><span class="sxs-lookup"><span data-stu-id="3f677-118">usedWeb</span></span>           | <span data-ttu-id="3f677-119">布尔</span><span class="sxs-lookup"><span data-stu-id="3f677-119">Boolean</span></span> |
| <span data-ttu-id="3f677-120">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="3f677-120">usedWindowsPhone</span></span>  | <span data-ttu-id="3f677-121">布尔</span><span class="sxs-lookup"><span data-stu-id="3f677-121">Boolean</span></span> |
| <span data-ttu-id="3f677-122">usediOS</span><span class="sxs-lookup"><span data-stu-id="3f677-122">usediOS</span></span>           | <span data-ttu-id="3f677-123">布尔</span><span class="sxs-lookup"><span data-stu-id="3f677-123">Boolean</span></span> |
| <span data-ttu-id="3f677-124">usedMac</span><span class="sxs-lookup"><span data-stu-id="3f677-124">usedMac</span></span>           | <span data-ttu-id="3f677-125">布尔</span><span class="sxs-lookup"><span data-stu-id="3f677-125">Boolean</span></span> |
| <span data-ttu-id="3f677-126">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="3f677-126">usedAndroidPhone</span></span>  | <span data-ttu-id="3f677-127">布尔</span><span class="sxs-lookup"><span data-stu-id="3f677-127">Boolean</span></span> |
| <span data-ttu-id="3f677-128">usedWindows</span><span class="sxs-lookup"><span data-stu-id="3f677-128">usedWindows</span></span>       | <span data-ttu-id="3f677-129">布尔</span><span class="sxs-lookup"><span data-stu-id="3f677-129">Boolean</span></span> |
| <span data-ttu-id="3f677-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3f677-130">reportPeriod</span></span>      | <span data-ttu-id="3f677-131">String</span><span class="sxs-lookup"><span data-stu-id="3f677-131">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="3f677-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f677-132">JSON representation</span></span>

<span data-ttu-id="3f677-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f677-133">The following is a JSON representation of the resource.</span></span>

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
