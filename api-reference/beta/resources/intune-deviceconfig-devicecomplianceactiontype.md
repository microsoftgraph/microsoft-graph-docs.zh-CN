---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05f9df39c563a47fa571a4badcf789ea4ddb08b1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979527"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="86e3f-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="86e3f-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="86e3f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="86e3f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86e3f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="86e3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86e3f-106">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="86e3f-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="86e3f-107">成员</span><span class="sxs-lookup"><span data-stu-id="86e3f-107">Members</span></span>
|<span data-ttu-id="86e3f-108">成员</span><span class="sxs-lookup"><span data-stu-id="86e3f-108">Member</span></span>|<span data-ttu-id="86e3f-109">值</span><span class="sxs-lookup"><span data-stu-id="86e3f-109">Value</span></span>|<span data-ttu-id="86e3f-110">说明</span><span class="sxs-lookup"><span data-stu-id="86e3f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86e3f-111">noAction</span><span class="sxs-lookup"><span data-stu-id="86e3f-111">noAction</span></span>|<span data-ttu-id="86e3f-112">0</span><span class="sxs-lookup"><span data-stu-id="86e3f-112">0</span></span>|<span data-ttu-id="86e3f-113">无操作</span><span class="sxs-lookup"><span data-stu-id="86e3f-113">No Action</span></span>|
|<span data-ttu-id="86e3f-114">通告</span><span class="sxs-lookup"><span data-stu-id="86e3f-114">notification</span></span>|<span data-ttu-id="86e3f-115">1</span><span class="sxs-lookup"><span data-stu-id="86e3f-115">1</span></span>|<span data-ttu-id="86e3f-116">发送通知</span><span class="sxs-lookup"><span data-stu-id="86e3f-116">Send Notification</span></span>|
|<span data-ttu-id="86e3f-117">数据</span><span class="sxs-lookup"><span data-stu-id="86e3f-117">block</span></span>|<span data-ttu-id="86e3f-118">双面</span><span class="sxs-lookup"><span data-stu-id="86e3f-118">2</span></span>|<span data-ttu-id="86e3f-119">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="86e3f-119">Block the device in AAD</span></span>|
|<span data-ttu-id="86e3f-120">注销</span><span class="sxs-lookup"><span data-stu-id="86e3f-120">retire</span></span>|<span data-ttu-id="86e3f-121">第三章</span><span class="sxs-lookup"><span data-stu-id="86e3f-121">3</span></span>|<span data-ttu-id="86e3f-122">停用设备</span><span class="sxs-lookup"><span data-stu-id="86e3f-122">Retire the device</span></span>|
|<span data-ttu-id="86e3f-123">擦</span><span class="sxs-lookup"><span data-stu-id="86e3f-123">wipe</span></span>|<span data-ttu-id="86e3f-124">4</span><span class="sxs-lookup"><span data-stu-id="86e3f-124">4</span></span>|<span data-ttu-id="86e3f-125">擦除设备</span><span class="sxs-lookup"><span data-stu-id="86e3f-125">Wipe the device</span></span>|
|<span data-ttu-id="86e3f-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="86e3f-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="86e3f-127">5</span><span class="sxs-lookup"><span data-stu-id="86e3f-127">5</span></span>|<span data-ttu-id="86e3f-128">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="86e3f-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="86e3f-129">pushNotification</span><span class="sxs-lookup"><span data-stu-id="86e3f-129">pushNotification</span></span>|<span data-ttu-id="86e3f-130">第</span><span class="sxs-lookup"><span data-stu-id="86e3f-130">9</span></span>|<span data-ttu-id="86e3f-131">将推送通知发送到设备</span><span class="sxs-lookup"><span data-stu-id="86e3f-131">Send push notification to device</span></span>|
|<span data-ttu-id="86e3f-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="86e3f-132">remoteLock</span></span>|<span data-ttu-id="86e3f-133">10 </span><span class="sxs-lookup"><span data-stu-id="86e3f-133">10</span></span>|<span data-ttu-id="86e3f-134">远程锁定设备</span><span class="sxs-lookup"><span data-stu-id="86e3f-134">Remotely lock the device</span></span>|





