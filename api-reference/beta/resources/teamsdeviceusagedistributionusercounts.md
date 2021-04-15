---
title: teamsDeviceUsageDistributionUserCounts 资源类型
description: 表示选定时段内按设备类型表示的用户数。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2d1c716a4be9ab6ffac7b37484d7cb8bc8f01ee9
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766565"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a><span data-ttu-id="cd409-103">teamsDeviceUsageDistributionUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd409-103">teamsDeviceUsageDistributionUserCounts resource type</span></span>

<span data-ttu-id="cd409-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd409-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd409-105">表示选定时段内按设备类型表示的用户数。</span><span class="sxs-lookup"><span data-stu-id="cd409-105">Represents number of users by device type over the selected time period.</span></span>

## <a name="properties"></a><span data-ttu-id="cd409-106">属性</span><span class="sxs-lookup"><span data-stu-id="cd409-106">Properties</span></span>

| <span data-ttu-id="cd409-107">属性</span><span class="sxs-lookup"><span data-stu-id="cd409-107">Property</span></span>          | <span data-ttu-id="cd409-108">类型</span><span class="sxs-lookup"><span data-stu-id="cd409-108">Type</span></span>   | <span data-ttu-id="cd409-109">说明</span><span class="sxs-lookup"><span data-stu-id="cd409-109">Description</span></span>                                                  |
| :---------------- | :----- | ------------------------------------------------------------ |
| <span data-ttu-id="cd409-110">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="cd409-110">reportRefreshDate</span></span> | <span data-ttu-id="cd409-111">日期</span><span class="sxs-lookup"><span data-stu-id="cd409-111">Date</span></span>   | <span data-ttu-id="cd409-112">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="cd409-112">The latest date of the content.</span></span>                              |
| <span data-ttu-id="cd409-113">web</span><span class="sxs-lookup"><span data-stu-id="cd409-113">web</span></span>               | <span data-ttu-id="cd409-114">Int64</span><span class="sxs-lookup"><span data-stu-id="cd409-114">Int64</span></span>  | <span data-ttu-id="cd409-115">在设备上 Teams Web 客户端中处于活动状态的用户数。</span><span class="sxs-lookup"><span data-stu-id="cd409-115">The number of users who were active in the Teams web client on devices.</span></span> |
| <span data-ttu-id="cd409-116">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="cd409-116">windowsPhone</span></span>      | <span data-ttu-id="cd409-117">Int64</span><span class="sxs-lookup"><span data-stu-id="cd409-117">Int64</span></span>  | <span data-ttu-id="cd409-118">在适用于 Windows Phone 的 Teams 移动客户端上处于活动状态的用户数量。</span><span class="sxs-lookup"><span data-stu-id="cd409-118">The number of users who were active on the Teams mobile client for Windows phone.</span></span> |
| <span data-ttu-id="cd409-119">androidPhone</span><span class="sxs-lookup"><span data-stu-id="cd409-119">androidPhone</span></span>      | <span data-ttu-id="cd409-120">Int64</span><span class="sxs-lookup"><span data-stu-id="cd409-120">Int64</span></span>  | <span data-ttu-id="cd409-121">在适用于 Android 的 Teams 移动客户端上处于活动状态的用户数。</span><span class="sxs-lookup"><span data-stu-id="cd409-121">The number of users who were active on the Teams mobile client for Android.</span></span> |
| <span data-ttu-id="cd409-122">ios</span><span class="sxs-lookup"><span data-stu-id="cd409-122">ios</span></span>               | <span data-ttu-id="cd409-123">Int64</span><span class="sxs-lookup"><span data-stu-id="cd409-123">Int64</span></span>  | <span data-ttu-id="cd409-124">在适用于 iOS 的 Teams 移动客户端上处于活动状态的用户数量。</span><span class="sxs-lookup"><span data-stu-id="cd409-124">The number of users who were active on the Teams mobile client for iOS.</span></span> |
| <span data-ttu-id="cd409-125">mac</span><span class="sxs-lookup"><span data-stu-id="cd409-125">mac</span></span>               | <span data-ttu-id="cd409-126">Int64</span><span class="sxs-lookup"><span data-stu-id="cd409-126">Int64</span></span>  | <span data-ttu-id="cd409-127">在 macOS 计算机上 Teams 桌面客户端中处于活动状态的用户数。</span><span class="sxs-lookup"><span data-stu-id="cd409-127">The number of users who were active in the Teams desktop client on a macOS computer.</span></span> |
| <span data-ttu-id="cd409-128">windows</span><span class="sxs-lookup"><span data-stu-id="cd409-128">windows</span></span>           | <span data-ttu-id="cd409-129">Int64</span><span class="sxs-lookup"><span data-stu-id="cd409-129">Int64</span></span>  | <span data-ttu-id="cd409-130">在基于 Windows 的计算机上在 Teams 桌面客户端中处于活动状态的用户数。</span><span class="sxs-lookup"><span data-stu-id="cd409-130">The number of users who were active in the Teams desktop client on a Windows-based computer.</span></span> |
| <span data-ttu-id="cd409-131">chromeOS</span><span class="sxs-lookup"><span data-stu-id="cd409-131">chromeOS</span></span>          | <span data-ttu-id="cd409-132">Int64</span><span class="sxs-lookup"><span data-stu-id="cd409-132">Int64</span></span>  | <span data-ttu-id="cd409-133">在 ChromeOS 计算机上 Teams 桌面客户端中处于活动状态的用户数。</span><span class="sxs-lookup"><span data-stu-id="cd409-133">The number of users who were active in the Teams desktop client on a ChromeOS computer.</span></span> |
| <span data-ttu-id="cd409-134">linux</span><span class="sxs-lookup"><span data-stu-id="cd409-134">linux</span></span>             | <span data-ttu-id="cd409-135">Int64</span><span class="sxs-lookup"><span data-stu-id="cd409-135">Int64</span></span>  | <span data-ttu-id="cd409-136">在 Linux 计算机上在 Teams 桌面客户端中处于活动状态的用户数。</span><span class="sxs-lookup"><span data-stu-id="cd409-136">The number of users who were active in the Teams desktop client on a Linux computer.</span></span> |
| <span data-ttu-id="cd409-137">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="cd409-137">reportPeriod</span></span>      | <span data-ttu-id="cd409-138">String</span><span class="sxs-lookup"><span data-stu-id="cd409-138">String</span></span> | <span data-ttu-id="cd409-139">报告涵盖的天数。</span><span class="sxs-lookup"><span data-stu-id="cd409-139">The number of days the report covers.</span></span>                        |

## <a name="json-representation"></a><span data-ttu-id="cd409-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd409-140">JSON representation</span></span>

<span data-ttu-id="cd409-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd409-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
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
  "reportPeriod": "String"
}
```


