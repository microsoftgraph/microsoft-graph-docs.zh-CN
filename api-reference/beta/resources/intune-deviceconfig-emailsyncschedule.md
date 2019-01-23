---
title: emailSyncSchedule 枚举类型
description: 电子邮件同步计划的可能值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8285b9a34e208b86b7c53c38e6aa015fd8c37560
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425181"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="19c11-103">emailSyncSchedule 枚举类型</span><span class="sxs-lookup"><span data-stu-id="19c11-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="19c11-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="19c11-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="19c11-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="19c11-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19c11-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="19c11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19c11-107">电子邮件同步计划的可能值。</span><span class="sxs-lookup"><span data-stu-id="19c11-107">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="19c11-108">成员</span><span class="sxs-lookup"><span data-stu-id="19c11-108">Members</span></span>
|<span data-ttu-id="19c11-109">成员</span><span class="sxs-lookup"><span data-stu-id="19c11-109">Member</span></span>|<span data-ttu-id="19c11-110">值</span><span class="sxs-lookup"><span data-stu-id="19c11-110">Value</span></span>|<span data-ttu-id="19c11-111">说明</span><span class="sxs-lookup"><span data-stu-id="19c11-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19c11-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="19c11-112">userDefined</span></span>|<span data-ttu-id="19c11-113">0</span><span class="sxs-lookup"><span data-stu-id="19c11-113">0</span></span>|<span data-ttu-id="19c11-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="19c11-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="19c11-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="19c11-115">asMessagesArrive</span></span>|<span data-ttu-id="19c11-116">1</span><span class="sxs-lookup"><span data-stu-id="19c11-116">1</span></span>|<span data-ttu-id="19c11-117">当消息到达同步。</span><span class="sxs-lookup"><span data-stu-id="19c11-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="19c11-118">手动</span><span class="sxs-lookup"><span data-stu-id="19c11-118">manual</span></span>|<span data-ttu-id="19c11-119">2</span><span class="sxs-lookup"><span data-stu-id="19c11-119">2</span></span>|<span data-ttu-id="19c11-120">手动同步。</span><span class="sxs-lookup"><span data-stu-id="19c11-120">Sync manually.</span></span>|
|<span data-ttu-id="19c11-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="19c11-121">fifteenMinutes</span></span>|<span data-ttu-id="19c11-122">3</span><span class="sxs-lookup"><span data-stu-id="19c11-122">3</span></span>|<span data-ttu-id="19c11-123">同步每 15 分钟。</span><span class="sxs-lookup"><span data-stu-id="19c11-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="19c11-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="19c11-124">thirtyMinutes</span></span>|<span data-ttu-id="19c11-125">4</span><span class="sxs-lookup"><span data-stu-id="19c11-125">4</span></span>|<span data-ttu-id="19c11-126">同步每 30 分钟。</span><span class="sxs-lookup"><span data-stu-id="19c11-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="19c11-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="19c11-127">sixtyMinutes</span></span>|<span data-ttu-id="19c11-128">5</span><span class="sxs-lookup"><span data-stu-id="19c11-128">5</span></span>|<span data-ttu-id="19c11-129">同步每隔 60 分钟。</span><span class="sxs-lookup"><span data-stu-id="19c11-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="19c11-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="19c11-130">basedOnMyUsage</span></span>|<span data-ttu-id="19c11-131">6</span><span class="sxs-lookup"><span data-stu-id="19c11-131">6</span></span>|<span data-ttu-id="19c11-132">根据我使用情况的同步。</span><span class="sxs-lookup"><span data-stu-id="19c11-132">Sync based on my usage.</span></span>|




