---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b2af0545dda4461115ed5f11975a6c9371d4010d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49283677"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="e1b49-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e1b49-103">deviceComplianceActionType enum type</span></span>

<span data-ttu-id="e1b49-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1b49-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1b49-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e1b49-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1b49-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e1b49-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1b49-107">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="e1b49-107">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="e1b49-108">成员</span><span class="sxs-lookup"><span data-stu-id="e1b49-108">Members</span></span>
|<span data-ttu-id="e1b49-109">成员</span><span class="sxs-lookup"><span data-stu-id="e1b49-109">Member</span></span>|<span data-ttu-id="e1b49-110">值</span><span class="sxs-lookup"><span data-stu-id="e1b49-110">Value</span></span>|<span data-ttu-id="e1b49-111">Description</span><span class="sxs-lookup"><span data-stu-id="e1b49-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1b49-112">noAction</span><span class="sxs-lookup"><span data-stu-id="e1b49-112">noAction</span></span>|<span data-ttu-id="e1b49-113">0</span><span class="sxs-lookup"><span data-stu-id="e1b49-113">0</span></span>|<span data-ttu-id="e1b49-114">无操作</span><span class="sxs-lookup"><span data-stu-id="e1b49-114">No Action</span></span>|
|<span data-ttu-id="e1b49-115">通告</span><span class="sxs-lookup"><span data-stu-id="e1b49-115">notification</span></span>|<span data-ttu-id="e1b49-116">1</span><span class="sxs-lookup"><span data-stu-id="e1b49-116">1</span></span>|<span data-ttu-id="e1b49-117">发送通知</span><span class="sxs-lookup"><span data-stu-id="e1b49-117">Send Notification</span></span>|
|<span data-ttu-id="e1b49-118">数据</span><span class="sxs-lookup"><span data-stu-id="e1b49-118">block</span></span>|<span data-ttu-id="e1b49-119">双面</span><span class="sxs-lookup"><span data-stu-id="e1b49-119">2</span></span>|<span data-ttu-id="e1b49-120">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="e1b49-120">Block the device in AAD</span></span>|
|<span data-ttu-id="e1b49-121">注销</span><span class="sxs-lookup"><span data-stu-id="e1b49-121">retire</span></span>|<span data-ttu-id="e1b49-122">第三章</span><span class="sxs-lookup"><span data-stu-id="e1b49-122">3</span></span>|<span data-ttu-id="e1b49-123">停用设备</span><span class="sxs-lookup"><span data-stu-id="e1b49-123">Retire the device</span></span>|
|<span data-ttu-id="e1b49-124">擦</span><span class="sxs-lookup"><span data-stu-id="e1b49-124">wipe</span></span>|<span data-ttu-id="e1b49-125">4 </span><span class="sxs-lookup"><span data-stu-id="e1b49-125">4</span></span>|<span data-ttu-id="e1b49-126">擦除设备</span><span class="sxs-lookup"><span data-stu-id="e1b49-126">Wipe the device</span></span>|
|<span data-ttu-id="e1b49-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="e1b49-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="e1b49-128">5 </span><span class="sxs-lookup"><span data-stu-id="e1b49-128">5</span></span>|<span data-ttu-id="e1b49-129">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="e1b49-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="e1b49-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="e1b49-130">pushNotification</span></span>|<span data-ttu-id="e1b49-131">9 </span><span class="sxs-lookup"><span data-stu-id="e1b49-131">9</span></span>|<span data-ttu-id="e1b49-132">将推送通知发送到设备</span><span class="sxs-lookup"><span data-stu-id="e1b49-132">Send push notification to device</span></span>|
|<span data-ttu-id="e1b49-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="e1b49-133">remoteLock</span></span>|<span data-ttu-id="e1b49-134">10  </span><span class="sxs-lookup"><span data-stu-id="e1b49-134">10</span></span>|<span data-ttu-id="e1b49-135">远程锁定设备</span><span class="sxs-lookup"><span data-stu-id="e1b49-135">Remotely lock the device</span></span>|




