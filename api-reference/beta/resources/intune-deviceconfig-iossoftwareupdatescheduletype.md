---
title: iosSoftwareUpdateScheduleType 枚举类型
description: 更新 iOS 软件更新的计划类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 915cab792c4a076f0ded4df64e189f57a0e04eb0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728547"
---
# <a name="iossoftwareupdatescheduletype-enum-type"></a><span data-ttu-id="e8436-103">iosSoftwareUpdateScheduleType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e8436-103">iosSoftwareUpdateScheduleType enum type</span></span>

<span data-ttu-id="e8436-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8436-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8436-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e8436-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8436-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e8436-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8436-107">更新 iOS 软件更新的计划类型。</span><span class="sxs-lookup"><span data-stu-id="e8436-107">Update schedule type for iOS software updates.</span></span>

## <a name="members"></a><span data-ttu-id="e8436-108">成员</span><span class="sxs-lookup"><span data-stu-id="e8436-108">Members</span></span>
|<span data-ttu-id="e8436-109">成员</span><span class="sxs-lookup"><span data-stu-id="e8436-109">Member</span></span>|<span data-ttu-id="e8436-110">值</span><span class="sxs-lookup"><span data-stu-id="e8436-110">Value</span></span>|<span data-ttu-id="e8436-111">说明</span><span class="sxs-lookup"><span data-stu-id="e8436-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8436-112">updateOutsideOfActiveHours</span><span class="sxs-lookup"><span data-stu-id="e8436-112">updateOutsideOfActiveHours</span></span>|<span data-ttu-id="e8436-113">0</span><span class="sxs-lookup"><span data-stu-id="e8436-113">0</span></span>|<span data-ttu-id="e8436-114">更新为主动时段之外的。</span><span class="sxs-lookup"><span data-stu-id="e8436-114">Update outside of active hours.</span></span>|
|<span data-ttu-id="e8436-115">alwaysUpdate</span><span class="sxs-lookup"><span data-stu-id="e8436-115">alwaysUpdate</span></span>|<span data-ttu-id="e8436-116">1</span><span class="sxs-lookup"><span data-stu-id="e8436-116">1</span></span>|<span data-ttu-id="e8436-117">时刻更新。</span><span class="sxs-lookup"><span data-stu-id="e8436-117">Always update.</span></span>|
|<span data-ttu-id="e8436-118">updateDuringTimeWindows</span><span class="sxs-lookup"><span data-stu-id="e8436-118">updateDuringTimeWindows</span></span>|<span data-ttu-id="e8436-119">双面</span><span class="sxs-lookup"><span data-stu-id="e8436-119">2</span></span>|<span data-ttu-id="e8436-120">在时间时段内更新。</span><span class="sxs-lookup"><span data-stu-id="e8436-120">Update during time windows.</span></span>|
|<span data-ttu-id="e8436-121">updateOutsideOfTimeWindows</span><span class="sxs-lookup"><span data-stu-id="e8436-121">updateOutsideOfTimeWindows</span></span>|<span data-ttu-id="e8436-122">第三章</span><span class="sxs-lookup"><span data-stu-id="e8436-122">3</span></span>|<span data-ttu-id="e8436-123">在时段外更新。</span><span class="sxs-lookup"><span data-stu-id="e8436-123">Update outside of time windows.</span></span>|





