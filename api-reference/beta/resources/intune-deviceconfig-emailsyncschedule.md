---
title: emailSyncSchedule 枚举类型
description: 电子邮件同步计划的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e4d3645ea2c0eaa7f8f1cf8138f1c0727cfa0d8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325629"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="59314-103">emailSyncSchedule 枚举类型</span><span class="sxs-lookup"><span data-stu-id="59314-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="59314-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="59314-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59314-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="59314-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59314-106">电子邮件同步计划的可能值。</span><span class="sxs-lookup"><span data-stu-id="59314-106">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="59314-107">成员</span><span class="sxs-lookup"><span data-stu-id="59314-107">Members</span></span>
|<span data-ttu-id="59314-108">成员</span><span class="sxs-lookup"><span data-stu-id="59314-108">Member</span></span>|<span data-ttu-id="59314-109">值</span><span class="sxs-lookup"><span data-stu-id="59314-109">Value</span></span>|<span data-ttu-id="59314-110">说明</span><span class="sxs-lookup"><span data-stu-id="59314-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59314-111">定制</span><span class="sxs-lookup"><span data-stu-id="59314-111">userDefined</span></span>|<span data-ttu-id="59314-112">0</span><span class="sxs-lookup"><span data-stu-id="59314-112">0</span></span>|<span data-ttu-id="59314-113">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="59314-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="59314-114">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="59314-114">asMessagesArrive</span></span>|<span data-ttu-id="59314-115">1</span><span class="sxs-lookup"><span data-stu-id="59314-115">1</span></span>|<span data-ttu-id="59314-116">邮件到达时同步。</span><span class="sxs-lookup"><span data-stu-id="59314-116">Sync as messages arrive.</span></span>|
|<span data-ttu-id="59314-117">手动</span><span class="sxs-lookup"><span data-stu-id="59314-117">manual</span></span>|<span data-ttu-id="59314-118">双面</span><span class="sxs-lookup"><span data-stu-id="59314-118">2</span></span>|<span data-ttu-id="59314-119">手动同步。</span><span class="sxs-lookup"><span data-stu-id="59314-119">Sync manually.</span></span>|
|<span data-ttu-id="59314-120">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="59314-120">fifteenMinutes</span></span>|<span data-ttu-id="59314-121">第三章</span><span class="sxs-lookup"><span data-stu-id="59314-121">3</span></span>|<span data-ttu-id="59314-122">每十五分钟同步一次。</span><span class="sxs-lookup"><span data-stu-id="59314-122">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="59314-123">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="59314-123">thirtyMinutes</span></span>|<span data-ttu-id="59314-124">4</span><span class="sxs-lookup"><span data-stu-id="59314-124">4</span></span>|<span data-ttu-id="59314-125">每三十分钟同步一次。</span><span class="sxs-lookup"><span data-stu-id="59314-125">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="59314-126">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="59314-126">sixtyMinutes</span></span>|<span data-ttu-id="59314-127">5</span><span class="sxs-lookup"><span data-stu-id="59314-127">5</span></span>|<span data-ttu-id="59314-128">每60分钟同步一次。</span><span class="sxs-lookup"><span data-stu-id="59314-128">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="59314-129">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="59314-129">basedOnMyUsage</span></span>|<span data-ttu-id="59314-130">型</span><span class="sxs-lookup"><span data-stu-id="59314-130">6</span></span>|<span data-ttu-id="59314-131">根据我的使用情况进行同步。</span><span class="sxs-lookup"><span data-stu-id="59314-131">Sync based on my usage.</span></span>|



