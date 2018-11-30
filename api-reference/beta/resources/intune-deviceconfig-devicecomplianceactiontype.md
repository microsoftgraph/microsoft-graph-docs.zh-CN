---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
ms.openlocfilehash: 98e54f163663cc041a3e3c31123504c051884309
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044537"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="618fa-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="618fa-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="618fa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="618fa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="618fa-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="618fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="618fa-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="618fa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="618fa-107">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="618fa-107">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="618fa-108">成员</span><span class="sxs-lookup"><span data-stu-id="618fa-108">Members</span></span>
|<span data-ttu-id="618fa-109">成员</span><span class="sxs-lookup"><span data-stu-id="618fa-109">Member</span></span>|<span data-ttu-id="618fa-110">值</span><span class="sxs-lookup"><span data-stu-id="618fa-110">Value</span></span>|<span data-ttu-id="618fa-111">说明</span><span class="sxs-lookup"><span data-stu-id="618fa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="618fa-112">noAction</span><span class="sxs-lookup"><span data-stu-id="618fa-112">noAction</span></span>|<span data-ttu-id="618fa-113">0</span><span class="sxs-lookup"><span data-stu-id="618fa-113">0</span></span>|<span data-ttu-id="618fa-114">任何操作</span><span class="sxs-lookup"><span data-stu-id="618fa-114">No Action</span></span>|
|<span data-ttu-id="618fa-115">通知</span><span class="sxs-lookup"><span data-stu-id="618fa-115">notification</span></span>|<span data-ttu-id="618fa-116">1</span><span class="sxs-lookup"><span data-stu-id="618fa-116">1</span></span>|<span data-ttu-id="618fa-117">发送通知</span><span class="sxs-lookup"><span data-stu-id="618fa-117">Send Notification</span></span>|
|<span data-ttu-id="618fa-118">阻止</span><span class="sxs-lookup"><span data-stu-id="618fa-118">block</span></span>|<span data-ttu-id="618fa-119">2</span><span class="sxs-lookup"><span data-stu-id="618fa-119">2</span></span>|<span data-ttu-id="618fa-120">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="618fa-120">Block the device in AAD</span></span>|
|<span data-ttu-id="618fa-121">停用</span><span class="sxs-lookup"><span data-stu-id="618fa-121">retire</span></span>|<span data-ttu-id="618fa-122">3</span><span class="sxs-lookup"><span data-stu-id="618fa-122">3</span></span>|<span data-ttu-id="618fa-123">停用设备</span><span class="sxs-lookup"><span data-stu-id="618fa-123">Retire the device</span></span>|
|<span data-ttu-id="618fa-124">擦除</span><span class="sxs-lookup"><span data-stu-id="618fa-124">wipe</span></span>|<span data-ttu-id="618fa-125">4</span><span class="sxs-lookup"><span data-stu-id="618fa-125">4</span></span>|<span data-ttu-id="618fa-126">擦除设备</span><span class="sxs-lookup"><span data-stu-id="618fa-126">Wipe the device</span></span>|
|<span data-ttu-id="618fa-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="618fa-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="618fa-128">5</span><span class="sxs-lookup"><span data-stu-id="618fa-128">5</span></span>|<span data-ttu-id="618fa-129">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="618fa-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="618fa-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="618fa-130">pushNotification</span></span>|<span data-ttu-id="618fa-131">9</span><span class="sxs-lookup"><span data-stu-id="618fa-131">9</span></span>|<span data-ttu-id="618fa-132">向设备发送推送通知</span><span class="sxs-lookup"><span data-stu-id="618fa-132">Send push notification to device</span></span>|
|<span data-ttu-id="618fa-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="618fa-133">remoteLock</span></span>|<span data-ttu-id="618fa-134">10</span><span class="sxs-lookup"><span data-stu-id="618fa-134">10</span></span>|<span data-ttu-id="618fa-135">远程锁定设备</span><span class="sxs-lookup"><span data-stu-id="618fa-135">Remotely lock the device</span></span>|





