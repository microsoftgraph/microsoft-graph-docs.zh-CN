---
title: emailSyncDuration 枚举类型
description: 电子邮件同步持续时间的可能值。
author: tfitzmac
ms.openlocfilehash: 512e20ad13c13fdf92e45cfe0a37792d97e17fbb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361164"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="a442f-103">emailSyncDuration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a442f-103">emailSyncDuration enum type</span></span>

> <span data-ttu-id="a442f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a442f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a442f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a442f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a442f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a442f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a442f-107">电子邮件同步持续时间的可能值。</span><span class="sxs-lookup"><span data-stu-id="a442f-107">Possible values for email sync duration.</span></span>
## <a name="members"></a><span data-ttu-id="a442f-108">成员</span><span class="sxs-lookup"><span data-stu-id="a442f-108">Members</span></span>
|<span data-ttu-id="a442f-109">成员</span><span class="sxs-lookup"><span data-stu-id="a442f-109">Member</span></span>|<span data-ttu-id="a442f-110">值</span><span class="sxs-lookup"><span data-stu-id="a442f-110">Value</span></span>|<span data-ttu-id="a442f-111">说明</span><span class="sxs-lookup"><span data-stu-id="a442f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a442f-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="a442f-112">userDefined</span></span>|<span data-ttu-id="a442f-113">0</span><span class="sxs-lookup"><span data-stu-id="a442f-113">0</span></span>|<span data-ttu-id="a442f-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="a442f-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="a442f-115">工期</span><span class="sxs-lookup"><span data-stu-id="a442f-115">oneDay</span></span>|<span data-ttu-id="a442f-116">1</span><span class="sxs-lookup"><span data-stu-id="a442f-116">1</span></span>|<span data-ttu-id="a442f-117">同步电子邮件中的一天。</span><span class="sxs-lookup"><span data-stu-id="a442f-117">Sync one day of email.</span></span>|
|<span data-ttu-id="a442f-118">3 个工作日</span><span class="sxs-lookup"><span data-stu-id="a442f-118">threeDays</span></span>|<span data-ttu-id="a442f-119">2</span><span class="sxs-lookup"><span data-stu-id="a442f-119">2</span></span>|<span data-ttu-id="a442f-120">同步三天的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="a442f-120">Sync three days of email.</span></span>|
|<span data-ttu-id="a442f-121">1 周时间</span><span class="sxs-lookup"><span data-stu-id="a442f-121">oneWeek</span></span>|<span data-ttu-id="a442f-122">3</span><span class="sxs-lookup"><span data-stu-id="a442f-122">3</span></span>|<span data-ttu-id="a442f-123">同步电子邮件的一周。</span><span class="sxs-lookup"><span data-stu-id="a442f-123">Sync one week of email.</span></span>|
|<span data-ttu-id="a442f-124">twoWeeks</span><span class="sxs-lookup"><span data-stu-id="a442f-124">twoWeeks</span></span>|<span data-ttu-id="a442f-125">4</span><span class="sxs-lookup"><span data-stu-id="a442f-125">4</span></span>|<span data-ttu-id="a442f-126">同步电子邮件的两个星期。</span><span class="sxs-lookup"><span data-stu-id="a442f-126">Sync two weeks of email.</span></span>|
|<span data-ttu-id="a442f-127">oneMonth</span><span class="sxs-lookup"><span data-stu-id="a442f-127">oneMonth</span></span>|<span data-ttu-id="a442f-128">5</span><span class="sxs-lookup"><span data-stu-id="a442f-128">5</span></span>|<span data-ttu-id="a442f-129">同步电子邮件的一个月。</span><span class="sxs-lookup"><span data-stu-id="a442f-129">Sync one month of email.</span></span>|
|<span data-ttu-id="a442f-130">无限制</span><span class="sxs-lookup"><span data-stu-id="a442f-130">unlimited</span></span>|<span data-ttu-id="a442f-131">6</span><span class="sxs-lookup"><span data-stu-id="a442f-131">6</span></span>|<span data-ttu-id="a442f-132">同步电子邮件不受限制的持续的时间。</span><span class="sxs-lookup"><span data-stu-id="a442f-132">Sync an unlimited duration of email.</span></span>|





