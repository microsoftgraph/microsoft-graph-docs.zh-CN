---
title: emailSyncDuration 枚举类型
description: 电子邮件同步持续时间的可能值。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d83a1ceb82820ddc44d8753e8ed05e00de09e36e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819380"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="467d5-103">emailSyncDuration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="467d5-103">emailSyncDuration enum type</span></span>

> <span data-ttu-id="467d5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="467d5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="467d5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="467d5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="467d5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="467d5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="467d5-107">电子邮件同步持续时间的可能值。</span><span class="sxs-lookup"><span data-stu-id="467d5-107">Possible values for email sync duration.</span></span>
## <a name="members"></a><span data-ttu-id="467d5-108">成员</span><span class="sxs-lookup"><span data-stu-id="467d5-108">Members</span></span>
|<span data-ttu-id="467d5-109">成员</span><span class="sxs-lookup"><span data-stu-id="467d5-109">Member</span></span>|<span data-ttu-id="467d5-110">值</span><span class="sxs-lookup"><span data-stu-id="467d5-110">Value</span></span>|<span data-ttu-id="467d5-111">Description</span><span class="sxs-lookup"><span data-stu-id="467d5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="467d5-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="467d5-112">userDefined</span></span>|<span data-ttu-id="467d5-113">0</span><span class="sxs-lookup"><span data-stu-id="467d5-113">0</span></span>|<span data-ttu-id="467d5-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="467d5-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="467d5-115">工期</span><span class="sxs-lookup"><span data-stu-id="467d5-115">oneDay</span></span>|<span data-ttu-id="467d5-116">1</span><span class="sxs-lookup"><span data-stu-id="467d5-116">1</span></span>|<span data-ttu-id="467d5-117">同步电子邮件中的一天。</span><span class="sxs-lookup"><span data-stu-id="467d5-117">Sync one day of email.</span></span>|
|<span data-ttu-id="467d5-118">3 个工作日</span><span class="sxs-lookup"><span data-stu-id="467d5-118">threeDays</span></span>|<span data-ttu-id="467d5-119">2</span><span class="sxs-lookup"><span data-stu-id="467d5-119">2</span></span>|<span data-ttu-id="467d5-120">同步三天的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="467d5-120">Sync three days of email.</span></span>|
|<span data-ttu-id="467d5-121">1 周时间</span><span class="sxs-lookup"><span data-stu-id="467d5-121">oneWeek</span></span>|<span data-ttu-id="467d5-122">3</span><span class="sxs-lookup"><span data-stu-id="467d5-122">3</span></span>|<span data-ttu-id="467d5-123">同步电子邮件的一周。</span><span class="sxs-lookup"><span data-stu-id="467d5-123">Sync one week of email.</span></span>|
|<span data-ttu-id="467d5-124">twoWeeks</span><span class="sxs-lookup"><span data-stu-id="467d5-124">twoWeeks</span></span>|<span data-ttu-id="467d5-125">4</span><span class="sxs-lookup"><span data-stu-id="467d5-125">4</span></span>|<span data-ttu-id="467d5-126">同步电子邮件的两个星期。</span><span class="sxs-lookup"><span data-stu-id="467d5-126">Sync two weeks of email.</span></span>|
|<span data-ttu-id="467d5-127">oneMonth</span><span class="sxs-lookup"><span data-stu-id="467d5-127">oneMonth</span></span>|<span data-ttu-id="467d5-128">5</span><span class="sxs-lookup"><span data-stu-id="467d5-128">5</span></span>|<span data-ttu-id="467d5-129">同步电子邮件的一个月。</span><span class="sxs-lookup"><span data-stu-id="467d5-129">Sync one month of email.</span></span>|
|<span data-ttu-id="467d5-130">无限制</span><span class="sxs-lookup"><span data-stu-id="467d5-130">unlimited</span></span>|<span data-ttu-id="467d5-131">6</span><span class="sxs-lookup"><span data-stu-id="467d5-131">6</span></span>|<span data-ttu-id="467d5-132">同步电子邮件不受限制的持续的时间。</span><span class="sxs-lookup"><span data-stu-id="467d5-132">Sync an unlimited duration of email.</span></span>|





