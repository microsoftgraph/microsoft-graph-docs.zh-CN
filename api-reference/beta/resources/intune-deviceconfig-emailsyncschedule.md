---
title: emailSyncSchedule 枚举类型
description: 电子邮件同步计划的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 209cacfad96a4523cce3a6125652dc86f61227d9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994202"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="16664-103">emailSyncSchedule 枚举类型</span><span class="sxs-lookup"><span data-stu-id="16664-103">emailSyncSchedule enum type</span></span>

<span data-ttu-id="16664-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16664-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16664-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="16664-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16664-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="16664-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16664-107">电子邮件同步计划的可能值。</span><span class="sxs-lookup"><span data-stu-id="16664-107">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="16664-108">成员</span><span class="sxs-lookup"><span data-stu-id="16664-108">Members</span></span>
|<span data-ttu-id="16664-109">成员</span><span class="sxs-lookup"><span data-stu-id="16664-109">Member</span></span>|<span data-ttu-id="16664-110">值</span><span class="sxs-lookup"><span data-stu-id="16664-110">Value</span></span>|<span data-ttu-id="16664-111">说明</span><span class="sxs-lookup"><span data-stu-id="16664-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16664-112">定制</span><span class="sxs-lookup"><span data-stu-id="16664-112">userDefined</span></span>|<span data-ttu-id="16664-113">0</span><span class="sxs-lookup"><span data-stu-id="16664-113">0</span></span>|<span data-ttu-id="16664-114">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="16664-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="16664-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="16664-115">asMessagesArrive</span></span>|<span data-ttu-id="16664-116">1 </span><span class="sxs-lookup"><span data-stu-id="16664-116">1</span></span>|<span data-ttu-id="16664-117">邮件到达时同步。</span><span class="sxs-lookup"><span data-stu-id="16664-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="16664-118">手动</span><span class="sxs-lookup"><span data-stu-id="16664-118">manual</span></span>|<span data-ttu-id="16664-119">2 </span><span class="sxs-lookup"><span data-stu-id="16664-119">2</span></span>|<span data-ttu-id="16664-120">手动同步。</span><span class="sxs-lookup"><span data-stu-id="16664-120">Sync manually.</span></span>|
|<span data-ttu-id="16664-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="16664-121">fifteenMinutes</span></span>|<span data-ttu-id="16664-122">第三章</span><span class="sxs-lookup"><span data-stu-id="16664-122">3</span></span>|<span data-ttu-id="16664-123">每十五分钟同步一次。</span><span class="sxs-lookup"><span data-stu-id="16664-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="16664-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="16664-124">thirtyMinutes</span></span>|<span data-ttu-id="16664-125">4 </span><span class="sxs-lookup"><span data-stu-id="16664-125">4</span></span>|<span data-ttu-id="16664-126">每三十分钟同步一次。</span><span class="sxs-lookup"><span data-stu-id="16664-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="16664-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="16664-127">sixtyMinutes</span></span>|<span data-ttu-id="16664-128">5 </span><span class="sxs-lookup"><span data-stu-id="16664-128">5</span></span>|<span data-ttu-id="16664-129">每60分钟同步一次。</span><span class="sxs-lookup"><span data-stu-id="16664-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="16664-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="16664-130">basedOnMyUsage</span></span>|<span data-ttu-id="16664-131">6 </span><span class="sxs-lookup"><span data-stu-id="16664-131">6</span></span>|<span data-ttu-id="16664-132">根据我的使用情况进行同步。</span><span class="sxs-lookup"><span data-stu-id="16664-132">Sync based on my usage.</span></span>|






