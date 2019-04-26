---
title: emailSyncSchedule 枚举类型
description: 电子邮件同步计划的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1da569d7050e88dd5eb41640bc2d8eaa602bb2b7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556219"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="f0b28-103">emailSyncSchedule 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f0b28-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="f0b28-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f0b28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0b28-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0b28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0b28-106">电子邮件同步计划的可能值。</span><span class="sxs-lookup"><span data-stu-id="f0b28-106">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="f0b28-107">成员</span><span class="sxs-lookup"><span data-stu-id="f0b28-107">Members</span></span>
|<span data-ttu-id="f0b28-108">成员</span><span class="sxs-lookup"><span data-stu-id="f0b28-108">Member</span></span>|<span data-ttu-id="f0b28-109">值</span><span class="sxs-lookup"><span data-stu-id="f0b28-109">Value</span></span>|<span data-ttu-id="f0b28-110">说明</span><span class="sxs-lookup"><span data-stu-id="f0b28-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0b28-111">定制</span><span class="sxs-lookup"><span data-stu-id="f0b28-111">userDefined</span></span>|<span data-ttu-id="f0b28-112">0</span><span class="sxs-lookup"><span data-stu-id="f0b28-112">0</span></span>|<span data-ttu-id="f0b28-113">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="f0b28-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="f0b28-114">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="f0b28-114">asMessagesArrive</span></span>|<span data-ttu-id="f0b28-115">1</span><span class="sxs-lookup"><span data-stu-id="f0b28-115">1</span></span>|<span data-ttu-id="f0b28-116">邮件到达时同步。</span><span class="sxs-lookup"><span data-stu-id="f0b28-116">Sync as messages arrive.</span></span>|
|<span data-ttu-id="f0b28-117">手动</span><span class="sxs-lookup"><span data-stu-id="f0b28-117">manual</span></span>|<span data-ttu-id="f0b28-118">2 </span><span class="sxs-lookup"><span data-stu-id="f0b28-118">2</span></span>|<span data-ttu-id="f0b28-119">手动同步。</span><span class="sxs-lookup"><span data-stu-id="f0b28-119">Sync manually.</span></span>|
|<span data-ttu-id="f0b28-120">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="f0b28-120">fifteenMinutes</span></span>|<span data-ttu-id="f0b28-121">3 </span><span class="sxs-lookup"><span data-stu-id="f0b28-121">3</span></span>|<span data-ttu-id="f0b28-122">每十五分钟同步一次。</span><span class="sxs-lookup"><span data-stu-id="f0b28-122">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="f0b28-123">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="f0b28-123">thirtyMinutes</span></span>|<span data-ttu-id="f0b28-124">4 </span><span class="sxs-lookup"><span data-stu-id="f0b28-124">4</span></span>|<span data-ttu-id="f0b28-125">每三十分钟同步一次。</span><span class="sxs-lookup"><span data-stu-id="f0b28-125">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="f0b28-126">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="f0b28-126">sixtyMinutes</span></span>|<span data-ttu-id="f0b28-127">5 </span><span class="sxs-lookup"><span data-stu-id="f0b28-127">5</span></span>|<span data-ttu-id="f0b28-128">每60分钟同步一次。</span><span class="sxs-lookup"><span data-stu-id="f0b28-128">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="f0b28-129">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="f0b28-129">basedOnMyUsage</span></span>|<span data-ttu-id="f0b28-130">6 </span><span class="sxs-lookup"><span data-stu-id="f0b28-130">6</span></span>|<span data-ttu-id="f0b28-131">根据我的使用情况进行同步。</span><span class="sxs-lookup"><span data-stu-id="f0b28-131">Sync based on my usage.</span></span>|





