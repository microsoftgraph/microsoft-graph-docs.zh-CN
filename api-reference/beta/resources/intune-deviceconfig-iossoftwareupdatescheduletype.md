---
title: iosSoftwareUpdateScheduleType 枚举类型
description: 更新 iOS 软件更新的计划类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 19be0994224d3700b39f0150336e924a1ad87d3c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085029"
---
# <a name="iossoftwareupdatescheduletype-enum-type"></a><span data-ttu-id="0ba14-103">iosSoftwareUpdateScheduleType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0ba14-103">iosSoftwareUpdateScheduleType enum type</span></span>

<span data-ttu-id="0ba14-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ba14-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ba14-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0ba14-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ba14-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ba14-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ba14-107">更新 iOS 软件更新的计划类型。</span><span class="sxs-lookup"><span data-stu-id="0ba14-107">Update schedule type for iOS software updates.</span></span>

## <a name="members"></a><span data-ttu-id="0ba14-108">成员</span><span class="sxs-lookup"><span data-stu-id="0ba14-108">Members</span></span>
|<span data-ttu-id="0ba14-109">成员</span><span class="sxs-lookup"><span data-stu-id="0ba14-109">Member</span></span>|<span data-ttu-id="0ba14-110">值</span><span class="sxs-lookup"><span data-stu-id="0ba14-110">Value</span></span>|<span data-ttu-id="0ba14-111">说明</span><span class="sxs-lookup"><span data-stu-id="0ba14-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ba14-112">updateOutsideOfActiveHours</span><span class="sxs-lookup"><span data-stu-id="0ba14-112">updateOutsideOfActiveHours</span></span>|<span data-ttu-id="0ba14-113">0</span><span class="sxs-lookup"><span data-stu-id="0ba14-113">0</span></span>|<span data-ttu-id="0ba14-114">更新为主动时段之外的。</span><span class="sxs-lookup"><span data-stu-id="0ba14-114">Update outside of active hours.</span></span>|
|<span data-ttu-id="0ba14-115">alwaysUpdate</span><span class="sxs-lookup"><span data-stu-id="0ba14-115">alwaysUpdate</span></span>|<span data-ttu-id="0ba14-116">1 </span><span class="sxs-lookup"><span data-stu-id="0ba14-116">1</span></span>|<span data-ttu-id="0ba14-117">时刻更新。</span><span class="sxs-lookup"><span data-stu-id="0ba14-117">Always update.</span></span>|
|<span data-ttu-id="0ba14-118">updateDuringTimeWindows</span><span class="sxs-lookup"><span data-stu-id="0ba14-118">updateDuringTimeWindows</span></span>|<span data-ttu-id="0ba14-119">2 </span><span class="sxs-lookup"><span data-stu-id="0ba14-119">2</span></span>|<span data-ttu-id="0ba14-120">在时间时段内更新。</span><span class="sxs-lookup"><span data-stu-id="0ba14-120">Update during time windows.</span></span>|
|<span data-ttu-id="0ba14-121">updateOutsideOfTimeWindows</span><span class="sxs-lookup"><span data-stu-id="0ba14-121">updateOutsideOfTimeWindows</span></span>|<span data-ttu-id="0ba14-122">第三章</span><span class="sxs-lookup"><span data-stu-id="0ba14-122">3</span></span>|<span data-ttu-id="0ba14-123">在时段外更新。</span><span class="sxs-lookup"><span data-stu-id="0ba14-123">Update outside of time windows.</span></span>|






