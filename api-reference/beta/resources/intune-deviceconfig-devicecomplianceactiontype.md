---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 33b18120e5ae0d928fbd7a7a42e87bf7f71d10ec
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735846"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="c6b60-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c6b60-103">deviceComplianceActionType enum type</span></span>

<span data-ttu-id="c6b60-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6b60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6b60-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c6b60-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6b60-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c6b60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6b60-107">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="c6b60-107">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="c6b60-108">成员</span><span class="sxs-lookup"><span data-stu-id="c6b60-108">Members</span></span>
|<span data-ttu-id="c6b60-109">成员</span><span class="sxs-lookup"><span data-stu-id="c6b60-109">Member</span></span>|<span data-ttu-id="c6b60-110">值</span><span class="sxs-lookup"><span data-stu-id="c6b60-110">Value</span></span>|<span data-ttu-id="c6b60-111">说明</span><span class="sxs-lookup"><span data-stu-id="c6b60-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6b60-112">noAction</span><span class="sxs-lookup"><span data-stu-id="c6b60-112">noAction</span></span>|<span data-ttu-id="c6b60-113">0</span><span class="sxs-lookup"><span data-stu-id="c6b60-113">0</span></span>|<span data-ttu-id="c6b60-114">无操作</span><span class="sxs-lookup"><span data-stu-id="c6b60-114">No Action</span></span>|
|<span data-ttu-id="c6b60-115">通告</span><span class="sxs-lookup"><span data-stu-id="c6b60-115">notification</span></span>|<span data-ttu-id="c6b60-116">1</span><span class="sxs-lookup"><span data-stu-id="c6b60-116">1</span></span>|<span data-ttu-id="c6b60-117">发送通知</span><span class="sxs-lookup"><span data-stu-id="c6b60-117">Send Notification</span></span>|
|<span data-ttu-id="c6b60-118">数据</span><span class="sxs-lookup"><span data-stu-id="c6b60-118">block</span></span>|<span data-ttu-id="c6b60-119">双面</span><span class="sxs-lookup"><span data-stu-id="c6b60-119">2</span></span>|<span data-ttu-id="c6b60-120">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="c6b60-120">Block the device in AAD</span></span>|
|<span data-ttu-id="c6b60-121">注销</span><span class="sxs-lookup"><span data-stu-id="c6b60-121">retire</span></span>|<span data-ttu-id="c6b60-122">第三章</span><span class="sxs-lookup"><span data-stu-id="c6b60-122">3</span></span>|<span data-ttu-id="c6b60-123">停用设备</span><span class="sxs-lookup"><span data-stu-id="c6b60-123">Retire the device</span></span>|
|<span data-ttu-id="c6b60-124">擦</span><span class="sxs-lookup"><span data-stu-id="c6b60-124">wipe</span></span>|<span data-ttu-id="c6b60-125">4 </span><span class="sxs-lookup"><span data-stu-id="c6b60-125">4</span></span>|<span data-ttu-id="c6b60-126">擦除设备</span><span class="sxs-lookup"><span data-stu-id="c6b60-126">Wipe the device</span></span>|
|<span data-ttu-id="c6b60-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="c6b60-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="c6b60-128">5 </span><span class="sxs-lookup"><span data-stu-id="c6b60-128">5</span></span>|<span data-ttu-id="c6b60-129">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="c6b60-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="c6b60-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="c6b60-130">pushNotification</span></span>|<span data-ttu-id="c6b60-131">9 </span><span class="sxs-lookup"><span data-stu-id="c6b60-131">9</span></span>|<span data-ttu-id="c6b60-132">将推送通知发送到设备</span><span class="sxs-lookup"><span data-stu-id="c6b60-132">Send push notification to device</span></span>|
|<span data-ttu-id="c6b60-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="c6b60-133">remoteLock</span></span>|<span data-ttu-id="c6b60-134">10  </span><span class="sxs-lookup"><span data-stu-id="c6b60-134">10</span></span>|<span data-ttu-id="c6b60-135">远程锁定设备</span><span class="sxs-lookup"><span data-stu-id="c6b60-135">Remotely lock the device</span></span>|





