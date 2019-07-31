---
title: teamsDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5bd7443e775a8a9de0dbbc27cf8843331f8f8cb7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007625"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="e3759-103">teamsDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="e3759-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e3759-104">属性</span><span class="sxs-lookup"><span data-stu-id="e3759-104">Properties</span></span>

| <span data-ttu-id="e3759-105">属性</span><span class="sxs-lookup"><span data-stu-id="e3759-105">Property</span></span>          | <span data-ttu-id="e3759-106">类型</span><span class="sxs-lookup"><span data-stu-id="e3759-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="e3759-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e3759-107">reportRefreshDate</span></span> | <span data-ttu-id="e3759-108">日期</span><span class="sxs-lookup"><span data-stu-id="e3759-108">Date</span></span>    |
| <span data-ttu-id="e3759-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e3759-109">userPrincipalName</span></span> | <span data-ttu-id="e3759-110">String</span><span class="sxs-lookup"><span data-stu-id="e3759-110">String</span></span>  |
| <span data-ttu-id="e3759-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="e3759-111">lastActivityDate</span></span>  | <span data-ttu-id="e3759-112">日期</span><span class="sxs-lookup"><span data-stu-id="e3759-112">Date</span></span>    |
| <span data-ttu-id="e3759-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="e3759-113">isDeleted</span></span>         | <span data-ttu-id="e3759-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3759-114">Boolean</span></span> |
| <span data-ttu-id="e3759-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="e3759-115">deletedDate</span></span>       | <span data-ttu-id="e3759-116">日期</span><span class="sxs-lookup"><span data-stu-id="e3759-116">Date</span></span>    |
| <span data-ttu-id="e3759-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="e3759-117">usedWeb</span></span>           | <span data-ttu-id="e3759-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3759-118">Boolean</span></span> |
| <span data-ttu-id="e3759-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="e3759-119">usedWindowsPhone</span></span>  | <span data-ttu-id="e3759-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3759-120">Boolean</span></span> |
| <span data-ttu-id="e3759-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="e3759-121">usediOS</span></span>           | <span data-ttu-id="e3759-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3759-122">Boolean</span></span> |
| <span data-ttu-id="e3759-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="e3759-123">usedMac</span></span>           | <span data-ttu-id="e3759-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3759-124">Boolean</span></span> |
| <span data-ttu-id="e3759-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="e3759-125">usedAndroidPhone</span></span>  | <span data-ttu-id="e3759-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3759-126">Boolean</span></span> |
| <span data-ttu-id="e3759-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="e3759-127">usedWindows</span></span>       | <span data-ttu-id="e3759-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3759-128">Boolean</span></span> |
| <span data-ttu-id="e3759-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e3759-129">reportPeriod</span></span>      | <span data-ttu-id="e3759-130">String</span><span class="sxs-lookup"><span data-stu-id="e3759-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="e3759-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3759-131">JSON representation</span></span>

<span data-ttu-id="e3759-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3759-132">The following is a JSON representation of the resource.</span></span>

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
