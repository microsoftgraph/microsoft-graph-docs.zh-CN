---
title: emailSyncSchedule 枚举类型
description: 电子邮件同步计划的可能值。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 178cba9e226b7f20e3fd917145e7bbd06f6c3a1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838393"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="3c55d-103">emailSyncSchedule 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3c55d-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="3c55d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3c55d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c55d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3c55d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c55d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3c55d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c55d-107">电子邮件同步计划的可能值。</span><span class="sxs-lookup"><span data-stu-id="3c55d-107">Possible values for email sync schedule.</span></span>
## <a name="members"></a><span data-ttu-id="3c55d-108">成员</span><span class="sxs-lookup"><span data-stu-id="3c55d-108">Members</span></span>
|<span data-ttu-id="3c55d-109">成员</span><span class="sxs-lookup"><span data-stu-id="3c55d-109">Member</span></span>|<span data-ttu-id="3c55d-110">值</span><span class="sxs-lookup"><span data-stu-id="3c55d-110">Value</span></span>|<span data-ttu-id="3c55d-111">Description</span><span class="sxs-lookup"><span data-stu-id="3c55d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c55d-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="3c55d-112">userDefined</span></span>|<span data-ttu-id="3c55d-113">0</span><span class="sxs-lookup"><span data-stu-id="3c55d-113">0</span></span>|<span data-ttu-id="3c55d-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="3c55d-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="3c55d-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="3c55d-115">asMessagesArrive</span></span>|<span data-ttu-id="3c55d-116">1</span><span class="sxs-lookup"><span data-stu-id="3c55d-116">1</span></span>|<span data-ttu-id="3c55d-117">当消息到达同步。</span><span class="sxs-lookup"><span data-stu-id="3c55d-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="3c55d-118">手动</span><span class="sxs-lookup"><span data-stu-id="3c55d-118">manual</span></span>|<span data-ttu-id="3c55d-119">2</span><span class="sxs-lookup"><span data-stu-id="3c55d-119">2</span></span>|<span data-ttu-id="3c55d-120">手动同步。</span><span class="sxs-lookup"><span data-stu-id="3c55d-120">Sync manually.</span></span>|
|<span data-ttu-id="3c55d-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="3c55d-121">fifteenMinutes</span></span>|<span data-ttu-id="3c55d-122">3</span><span class="sxs-lookup"><span data-stu-id="3c55d-122">3</span></span>|<span data-ttu-id="3c55d-123">同步每 15 分钟。</span><span class="sxs-lookup"><span data-stu-id="3c55d-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="3c55d-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="3c55d-124">thirtyMinutes</span></span>|<span data-ttu-id="3c55d-125">4</span><span class="sxs-lookup"><span data-stu-id="3c55d-125">4</span></span>|<span data-ttu-id="3c55d-126">同步每 30 分钟。</span><span class="sxs-lookup"><span data-stu-id="3c55d-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="3c55d-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="3c55d-127">sixtyMinutes</span></span>|<span data-ttu-id="3c55d-128">5</span><span class="sxs-lookup"><span data-stu-id="3c55d-128">5</span></span>|<span data-ttu-id="3c55d-129">同步每隔 60 分钟。</span><span class="sxs-lookup"><span data-stu-id="3c55d-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="3c55d-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="3c55d-130">basedOnMyUsage</span></span>|<span data-ttu-id="3c55d-131">6</span><span class="sxs-lookup"><span data-stu-id="3c55d-131">6</span></span>|<span data-ttu-id="3c55d-132">根据我使用情况的同步。</span><span class="sxs-lookup"><span data-stu-id="3c55d-132">Sync based on my usage.</span></span>|





