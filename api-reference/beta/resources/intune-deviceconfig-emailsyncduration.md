---
title: emailSyncDuration 枚举类型
description: 电子邮件同步持续时间的可能值。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1ca28161d7a4f8b0683be6a96df00bf4cdd7cda6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460092"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="cd49c-103">emailSyncDuration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cd49c-103">emailSyncDuration enum type</span></span>

<span data-ttu-id="cd49c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd49c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd49c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cd49c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd49c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cd49c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd49c-107">电子邮件同步持续时间的可能值。</span><span class="sxs-lookup"><span data-stu-id="cd49c-107">Possible values for email sync duration.</span></span>

## <a name="members"></a><span data-ttu-id="cd49c-108">成员</span><span class="sxs-lookup"><span data-stu-id="cd49c-108">Members</span></span>
|<span data-ttu-id="cd49c-109">成员</span><span class="sxs-lookup"><span data-stu-id="cd49c-109">Member</span></span>|<span data-ttu-id="cd49c-110">值</span><span class="sxs-lookup"><span data-stu-id="cd49c-110">Value</span></span>|<span data-ttu-id="cd49c-111">说明</span><span class="sxs-lookup"><span data-stu-id="cd49c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd49c-112">定制</span><span class="sxs-lookup"><span data-stu-id="cd49c-112">userDefined</span></span>|<span data-ttu-id="cd49c-113">0</span><span class="sxs-lookup"><span data-stu-id="cd49c-113">0</span></span>|<span data-ttu-id="cd49c-114">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="cd49c-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="cd49c-115">oneDay</span><span class="sxs-lookup"><span data-stu-id="cd49c-115">oneDay</span></span>|<span data-ttu-id="cd49c-116">1</span><span class="sxs-lookup"><span data-stu-id="cd49c-116">1</span></span>|<span data-ttu-id="cd49c-117">同步一天的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="cd49c-117">Sync one day of email.</span></span>|
|<span data-ttu-id="cd49c-118">threeDays</span><span class="sxs-lookup"><span data-stu-id="cd49c-118">threeDays</span></span>|<span data-ttu-id="cd49c-119">双面</span><span class="sxs-lookup"><span data-stu-id="cd49c-119">2</span></span>|<span data-ttu-id="cd49c-120">同步三天的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="cd49c-120">Sync three days of email.</span></span>|
|<span data-ttu-id="cd49c-121">oneWeek</span><span class="sxs-lookup"><span data-stu-id="cd49c-121">oneWeek</span></span>|<span data-ttu-id="cd49c-122">第三章</span><span class="sxs-lookup"><span data-stu-id="cd49c-122">3</span></span>|<span data-ttu-id="cd49c-123">同步一周电子邮件。</span><span class="sxs-lookup"><span data-stu-id="cd49c-123">Sync one week of email.</span></span>|
|<span data-ttu-id="cd49c-124">twoWeeks</span><span class="sxs-lookup"><span data-stu-id="cd49c-124">twoWeeks</span></span>|<span data-ttu-id="cd49c-125">4 </span><span class="sxs-lookup"><span data-stu-id="cd49c-125">4</span></span>|<span data-ttu-id="cd49c-126">同步两周的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="cd49c-126">Sync two weeks of email.</span></span>|
|<span data-ttu-id="cd49c-127">oneMonth</span><span class="sxs-lookup"><span data-stu-id="cd49c-127">oneMonth</span></span>|<span data-ttu-id="cd49c-128">5 </span><span class="sxs-lookup"><span data-stu-id="cd49c-128">5</span></span>|<span data-ttu-id="cd49c-129">同步一个月的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="cd49c-129">Sync one month of email.</span></span>|
|<span data-ttu-id="cd49c-130">不限制</span><span class="sxs-lookup"><span data-stu-id="cd49c-130">unlimited</span></span>|<span data-ttu-id="cd49c-131">6 </span><span class="sxs-lookup"><span data-stu-id="cd49c-131">6</span></span>|<span data-ttu-id="cd49c-132">同步无限制的电子邮件持续时间。</span><span class="sxs-lookup"><span data-stu-id="cd49c-132">Sync an unlimited duration of email.</span></span>|



