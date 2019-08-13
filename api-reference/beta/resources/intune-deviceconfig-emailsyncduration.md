---
title: emailSyncDuration 枚举类型
description: 电子邮件同步持续时间的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fc05be47c2adc0764a2cdb1e69f7ec11413320cc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357192"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="2d1d2-103">emailSyncDuration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2d1d2-103">emailSyncDuration enum type</span></span>

> <span data-ttu-id="2d1d2-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2d1d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d1d2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d1d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d1d2-106">电子邮件同步持续时间的可能值。</span><span class="sxs-lookup"><span data-stu-id="2d1d2-106">Possible values for email sync duration.</span></span>

## <a name="members"></a><span data-ttu-id="2d1d2-107">成员</span><span class="sxs-lookup"><span data-stu-id="2d1d2-107">Members</span></span>
|<span data-ttu-id="2d1d2-108">成员</span><span class="sxs-lookup"><span data-stu-id="2d1d2-108">Member</span></span>|<span data-ttu-id="2d1d2-109">值</span><span class="sxs-lookup"><span data-stu-id="2d1d2-109">Value</span></span>|<span data-ttu-id="2d1d2-110">说明</span><span class="sxs-lookup"><span data-stu-id="2d1d2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d1d2-111">定制</span><span class="sxs-lookup"><span data-stu-id="2d1d2-111">userDefined</span></span>|<span data-ttu-id="2d1d2-112">0</span><span class="sxs-lookup"><span data-stu-id="2d1d2-112">0</span></span>|<span data-ttu-id="2d1d2-113">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="2d1d2-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="2d1d2-114">oneDay</span><span class="sxs-lookup"><span data-stu-id="2d1d2-114">oneDay</span></span>|<span data-ttu-id="2d1d2-115">1</span><span class="sxs-lookup"><span data-stu-id="2d1d2-115">1</span></span>|<span data-ttu-id="2d1d2-116">同步一天的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="2d1d2-116">Sync one day of email.</span></span>|
|<span data-ttu-id="2d1d2-117">threeDays</span><span class="sxs-lookup"><span data-stu-id="2d1d2-117">threeDays</span></span>|<span data-ttu-id="2d1d2-118">双面</span><span class="sxs-lookup"><span data-stu-id="2d1d2-118">2</span></span>|<span data-ttu-id="2d1d2-119">同步三天的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="2d1d2-119">Sync three days of email.</span></span>|
|<span data-ttu-id="2d1d2-120">oneWeek</span><span class="sxs-lookup"><span data-stu-id="2d1d2-120">oneWeek</span></span>|<span data-ttu-id="2d1d2-121">第三章</span><span class="sxs-lookup"><span data-stu-id="2d1d2-121">3</span></span>|<span data-ttu-id="2d1d2-122">同步一周电子邮件。</span><span class="sxs-lookup"><span data-stu-id="2d1d2-122">Sync one week of email.</span></span>|
|<span data-ttu-id="2d1d2-123">twoWeeks</span><span class="sxs-lookup"><span data-stu-id="2d1d2-123">twoWeeks</span></span>|<span data-ttu-id="2d1d2-124">4</span><span class="sxs-lookup"><span data-stu-id="2d1d2-124">4</span></span>|<span data-ttu-id="2d1d2-125">同步两周的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="2d1d2-125">Sync two weeks of email.</span></span>|
|<span data-ttu-id="2d1d2-126">oneMonth</span><span class="sxs-lookup"><span data-stu-id="2d1d2-126">oneMonth</span></span>|<span data-ttu-id="2d1d2-127">5</span><span class="sxs-lookup"><span data-stu-id="2d1d2-127">5</span></span>|<span data-ttu-id="2d1d2-128">同步一个月的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="2d1d2-128">Sync one month of email.</span></span>|
|<span data-ttu-id="2d1d2-129">不限制</span><span class="sxs-lookup"><span data-stu-id="2d1d2-129">unlimited</span></span>|<span data-ttu-id="2d1d2-130">型</span><span class="sxs-lookup"><span data-stu-id="2d1d2-130">6</span></span>|<span data-ttu-id="2d1d2-131">同步无限制的电子邮件持续时间。</span><span class="sxs-lookup"><span data-stu-id="2d1d2-131">Sync an unlimited duration of email.</span></span>|



