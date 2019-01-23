---
title: emailSyncDuration 枚举类型
description: 电子邮件同步持续时间的可能值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8bf62aea1904c0fd25867aef308ca5a269e3ea20
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399407"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="5a33a-103">emailSyncDuration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5a33a-103">emailSyncDuration enum type</span></span>

> <span data-ttu-id="5a33a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="5a33a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5a33a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5a33a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a33a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5a33a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a33a-107">电子邮件同步持续时间的可能值。</span><span class="sxs-lookup"><span data-stu-id="5a33a-107">Possible values for email sync duration.</span></span>

## <a name="members"></a><span data-ttu-id="5a33a-108">成员</span><span class="sxs-lookup"><span data-stu-id="5a33a-108">Members</span></span>
|<span data-ttu-id="5a33a-109">成员</span><span class="sxs-lookup"><span data-stu-id="5a33a-109">Member</span></span>|<span data-ttu-id="5a33a-110">值</span><span class="sxs-lookup"><span data-stu-id="5a33a-110">Value</span></span>|<span data-ttu-id="5a33a-111">说明</span><span class="sxs-lookup"><span data-stu-id="5a33a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a33a-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="5a33a-112">userDefined</span></span>|<span data-ttu-id="5a33a-113">0</span><span class="sxs-lookup"><span data-stu-id="5a33a-113">0</span></span>|<span data-ttu-id="5a33a-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="5a33a-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="5a33a-115">工期</span><span class="sxs-lookup"><span data-stu-id="5a33a-115">oneDay</span></span>|<span data-ttu-id="5a33a-116">1</span><span class="sxs-lookup"><span data-stu-id="5a33a-116">1</span></span>|<span data-ttu-id="5a33a-117">同步电子邮件中的一天。</span><span class="sxs-lookup"><span data-stu-id="5a33a-117">Sync one day of email.</span></span>|
|<span data-ttu-id="5a33a-118">3 个工作日</span><span class="sxs-lookup"><span data-stu-id="5a33a-118">threeDays</span></span>|<span data-ttu-id="5a33a-119">2</span><span class="sxs-lookup"><span data-stu-id="5a33a-119">2</span></span>|<span data-ttu-id="5a33a-120">同步三天的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="5a33a-120">Sync three days of email.</span></span>|
|<span data-ttu-id="5a33a-121">1 周时间</span><span class="sxs-lookup"><span data-stu-id="5a33a-121">oneWeek</span></span>|<span data-ttu-id="5a33a-122">3</span><span class="sxs-lookup"><span data-stu-id="5a33a-122">3</span></span>|<span data-ttu-id="5a33a-123">同步电子邮件的一周。</span><span class="sxs-lookup"><span data-stu-id="5a33a-123">Sync one week of email.</span></span>|
|<span data-ttu-id="5a33a-124">twoWeeks</span><span class="sxs-lookup"><span data-stu-id="5a33a-124">twoWeeks</span></span>|<span data-ttu-id="5a33a-125">4</span><span class="sxs-lookup"><span data-stu-id="5a33a-125">4</span></span>|<span data-ttu-id="5a33a-126">同步电子邮件的两个星期。</span><span class="sxs-lookup"><span data-stu-id="5a33a-126">Sync two weeks of email.</span></span>|
|<span data-ttu-id="5a33a-127">oneMonth</span><span class="sxs-lookup"><span data-stu-id="5a33a-127">oneMonth</span></span>|<span data-ttu-id="5a33a-128">5</span><span class="sxs-lookup"><span data-stu-id="5a33a-128">5</span></span>|<span data-ttu-id="5a33a-129">同步电子邮件的一个月。</span><span class="sxs-lookup"><span data-stu-id="5a33a-129">Sync one month of email.</span></span>|
|<span data-ttu-id="5a33a-130">无限制</span><span class="sxs-lookup"><span data-stu-id="5a33a-130">unlimited</span></span>|<span data-ttu-id="5a33a-131">6</span><span class="sxs-lookup"><span data-stu-id="5a33a-131">6</span></span>|<span data-ttu-id="5a33a-132">同步电子邮件不受限制的持续的时间。</span><span class="sxs-lookup"><span data-stu-id="5a33a-132">Sync an unlimited duration of email.</span></span>|




