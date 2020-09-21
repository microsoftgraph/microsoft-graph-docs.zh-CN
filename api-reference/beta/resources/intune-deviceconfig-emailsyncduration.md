---
title: emailSyncDuration 枚举类型
description: 电子邮件同步持续时间的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 64dbd2e5321affeacc45eeccc63ad76b862f70db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003729"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="81cc3-103">emailSyncDuration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="81cc3-103">emailSyncDuration enum type</span></span>

<span data-ttu-id="81cc3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81cc3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81cc3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="81cc3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81cc3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81cc3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81cc3-107">电子邮件同步持续时间的可能值。</span><span class="sxs-lookup"><span data-stu-id="81cc3-107">Possible values for email sync duration.</span></span>

## <a name="members"></a><span data-ttu-id="81cc3-108">成员</span><span class="sxs-lookup"><span data-stu-id="81cc3-108">Members</span></span>
|<span data-ttu-id="81cc3-109">成员</span><span class="sxs-lookup"><span data-stu-id="81cc3-109">Member</span></span>|<span data-ttu-id="81cc3-110">值</span><span class="sxs-lookup"><span data-stu-id="81cc3-110">Value</span></span>|<span data-ttu-id="81cc3-111">说明</span><span class="sxs-lookup"><span data-stu-id="81cc3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81cc3-112">定制</span><span class="sxs-lookup"><span data-stu-id="81cc3-112">userDefined</span></span>|<span data-ttu-id="81cc3-113">0</span><span class="sxs-lookup"><span data-stu-id="81cc3-113">0</span></span>|<span data-ttu-id="81cc3-114">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="81cc3-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="81cc3-115">oneDay</span><span class="sxs-lookup"><span data-stu-id="81cc3-115">oneDay</span></span>|<span data-ttu-id="81cc3-116">1 </span><span class="sxs-lookup"><span data-stu-id="81cc3-116">1</span></span>|<span data-ttu-id="81cc3-117">同步一天的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="81cc3-117">Sync one day of email.</span></span>|
|<span data-ttu-id="81cc3-118">threeDays</span><span class="sxs-lookup"><span data-stu-id="81cc3-118">threeDays</span></span>|<span data-ttu-id="81cc3-119">2 </span><span class="sxs-lookup"><span data-stu-id="81cc3-119">2</span></span>|<span data-ttu-id="81cc3-120">同步三天的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="81cc3-120">Sync three days of email.</span></span>|
|<span data-ttu-id="81cc3-121">oneWeek</span><span class="sxs-lookup"><span data-stu-id="81cc3-121">oneWeek</span></span>|<span data-ttu-id="81cc3-122">第三章</span><span class="sxs-lookup"><span data-stu-id="81cc3-122">3</span></span>|<span data-ttu-id="81cc3-123">同步一周电子邮件。</span><span class="sxs-lookup"><span data-stu-id="81cc3-123">Sync one week of email.</span></span>|
|<span data-ttu-id="81cc3-124">twoWeeks</span><span class="sxs-lookup"><span data-stu-id="81cc3-124">twoWeeks</span></span>|<span data-ttu-id="81cc3-125">4 </span><span class="sxs-lookup"><span data-stu-id="81cc3-125">4</span></span>|<span data-ttu-id="81cc3-126">同步两周的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="81cc3-126">Sync two weeks of email.</span></span>|
|<span data-ttu-id="81cc3-127">oneMonth</span><span class="sxs-lookup"><span data-stu-id="81cc3-127">oneMonth</span></span>|<span data-ttu-id="81cc3-128">5 </span><span class="sxs-lookup"><span data-stu-id="81cc3-128">5</span></span>|<span data-ttu-id="81cc3-129">同步一个月的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="81cc3-129">Sync one month of email.</span></span>|
|<span data-ttu-id="81cc3-130">不限制</span><span class="sxs-lookup"><span data-stu-id="81cc3-130">unlimited</span></span>|<span data-ttu-id="81cc3-131">6 </span><span class="sxs-lookup"><span data-stu-id="81cc3-131">6</span></span>|<span data-ttu-id="81cc3-132">同步无限制的电子邮件持续时间。</span><span class="sxs-lookup"><span data-stu-id="81cc3-132">Sync an unlimited duration of email.</span></span>|






