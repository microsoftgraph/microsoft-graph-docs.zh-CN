---
title: emailSyncDuration 枚举类型
description: 电子邮件同步持续时间的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4c199f55d78f14ca7e77a24a0e1c62762b51afb3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705958"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="f4f4c-103">emailSyncDuration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f4f4c-103">emailSyncDuration enum type</span></span>

<span data-ttu-id="f4f4c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4f4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4f4c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4f4c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4f4c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4f4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4f4c-107">电子邮件同步持续时间的可能值。</span><span class="sxs-lookup"><span data-stu-id="f4f4c-107">Possible values for email sync duration.</span></span>

## <a name="members"></a><span data-ttu-id="f4f4c-108">成员</span><span class="sxs-lookup"><span data-stu-id="f4f4c-108">Members</span></span>
|<span data-ttu-id="f4f4c-109">成员</span><span class="sxs-lookup"><span data-stu-id="f4f4c-109">Member</span></span>|<span data-ttu-id="f4f4c-110">值</span><span class="sxs-lookup"><span data-stu-id="f4f4c-110">Value</span></span>|<span data-ttu-id="f4f4c-111">说明</span><span class="sxs-lookup"><span data-stu-id="f4f4c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4f4c-112">定制</span><span class="sxs-lookup"><span data-stu-id="f4f4c-112">userDefined</span></span>|<span data-ttu-id="f4f4c-113">0</span><span class="sxs-lookup"><span data-stu-id="f4f4c-113">0</span></span>|<span data-ttu-id="f4f4c-114">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="f4f4c-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="f4f4c-115">oneDay</span><span class="sxs-lookup"><span data-stu-id="f4f4c-115">oneDay</span></span>|<span data-ttu-id="f4f4c-116">1</span><span class="sxs-lookup"><span data-stu-id="f4f4c-116">1</span></span>|<span data-ttu-id="f4f4c-117">同步一天的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="f4f4c-117">Sync one day of email.</span></span>|
|<span data-ttu-id="f4f4c-118">threeDays</span><span class="sxs-lookup"><span data-stu-id="f4f4c-118">threeDays</span></span>|<span data-ttu-id="f4f4c-119">双面</span><span class="sxs-lookup"><span data-stu-id="f4f4c-119">2</span></span>|<span data-ttu-id="f4f4c-120">同步三天的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="f4f4c-120">Sync three days of email.</span></span>|
|<span data-ttu-id="f4f4c-121">oneWeek</span><span class="sxs-lookup"><span data-stu-id="f4f4c-121">oneWeek</span></span>|<span data-ttu-id="f4f4c-122">第三章</span><span class="sxs-lookup"><span data-stu-id="f4f4c-122">3</span></span>|<span data-ttu-id="f4f4c-123">同步一周电子邮件。</span><span class="sxs-lookup"><span data-stu-id="f4f4c-123">Sync one week of email.</span></span>|
|<span data-ttu-id="f4f4c-124">twoWeeks</span><span class="sxs-lookup"><span data-stu-id="f4f4c-124">twoWeeks</span></span>|<span data-ttu-id="f4f4c-125">4 </span><span class="sxs-lookup"><span data-stu-id="f4f4c-125">4</span></span>|<span data-ttu-id="f4f4c-126">同步两周的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="f4f4c-126">Sync two weeks of email.</span></span>|
|<span data-ttu-id="f4f4c-127">oneMonth</span><span class="sxs-lookup"><span data-stu-id="f4f4c-127">oneMonth</span></span>|<span data-ttu-id="f4f4c-128">5 </span><span class="sxs-lookup"><span data-stu-id="f4f4c-128">5</span></span>|<span data-ttu-id="f4f4c-129">同步一个月的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="f4f4c-129">Sync one month of email.</span></span>|
|<span data-ttu-id="f4f4c-130">不限制</span><span class="sxs-lookup"><span data-stu-id="f4f4c-130">unlimited</span></span>|<span data-ttu-id="f4f4c-131">6 </span><span class="sxs-lookup"><span data-stu-id="f4f4c-131">6</span></span>|<span data-ttu-id="f4f4c-132">同步无限制的电子邮件持续时间。</span><span class="sxs-lookup"><span data-stu-id="f4f4c-132">Sync an unlimited duration of email.</span></span>|





