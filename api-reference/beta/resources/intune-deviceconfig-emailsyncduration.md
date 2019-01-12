---
title: emailSyncDuration 枚举类型
description: 电子邮件同步持续时间的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fcabbe69c10cd490732560ea856c39c5cfd8cb44
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986409"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="efaad-103">emailSyncDuration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="efaad-103">emailSyncDuration enum type</span></span>

> <span data-ttu-id="efaad-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="efaad-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="efaad-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="efaad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="efaad-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="efaad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="efaad-107">电子邮件同步持续时间的可能值。</span><span class="sxs-lookup"><span data-stu-id="efaad-107">Possible values for email sync duration.</span></span>
## <a name="members"></a><span data-ttu-id="efaad-108">成员</span><span class="sxs-lookup"><span data-stu-id="efaad-108">Members</span></span>
|<span data-ttu-id="efaad-109">成员</span><span class="sxs-lookup"><span data-stu-id="efaad-109">Member</span></span>|<span data-ttu-id="efaad-110">值</span><span class="sxs-lookup"><span data-stu-id="efaad-110">Value</span></span>|<span data-ttu-id="efaad-111">说明</span><span class="sxs-lookup"><span data-stu-id="efaad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efaad-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="efaad-112">userDefined</span></span>|<span data-ttu-id="efaad-113">0</span><span class="sxs-lookup"><span data-stu-id="efaad-113">0</span></span>|<span data-ttu-id="efaad-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="efaad-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="efaad-115">工期</span><span class="sxs-lookup"><span data-stu-id="efaad-115">oneDay</span></span>|<span data-ttu-id="efaad-116">1</span><span class="sxs-lookup"><span data-stu-id="efaad-116">1</span></span>|<span data-ttu-id="efaad-117">同步电子邮件中的一天。</span><span class="sxs-lookup"><span data-stu-id="efaad-117">Sync one day of email.</span></span>|
|<span data-ttu-id="efaad-118">3 个工作日</span><span class="sxs-lookup"><span data-stu-id="efaad-118">threeDays</span></span>|<span data-ttu-id="efaad-119">2</span><span class="sxs-lookup"><span data-stu-id="efaad-119">2</span></span>|<span data-ttu-id="efaad-120">同步三天的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="efaad-120">Sync three days of email.</span></span>|
|<span data-ttu-id="efaad-121">1 周时间</span><span class="sxs-lookup"><span data-stu-id="efaad-121">oneWeek</span></span>|<span data-ttu-id="efaad-122">3</span><span class="sxs-lookup"><span data-stu-id="efaad-122">3</span></span>|<span data-ttu-id="efaad-123">同步电子邮件的一周。</span><span class="sxs-lookup"><span data-stu-id="efaad-123">Sync one week of email.</span></span>|
|<span data-ttu-id="efaad-124">twoWeeks</span><span class="sxs-lookup"><span data-stu-id="efaad-124">twoWeeks</span></span>|<span data-ttu-id="efaad-125">4</span><span class="sxs-lookup"><span data-stu-id="efaad-125">4</span></span>|<span data-ttu-id="efaad-126">同步电子邮件的两个星期。</span><span class="sxs-lookup"><span data-stu-id="efaad-126">Sync two weeks of email.</span></span>|
|<span data-ttu-id="efaad-127">oneMonth</span><span class="sxs-lookup"><span data-stu-id="efaad-127">oneMonth</span></span>|<span data-ttu-id="efaad-128">5</span><span class="sxs-lookup"><span data-stu-id="efaad-128">5</span></span>|<span data-ttu-id="efaad-129">同步电子邮件的一个月。</span><span class="sxs-lookup"><span data-stu-id="efaad-129">Sync one month of email.</span></span>|
|<span data-ttu-id="efaad-130">无限制</span><span class="sxs-lookup"><span data-stu-id="efaad-130">unlimited</span></span>|<span data-ttu-id="efaad-131">6</span><span class="sxs-lookup"><span data-stu-id="efaad-131">6</span></span>|<span data-ttu-id="efaad-132">同步电子邮件不受限制的持续的时间。</span><span class="sxs-lookup"><span data-stu-id="efaad-132">Sync an unlimited duration of email.</span></span>|





