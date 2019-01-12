---
title: teamsDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8cdd2fe1a212bb1d36846b80fc1b558c576deb47
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953783"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="bc64e-103">teamsDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc64e-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="bc64e-104">属性</span><span class="sxs-lookup"><span data-stu-id="bc64e-104">Properties</span></span>

| <span data-ttu-id="bc64e-105">属性</span><span class="sxs-lookup"><span data-stu-id="bc64e-105">Property</span></span>          | <span data-ttu-id="bc64e-106">类型</span><span class="sxs-lookup"><span data-stu-id="bc64e-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="bc64e-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="bc64e-107">reportRefreshDate</span></span> | <span data-ttu-id="bc64e-108">日期</span><span class="sxs-lookup"><span data-stu-id="bc64e-108">Date</span></span>    |
| <span data-ttu-id="bc64e-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bc64e-109">userPrincipalName</span></span> | <span data-ttu-id="bc64e-110">字符串</span><span class="sxs-lookup"><span data-stu-id="bc64e-110">String</span></span>  |
| <span data-ttu-id="bc64e-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="bc64e-111">lastActivityDate</span></span>  | <span data-ttu-id="bc64e-112">日期</span><span class="sxs-lookup"><span data-stu-id="bc64e-112">Date</span></span>    |
| <span data-ttu-id="bc64e-113">被</span><span class="sxs-lookup"><span data-stu-id="bc64e-113">isDeleted</span></span>         | <span data-ttu-id="bc64e-114">布尔</span><span class="sxs-lookup"><span data-stu-id="bc64e-114">Boolean</span></span> |
| <span data-ttu-id="bc64e-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="bc64e-115">deletedDate</span></span>       | <span data-ttu-id="bc64e-116">日期</span><span class="sxs-lookup"><span data-stu-id="bc64e-116">Date</span></span>    |
| <span data-ttu-id="bc64e-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="bc64e-117">usedWeb</span></span>           | <span data-ttu-id="bc64e-118">布尔</span><span class="sxs-lookup"><span data-stu-id="bc64e-118">Boolean</span></span> |
| <span data-ttu-id="bc64e-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="bc64e-119">usedWindowsPhone</span></span>  | <span data-ttu-id="bc64e-120">布尔</span><span class="sxs-lookup"><span data-stu-id="bc64e-120">Boolean</span></span> |
| <span data-ttu-id="bc64e-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="bc64e-121">usediOS</span></span>           | <span data-ttu-id="bc64e-122">布尔</span><span class="sxs-lookup"><span data-stu-id="bc64e-122">Boolean</span></span> |
| <span data-ttu-id="bc64e-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="bc64e-123">usedMac</span></span>           | <span data-ttu-id="bc64e-124">布尔</span><span class="sxs-lookup"><span data-stu-id="bc64e-124">Boolean</span></span> |
| <span data-ttu-id="bc64e-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="bc64e-125">usedAndroidPhone</span></span>  | <span data-ttu-id="bc64e-126">布尔</span><span class="sxs-lookup"><span data-stu-id="bc64e-126">Boolean</span></span> |
| <span data-ttu-id="bc64e-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="bc64e-127">usedWindows</span></span>       | <span data-ttu-id="bc64e-128">布尔</span><span class="sxs-lookup"><span data-stu-id="bc64e-128">Boolean</span></span> |
| <span data-ttu-id="bc64e-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="bc64e-129">reportPeriod</span></span>      | <span data-ttu-id="bc64e-130">String</span><span class="sxs-lookup"><span data-stu-id="bc64e-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="bc64e-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc64e-131">JSON representation</span></span>

<span data-ttu-id="bc64e-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc64e-132">The following is a JSON representation of the resource.</span></span>

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
