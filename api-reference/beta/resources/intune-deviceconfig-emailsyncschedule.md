---
title: emailSyncSchedule 枚举类型
description: 电子邮件同步计划的可能值。
author: tfitzmac
ms.openlocfilehash: f0e6673064f7e483756dfcfec8ce074e809dfcf4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308678"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="aee78-103">emailSyncSchedule 枚举类型</span><span class="sxs-lookup"><span data-stu-id="aee78-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="aee78-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aee78-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aee78-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aee78-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aee78-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="aee78-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aee78-107">电子邮件同步计划的可能值。</span><span class="sxs-lookup"><span data-stu-id="aee78-107">Possible values for email sync schedule.</span></span>
## <a name="members"></a><span data-ttu-id="aee78-108">成员</span><span class="sxs-lookup"><span data-stu-id="aee78-108">Members</span></span>
|<span data-ttu-id="aee78-109">成员</span><span class="sxs-lookup"><span data-stu-id="aee78-109">Member</span></span>|<span data-ttu-id="aee78-110">值</span><span class="sxs-lookup"><span data-stu-id="aee78-110">Value</span></span>|<span data-ttu-id="aee78-111">说明</span><span class="sxs-lookup"><span data-stu-id="aee78-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aee78-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="aee78-112">userDefined</span></span>|<span data-ttu-id="aee78-113">0</span><span class="sxs-lookup"><span data-stu-id="aee78-113">0</span></span>|<span data-ttu-id="aee78-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="aee78-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="aee78-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="aee78-115">asMessagesArrive</span></span>|<span data-ttu-id="aee78-116">1</span><span class="sxs-lookup"><span data-stu-id="aee78-116">1</span></span>|<span data-ttu-id="aee78-117">当消息到达同步。</span><span class="sxs-lookup"><span data-stu-id="aee78-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="aee78-118">手动</span><span class="sxs-lookup"><span data-stu-id="aee78-118">manual</span></span>|<span data-ttu-id="aee78-119">2</span><span class="sxs-lookup"><span data-stu-id="aee78-119">2</span></span>|<span data-ttu-id="aee78-120">手动同步。</span><span class="sxs-lookup"><span data-stu-id="aee78-120">Sync manually.</span></span>|
|<span data-ttu-id="aee78-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="aee78-121">fifteenMinutes</span></span>|<span data-ttu-id="aee78-122">3</span><span class="sxs-lookup"><span data-stu-id="aee78-122">3</span></span>|<span data-ttu-id="aee78-123">同步每 15 分钟。</span><span class="sxs-lookup"><span data-stu-id="aee78-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="aee78-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="aee78-124">thirtyMinutes</span></span>|<span data-ttu-id="aee78-125">4</span><span class="sxs-lookup"><span data-stu-id="aee78-125">4</span></span>|<span data-ttu-id="aee78-126">同步每 30 分钟。</span><span class="sxs-lookup"><span data-stu-id="aee78-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="aee78-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="aee78-127">sixtyMinutes</span></span>|<span data-ttu-id="aee78-128">5</span><span class="sxs-lookup"><span data-stu-id="aee78-128">5</span></span>|<span data-ttu-id="aee78-129">同步每隔 60 分钟。</span><span class="sxs-lookup"><span data-stu-id="aee78-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="aee78-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="aee78-130">basedOnMyUsage</span></span>|<span data-ttu-id="aee78-131">6</span><span class="sxs-lookup"><span data-stu-id="aee78-131">6</span></span>|<span data-ttu-id="aee78-132">根据我使用情况的同步。</span><span class="sxs-lookup"><span data-stu-id="aee78-132">Sync based on my usage.</span></span>|





