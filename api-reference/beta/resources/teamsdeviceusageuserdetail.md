---
title: teamsDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8cdd2fe1a212bb1d36846b80fc1b558c576deb47
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553601"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="afb3d-103">teamsDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="afb3d-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="afb3d-104">属性</span><span class="sxs-lookup"><span data-stu-id="afb3d-104">Properties</span></span>

| <span data-ttu-id="afb3d-105">属性</span><span class="sxs-lookup"><span data-stu-id="afb3d-105">Property</span></span>          | <span data-ttu-id="afb3d-106">类型</span><span class="sxs-lookup"><span data-stu-id="afb3d-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="afb3d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="afb3d-107">reportRefreshDate</span></span> | <span data-ttu-id="afb3d-108">Date</span><span class="sxs-lookup"><span data-stu-id="afb3d-108">Date</span></span>    |
| <span data-ttu-id="afb3d-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="afb3d-109">userPrincipalName</span></span> | <span data-ttu-id="afb3d-110">String</span><span class="sxs-lookup"><span data-stu-id="afb3d-110">String</span></span>  |
| <span data-ttu-id="afb3d-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="afb3d-111">lastActivityDate</span></span>  | <span data-ttu-id="afb3d-112">Date</span><span class="sxs-lookup"><span data-stu-id="afb3d-112">Date</span></span>    |
| <span data-ttu-id="afb3d-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="afb3d-113">isDeleted</span></span>         | <span data-ttu-id="afb3d-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="afb3d-114">Boolean</span></span> |
| <span data-ttu-id="afb3d-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="afb3d-115">deletedDate</span></span>       | <span data-ttu-id="afb3d-116">Date</span><span class="sxs-lookup"><span data-stu-id="afb3d-116">Date</span></span>    |
| <span data-ttu-id="afb3d-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="afb3d-117">usedWeb</span></span>           | <span data-ttu-id="afb3d-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="afb3d-118">Boolean</span></span> |
| <span data-ttu-id="afb3d-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="afb3d-119">usedWindowsPhone</span></span>  | <span data-ttu-id="afb3d-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="afb3d-120">Boolean</span></span> |
| <span data-ttu-id="afb3d-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="afb3d-121">usediOS</span></span>           | <span data-ttu-id="afb3d-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="afb3d-122">Boolean</span></span> |
| <span data-ttu-id="afb3d-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="afb3d-123">usedMac</span></span>           | <span data-ttu-id="afb3d-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="afb3d-124">Boolean</span></span> |
| <span data-ttu-id="afb3d-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="afb3d-125">usedAndroidPhone</span></span>  | <span data-ttu-id="afb3d-126">布尔值</span><span class="sxs-lookup"><span data-stu-id="afb3d-126">Boolean</span></span> |
| <span data-ttu-id="afb3d-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="afb3d-127">usedWindows</span></span>       | <span data-ttu-id="afb3d-128">布尔值</span><span class="sxs-lookup"><span data-stu-id="afb3d-128">Boolean</span></span> |
| <span data-ttu-id="afb3d-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="afb3d-129">reportPeriod</span></span>      | <span data-ttu-id="afb3d-130">String</span><span class="sxs-lookup"><span data-stu-id="afb3d-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="afb3d-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="afb3d-131">JSON representation</span></span>

<span data-ttu-id="afb3d-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="afb3d-132">The following is a JSON representation of the resource.</span></span>

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
