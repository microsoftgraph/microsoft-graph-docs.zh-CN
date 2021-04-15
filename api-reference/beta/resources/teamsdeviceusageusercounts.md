---
title: teamsDeviceUsageUserCounts 资源类型
description: 表示按设备类型表示的每日用户数。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9d7b813727a5ac9b2f7547e108bad8ee455d206b
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766572"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="d889b-103">teamsDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="d889b-103">teamsDeviceUsageUserCounts resource type</span></span>

<span data-ttu-id="d889b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d889b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d889b-105">表示按设备类型表示的每日用户数。</span><span class="sxs-lookup"><span data-stu-id="d889b-105">Represents number of daily users by device type.</span></span>

## <a name="properties"></a><span data-ttu-id="d889b-106">属性</span><span class="sxs-lookup"><span data-stu-id="d889b-106">Properties</span></span>

| <span data-ttu-id="d889b-107">属性</span><span class="sxs-lookup"><span data-stu-id="d889b-107">Property</span></span>          | <span data-ttu-id="d889b-108">类型</span><span class="sxs-lookup"><span data-stu-id="d889b-108">Type</span></span>   | <span data-ttu-id="d889b-109">说明</span><span class="sxs-lookup"><span data-stu-id="d889b-109">Description</span></span>                                                  |
| :---------------- | :----- | ------------------------------------------------------------ |
| <span data-ttu-id="d889b-110">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d889b-110">reportRefreshDate</span></span> | <span data-ttu-id="d889b-111">日期</span><span class="sxs-lookup"><span data-stu-id="d889b-111">Date</span></span>   | <span data-ttu-id="d889b-112">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="d889b-112">The latest date of the content.</span></span>                              |
| <span data-ttu-id="d889b-113">web</span><span class="sxs-lookup"><span data-stu-id="d889b-113">web</span></span>               | <span data-ttu-id="d889b-114">Int64</span><span class="sxs-lookup"><span data-stu-id="d889b-114">Int64</span></span>  | <span data-ttu-id="d889b-115">在设备上 Teams Web 客户端中处于活动状态的用户数。</span><span class="sxs-lookup"><span data-stu-id="d889b-115">The number of users who were active in the Teams web client on devices.</span></span> |
| <span data-ttu-id="d889b-116">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="d889b-116">windowsPhone</span></span>      | <span data-ttu-id="d889b-117">Int64</span><span class="sxs-lookup"><span data-stu-id="d889b-117">Int64</span></span>  | <span data-ttu-id="d889b-118">在适用于 Windows Phone 的 Teams 移动客户端上处于活动状态的用户数量。</span><span class="sxs-lookup"><span data-stu-id="d889b-118">The number of users who were active on the Teams mobile client for Windows phone.</span></span> |
| <span data-ttu-id="d889b-119">androidPhone</span><span class="sxs-lookup"><span data-stu-id="d889b-119">androidPhone</span></span>      | <span data-ttu-id="d889b-120">Int64</span><span class="sxs-lookup"><span data-stu-id="d889b-120">Int64</span></span>  | <span data-ttu-id="d889b-121">在适用于 Android 的 Teams 移动客户端上处于活动状态的用户数。</span><span class="sxs-lookup"><span data-stu-id="d889b-121">The number of users who were active on the Teams mobile client for Android.</span></span> |
| <span data-ttu-id="d889b-122">ios</span><span class="sxs-lookup"><span data-stu-id="d889b-122">ios</span></span>               | <span data-ttu-id="d889b-123">Int64</span><span class="sxs-lookup"><span data-stu-id="d889b-123">Int64</span></span>  | <span data-ttu-id="d889b-124">在适用于 iOS 的 Teams 移动客户端上处于活动状态的用户数量。</span><span class="sxs-lookup"><span data-stu-id="d889b-124">The number of users who were active on the Teams mobile client for iOS.</span></span> |
| <span data-ttu-id="d889b-125">mac</span><span class="sxs-lookup"><span data-stu-id="d889b-125">mac</span></span>               | <span data-ttu-id="d889b-126">Int64</span><span class="sxs-lookup"><span data-stu-id="d889b-126">Int64</span></span>  | <span data-ttu-id="d889b-127">在 macOS 计算机上 Teams 桌面客户端中处于活动状态的用户数。</span><span class="sxs-lookup"><span data-stu-id="d889b-127">The number of users who were active in the Teams desktop client on a macOS computer.</span></span> |
| <span data-ttu-id="d889b-128">windows</span><span class="sxs-lookup"><span data-stu-id="d889b-128">windows</span></span>           | <span data-ttu-id="d889b-129">Int64</span><span class="sxs-lookup"><span data-stu-id="d889b-129">Int64</span></span>  | <span data-ttu-id="d889b-130">在基于 Windows 的计算机上在 Teams 桌面客户端中处于活动状态的用户数。</span><span class="sxs-lookup"><span data-stu-id="d889b-130">The number of users who were active in the Teams desktop client on a Windows-based computer.</span></span> |
| <span data-ttu-id="d889b-131">chromeOS</span><span class="sxs-lookup"><span data-stu-id="d889b-131">chromeOS</span></span>          | <span data-ttu-id="d889b-132">Int64</span><span class="sxs-lookup"><span data-stu-id="d889b-132">Int64</span></span>  | <span data-ttu-id="d889b-133">在 ChromeOS 计算机上 Teams 桌面客户端中处于活动状态的用户数。</span><span class="sxs-lookup"><span data-stu-id="d889b-133">The number of users who were active in the Teams desktop client on a ChromeOS computer.</span></span> |
| <span data-ttu-id="d889b-134">linux</span><span class="sxs-lookup"><span data-stu-id="d889b-134">linux</span></span>             | <span data-ttu-id="d889b-135">Int64</span><span class="sxs-lookup"><span data-stu-id="d889b-135">Int64</span></span>  | <span data-ttu-id="d889b-136">在 Linux 计算机上在 Teams 桌面客户端中处于活动状态的用户数。</span><span class="sxs-lookup"><span data-stu-id="d889b-136">The number of users who were active in the Teams desktop client on a Linux computer.</span></span> |
| <span data-ttu-id="d889b-137">reportDate</span><span class="sxs-lookup"><span data-stu-id="d889b-137">reportDate</span></span>        | <span data-ttu-id="d889b-138">日期</span><span class="sxs-lookup"><span data-stu-id="d889b-138">Date</span></span>   | <span data-ttu-id="d889b-139">用户执行活动的日期。</span><span class="sxs-lookup"><span data-stu-id="d889b-139">The date on which the users performed the activities.</span></span>        |
| <span data-ttu-id="d889b-140">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d889b-140">reportPeriod</span></span>      | <span data-ttu-id="d889b-141">String</span><span class="sxs-lookup"><span data-stu-id="d889b-141">String</span></span> | <span data-ttu-id="d889b-142">报告涵盖的天数。</span><span class="sxs-lookup"><span data-stu-id="d889b-142">The number of days the report covers.</span></span>                        |

## <a name="representation"></a><span data-ttu-id="d889b-143">表示形式</span><span class="sxs-lookup"><span data-stu-id="d889b-143">representation</span></span>

<span data-ttu-id="d889b-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d889b-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "chromeOS": 1024, 
  "linux": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


