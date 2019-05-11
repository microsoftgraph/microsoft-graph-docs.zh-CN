---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37caa3ca741c752a67a9f90222856b31fa4978c3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947202"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="e4359-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e4359-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="e4359-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e4359-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4359-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4359-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4359-106">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="e4359-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="e4359-107">成员</span><span class="sxs-lookup"><span data-stu-id="e4359-107">Members</span></span>
|<span data-ttu-id="e4359-108">成员</span><span class="sxs-lookup"><span data-stu-id="e4359-108">Member</span></span>|<span data-ttu-id="e4359-109">值</span><span class="sxs-lookup"><span data-stu-id="e4359-109">Value</span></span>|<span data-ttu-id="e4359-110">说明</span><span class="sxs-lookup"><span data-stu-id="e4359-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4359-111">noAction</span><span class="sxs-lookup"><span data-stu-id="e4359-111">noAction</span></span>|<span data-ttu-id="e4359-112">0</span><span class="sxs-lookup"><span data-stu-id="e4359-112">0</span></span>|<span data-ttu-id="e4359-113">无操作</span><span class="sxs-lookup"><span data-stu-id="e4359-113">No Action</span></span>|
|<span data-ttu-id="e4359-114">通告</span><span class="sxs-lookup"><span data-stu-id="e4359-114">notification</span></span>|<span data-ttu-id="e4359-115">1</span><span class="sxs-lookup"><span data-stu-id="e4359-115">1</span></span>|<span data-ttu-id="e4359-116">发送通知</span><span class="sxs-lookup"><span data-stu-id="e4359-116">Send Notification</span></span>|
|<span data-ttu-id="e4359-117">数据</span><span class="sxs-lookup"><span data-stu-id="e4359-117">block</span></span>|<span data-ttu-id="e4359-118">双面</span><span class="sxs-lookup"><span data-stu-id="e4359-118">2</span></span>|<span data-ttu-id="e4359-119">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="e4359-119">Block the device in AAD</span></span>|
|<span data-ttu-id="e4359-120">注销</span><span class="sxs-lookup"><span data-stu-id="e4359-120">retire</span></span>|<span data-ttu-id="e4359-121">第三章</span><span class="sxs-lookup"><span data-stu-id="e4359-121">3</span></span>|<span data-ttu-id="e4359-122">停用设备</span><span class="sxs-lookup"><span data-stu-id="e4359-122">Retire the device</span></span>|
|<span data-ttu-id="e4359-123">擦</span><span class="sxs-lookup"><span data-stu-id="e4359-123">wipe</span></span>|<span data-ttu-id="e4359-124">4</span><span class="sxs-lookup"><span data-stu-id="e4359-124">4</span></span>|<span data-ttu-id="e4359-125">擦除设备</span><span class="sxs-lookup"><span data-stu-id="e4359-125">Wipe the device</span></span>|
|<span data-ttu-id="e4359-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="e4359-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="e4359-127">5</span><span class="sxs-lookup"><span data-stu-id="e4359-127">5</span></span>|<span data-ttu-id="e4359-128">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="e4359-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="e4359-129">pushNotification</span><span class="sxs-lookup"><span data-stu-id="e4359-129">pushNotification</span></span>|<span data-ttu-id="e4359-130">第</span><span class="sxs-lookup"><span data-stu-id="e4359-130">9</span></span>|<span data-ttu-id="e4359-131">将推送通知发送到设备</span><span class="sxs-lookup"><span data-stu-id="e4359-131">Send push notification to device</span></span>|
|<span data-ttu-id="e4359-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="e4359-132">remoteLock</span></span>|<span data-ttu-id="e4359-133">10 </span><span class="sxs-lookup"><span data-stu-id="e4359-133">10</span></span>|<span data-ttu-id="e4359-134">远程锁定设备</span><span class="sxs-lookup"><span data-stu-id="e4359-134">Remotely lock the device</span></span>|




