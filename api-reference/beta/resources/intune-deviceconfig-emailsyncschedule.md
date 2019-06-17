---
title: emailSyncSchedule 枚举类型
description: 电子邮件同步计划的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f84c9a5cdb5d9608a34553c2a3a6f05a989b78a8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995061"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="792a6-103">emailSyncSchedule 枚举类型</span><span class="sxs-lookup"><span data-stu-id="792a6-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="792a6-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="792a6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="792a6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="792a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="792a6-106">电子邮件同步计划的可能值。</span><span class="sxs-lookup"><span data-stu-id="792a6-106">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="792a6-107">成员</span><span class="sxs-lookup"><span data-stu-id="792a6-107">Members</span></span>
|<span data-ttu-id="792a6-108">成员</span><span class="sxs-lookup"><span data-stu-id="792a6-108">Member</span></span>|<span data-ttu-id="792a6-109">值</span><span class="sxs-lookup"><span data-stu-id="792a6-109">Value</span></span>|<span data-ttu-id="792a6-110">说明</span><span class="sxs-lookup"><span data-stu-id="792a6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="792a6-111">定制</span><span class="sxs-lookup"><span data-stu-id="792a6-111">userDefined</span></span>|<span data-ttu-id="792a6-112">0</span><span class="sxs-lookup"><span data-stu-id="792a6-112">0</span></span>|<span data-ttu-id="792a6-113">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="792a6-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="792a6-114">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="792a6-114">asMessagesArrive</span></span>|<span data-ttu-id="792a6-115">1</span><span class="sxs-lookup"><span data-stu-id="792a6-115">1</span></span>|<span data-ttu-id="792a6-116">邮件到达时同步。</span><span class="sxs-lookup"><span data-stu-id="792a6-116">Sync as messages arrive.</span></span>|
|<span data-ttu-id="792a6-117">手动</span><span class="sxs-lookup"><span data-stu-id="792a6-117">manual</span></span>|<span data-ttu-id="792a6-118">双面</span><span class="sxs-lookup"><span data-stu-id="792a6-118">2</span></span>|<span data-ttu-id="792a6-119">手动同步。</span><span class="sxs-lookup"><span data-stu-id="792a6-119">Sync manually.</span></span>|
|<span data-ttu-id="792a6-120">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="792a6-120">fifteenMinutes</span></span>|<span data-ttu-id="792a6-121">第三章</span><span class="sxs-lookup"><span data-stu-id="792a6-121">3</span></span>|<span data-ttu-id="792a6-122">每十五分钟同步一次。</span><span class="sxs-lookup"><span data-stu-id="792a6-122">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="792a6-123">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="792a6-123">thirtyMinutes</span></span>|<span data-ttu-id="792a6-124">4</span><span class="sxs-lookup"><span data-stu-id="792a6-124">4</span></span>|<span data-ttu-id="792a6-125">每三十分钟同步一次。</span><span class="sxs-lookup"><span data-stu-id="792a6-125">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="792a6-126">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="792a6-126">sixtyMinutes</span></span>|<span data-ttu-id="792a6-127">5</span><span class="sxs-lookup"><span data-stu-id="792a6-127">5</span></span>|<span data-ttu-id="792a6-128">每60分钟同步一次。</span><span class="sxs-lookup"><span data-stu-id="792a6-128">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="792a6-129">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="792a6-129">basedOnMyUsage</span></span>|<span data-ttu-id="792a6-130">型</span><span class="sxs-lookup"><span data-stu-id="792a6-130">6</span></span>|<span data-ttu-id="792a6-131">根据我的使用情况进行同步。</span><span class="sxs-lookup"><span data-stu-id="792a6-131">Sync based on my usage.</span></span>|





