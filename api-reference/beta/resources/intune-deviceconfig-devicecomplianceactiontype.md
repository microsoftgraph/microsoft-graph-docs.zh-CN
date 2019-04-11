---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba07cb2b0fe076642cb1157a5d5df09a04a63a47
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772942"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="b8406-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b8406-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="b8406-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b8406-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8406-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b8406-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8406-106">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="b8406-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="b8406-107">成员</span><span class="sxs-lookup"><span data-stu-id="b8406-107">Members</span></span>
|<span data-ttu-id="b8406-108">成员</span><span class="sxs-lookup"><span data-stu-id="b8406-108">Member</span></span>|<span data-ttu-id="b8406-109">值</span><span class="sxs-lookup"><span data-stu-id="b8406-109">Value</span></span>|<span data-ttu-id="b8406-110">说明</span><span class="sxs-lookup"><span data-stu-id="b8406-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8406-111">noAction</span><span class="sxs-lookup"><span data-stu-id="b8406-111">noAction</span></span>|<span data-ttu-id="b8406-112">0</span><span class="sxs-lookup"><span data-stu-id="b8406-112">0</span></span>|<span data-ttu-id="b8406-113">无操作</span><span class="sxs-lookup"><span data-stu-id="b8406-113">No Action</span></span>|
|<span data-ttu-id="b8406-114">通告</span><span class="sxs-lookup"><span data-stu-id="b8406-114">notification</span></span>|<span data-ttu-id="b8406-115">1</span><span class="sxs-lookup"><span data-stu-id="b8406-115">1</span></span>|<span data-ttu-id="b8406-116">发送通知</span><span class="sxs-lookup"><span data-stu-id="b8406-116">Send Notification</span></span>|
|<span data-ttu-id="b8406-117">数据</span><span class="sxs-lookup"><span data-stu-id="b8406-117">block</span></span>|<span data-ttu-id="b8406-118">双面</span><span class="sxs-lookup"><span data-stu-id="b8406-118">2</span></span>|<span data-ttu-id="b8406-119">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="b8406-119">Block the device in AAD</span></span>|
|<span data-ttu-id="b8406-120">注销</span><span class="sxs-lookup"><span data-stu-id="b8406-120">retire</span></span>|<span data-ttu-id="b8406-121">第三章</span><span class="sxs-lookup"><span data-stu-id="b8406-121">3</span></span>|<span data-ttu-id="b8406-122">停用设备</span><span class="sxs-lookup"><span data-stu-id="b8406-122">Retire the device</span></span>|
|<span data-ttu-id="b8406-123">擦</span><span class="sxs-lookup"><span data-stu-id="b8406-123">wipe</span></span>|<span data-ttu-id="b8406-124">4</span><span class="sxs-lookup"><span data-stu-id="b8406-124">4</span></span>|<span data-ttu-id="b8406-125">擦除设备</span><span class="sxs-lookup"><span data-stu-id="b8406-125">Wipe the device</span></span>|
|<span data-ttu-id="b8406-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="b8406-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="b8406-127">5</span><span class="sxs-lookup"><span data-stu-id="b8406-127">5</span></span>|<span data-ttu-id="b8406-128">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="b8406-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="b8406-129">pushNotification</span><span class="sxs-lookup"><span data-stu-id="b8406-129">pushNotification</span></span>|<span data-ttu-id="b8406-130">第</span><span class="sxs-lookup"><span data-stu-id="b8406-130">9</span></span>|<span data-ttu-id="b8406-131">将推送通知发送到设备</span><span class="sxs-lookup"><span data-stu-id="b8406-131">Send push notification to device</span></span>|
|<span data-ttu-id="b8406-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="b8406-132">remoteLock</span></span>|<span data-ttu-id="b8406-133">10</span><span class="sxs-lookup"><span data-stu-id="b8406-133">10</span></span>|<span data-ttu-id="b8406-134">远程锁定设备</span><span class="sxs-lookup"><span data-stu-id="b8406-134">Remotely lock the device</span></span>|





