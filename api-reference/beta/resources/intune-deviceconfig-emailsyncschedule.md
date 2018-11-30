---
title: emailSyncSchedule 枚举类型
description: 电子邮件同步计划的可能值。
ms.openlocfilehash: 48c5d433815d5f27d018d97ac479641146754669
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041632"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="8f41c-103">emailSyncSchedule 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8f41c-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="8f41c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8f41c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f41c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8f41c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f41c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8f41c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f41c-107">电子邮件同步计划的可能值。</span><span class="sxs-lookup"><span data-stu-id="8f41c-107">Possible values for email sync schedule.</span></span>
## <a name="members"></a><span data-ttu-id="8f41c-108">成员</span><span class="sxs-lookup"><span data-stu-id="8f41c-108">Members</span></span>
|<span data-ttu-id="8f41c-109">成员</span><span class="sxs-lookup"><span data-stu-id="8f41c-109">Member</span></span>|<span data-ttu-id="8f41c-110">值</span><span class="sxs-lookup"><span data-stu-id="8f41c-110">Value</span></span>|<span data-ttu-id="8f41c-111">说明</span><span class="sxs-lookup"><span data-stu-id="8f41c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f41c-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="8f41c-112">userDefined</span></span>|<span data-ttu-id="8f41c-113">0</span><span class="sxs-lookup"><span data-stu-id="8f41c-113">0</span></span>|<span data-ttu-id="8f41c-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="8f41c-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="8f41c-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="8f41c-115">asMessagesArrive</span></span>|<span data-ttu-id="8f41c-116">1</span><span class="sxs-lookup"><span data-stu-id="8f41c-116">1</span></span>|<span data-ttu-id="8f41c-117">当消息到达同步。</span><span class="sxs-lookup"><span data-stu-id="8f41c-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="8f41c-118">手动</span><span class="sxs-lookup"><span data-stu-id="8f41c-118">manual</span></span>|<span data-ttu-id="8f41c-119">2</span><span class="sxs-lookup"><span data-stu-id="8f41c-119">2</span></span>|<span data-ttu-id="8f41c-120">手动同步。</span><span class="sxs-lookup"><span data-stu-id="8f41c-120">Sync manually.</span></span>|
|<span data-ttu-id="8f41c-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="8f41c-121">fifteenMinutes</span></span>|<span data-ttu-id="8f41c-122">3</span><span class="sxs-lookup"><span data-stu-id="8f41c-122">3</span></span>|<span data-ttu-id="8f41c-123">同步每 15 分钟。</span><span class="sxs-lookup"><span data-stu-id="8f41c-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="8f41c-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="8f41c-124">thirtyMinutes</span></span>|<span data-ttu-id="8f41c-125">4</span><span class="sxs-lookup"><span data-stu-id="8f41c-125">4</span></span>|<span data-ttu-id="8f41c-126">同步每 30 分钟。</span><span class="sxs-lookup"><span data-stu-id="8f41c-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="8f41c-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="8f41c-127">sixtyMinutes</span></span>|<span data-ttu-id="8f41c-128">5</span><span class="sxs-lookup"><span data-stu-id="8f41c-128">5</span></span>|<span data-ttu-id="8f41c-129">同步每隔 60 分钟。</span><span class="sxs-lookup"><span data-stu-id="8f41c-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="8f41c-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="8f41c-130">basedOnMyUsage</span></span>|<span data-ttu-id="8f41c-131">6</span><span class="sxs-lookup"><span data-stu-id="8f41c-131">6</span></span>|<span data-ttu-id="8f41c-132">根据我使用情况的同步。</span><span class="sxs-lookup"><span data-stu-id="8f41c-132">Sync based on my usage.</span></span>|





