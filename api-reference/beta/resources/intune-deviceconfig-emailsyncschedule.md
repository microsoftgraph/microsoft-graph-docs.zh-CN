---
title: emailSyncSchedule 枚举类型
description: 电子邮件同步计划的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 63e0c1ffaed029ca5ba010181c70ab0588135a36
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49198872"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="0ad98-103">emailSyncSchedule 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0ad98-103">emailSyncSchedule enum type</span></span>

<span data-ttu-id="0ad98-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ad98-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ad98-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0ad98-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ad98-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ad98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ad98-107">电子邮件同步计划的可能值。</span><span class="sxs-lookup"><span data-stu-id="0ad98-107">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="0ad98-108">成员</span><span class="sxs-lookup"><span data-stu-id="0ad98-108">Members</span></span>
|<span data-ttu-id="0ad98-109">成员</span><span class="sxs-lookup"><span data-stu-id="0ad98-109">Member</span></span>|<span data-ttu-id="0ad98-110">值</span><span class="sxs-lookup"><span data-stu-id="0ad98-110">Value</span></span>|<span data-ttu-id="0ad98-111">说明</span><span class="sxs-lookup"><span data-stu-id="0ad98-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ad98-112">定制</span><span class="sxs-lookup"><span data-stu-id="0ad98-112">userDefined</span></span>|<span data-ttu-id="0ad98-113">0</span><span class="sxs-lookup"><span data-stu-id="0ad98-113">0</span></span>|<span data-ttu-id="0ad98-114">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="0ad98-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="0ad98-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="0ad98-115">asMessagesArrive</span></span>|<span data-ttu-id="0ad98-116">1</span><span class="sxs-lookup"><span data-stu-id="0ad98-116">1</span></span>|<span data-ttu-id="0ad98-117">邮件到达时同步。</span><span class="sxs-lookup"><span data-stu-id="0ad98-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="0ad98-118">手动</span><span class="sxs-lookup"><span data-stu-id="0ad98-118">manual</span></span>|<span data-ttu-id="0ad98-119">双面</span><span class="sxs-lookup"><span data-stu-id="0ad98-119">2</span></span>|<span data-ttu-id="0ad98-120">手动同步。</span><span class="sxs-lookup"><span data-stu-id="0ad98-120">Sync manually.</span></span>|
|<span data-ttu-id="0ad98-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="0ad98-121">fifteenMinutes</span></span>|<span data-ttu-id="0ad98-122">第三章</span><span class="sxs-lookup"><span data-stu-id="0ad98-122">3</span></span>|<span data-ttu-id="0ad98-123">每十五分钟同步一次。</span><span class="sxs-lookup"><span data-stu-id="0ad98-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="0ad98-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="0ad98-124">thirtyMinutes</span></span>|<span data-ttu-id="0ad98-125">4 </span><span class="sxs-lookup"><span data-stu-id="0ad98-125">4</span></span>|<span data-ttu-id="0ad98-126">每三十分钟同步一次。</span><span class="sxs-lookup"><span data-stu-id="0ad98-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="0ad98-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="0ad98-127">sixtyMinutes</span></span>|<span data-ttu-id="0ad98-128">5 </span><span class="sxs-lookup"><span data-stu-id="0ad98-128">5</span></span>|<span data-ttu-id="0ad98-129">每60分钟同步一次。</span><span class="sxs-lookup"><span data-stu-id="0ad98-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="0ad98-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="0ad98-130">basedOnMyUsage</span></span>|<span data-ttu-id="0ad98-131">6 </span><span class="sxs-lookup"><span data-stu-id="0ad98-131">6</span></span>|<span data-ttu-id="0ad98-132">根据我的使用情况进行同步。</span><span class="sxs-lookup"><span data-stu-id="0ad98-132">Sync based on my usage.</span></span>|




