---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bff5247237cc0d6daf45515c5bdbaaa3e675017a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526717"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="01743-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="01743-103">deviceComplianceActionType enum type</span></span>

<span data-ttu-id="01743-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="01743-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01743-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="01743-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01743-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="01743-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01743-107">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="01743-107">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="01743-108">成员</span><span class="sxs-lookup"><span data-stu-id="01743-108">Members</span></span>
|<span data-ttu-id="01743-109">成员</span><span class="sxs-lookup"><span data-stu-id="01743-109">Member</span></span>|<span data-ttu-id="01743-110">值</span><span class="sxs-lookup"><span data-stu-id="01743-110">Value</span></span>|<span data-ttu-id="01743-111">说明</span><span class="sxs-lookup"><span data-stu-id="01743-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01743-112">noAction</span><span class="sxs-lookup"><span data-stu-id="01743-112">noAction</span></span>|<span data-ttu-id="01743-113">0</span><span class="sxs-lookup"><span data-stu-id="01743-113">0</span></span>|<span data-ttu-id="01743-114">无操作</span><span class="sxs-lookup"><span data-stu-id="01743-114">No Action</span></span>|
|<span data-ttu-id="01743-115">通告</span><span class="sxs-lookup"><span data-stu-id="01743-115">notification</span></span>|<span data-ttu-id="01743-116">1 </span><span class="sxs-lookup"><span data-stu-id="01743-116">1</span></span>|<span data-ttu-id="01743-117">发送通知</span><span class="sxs-lookup"><span data-stu-id="01743-117">Send Notification</span></span>|
|<span data-ttu-id="01743-118">数据</span><span class="sxs-lookup"><span data-stu-id="01743-118">block</span></span>|<span data-ttu-id="01743-119">2 </span><span class="sxs-lookup"><span data-stu-id="01743-119">2</span></span>|<span data-ttu-id="01743-120">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="01743-120">Block the device in AAD</span></span>|
|<span data-ttu-id="01743-121">注销</span><span class="sxs-lookup"><span data-stu-id="01743-121">retire</span></span>|<span data-ttu-id="01743-122">3 </span><span class="sxs-lookup"><span data-stu-id="01743-122">3</span></span>|<span data-ttu-id="01743-123">停用设备</span><span class="sxs-lookup"><span data-stu-id="01743-123">Retire the device</span></span>|
|<span data-ttu-id="01743-124">擦</span><span class="sxs-lookup"><span data-stu-id="01743-124">wipe</span></span>|<span data-ttu-id="01743-125">4 </span><span class="sxs-lookup"><span data-stu-id="01743-125">4</span></span>|<span data-ttu-id="01743-126">擦除设备</span><span class="sxs-lookup"><span data-stu-id="01743-126">Wipe the device</span></span>|
|<span data-ttu-id="01743-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="01743-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="01743-128">5 </span><span class="sxs-lookup"><span data-stu-id="01743-128">5</span></span>|<span data-ttu-id="01743-129">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="01743-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="01743-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="01743-130">pushNotification</span></span>|<span data-ttu-id="01743-131">9 </span><span class="sxs-lookup"><span data-stu-id="01743-131">9</span></span>|<span data-ttu-id="01743-132">将推送通知发送到设备</span><span class="sxs-lookup"><span data-stu-id="01743-132">Send push notification to device</span></span>|
|<span data-ttu-id="01743-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="01743-133">remoteLock</span></span>|<span data-ttu-id="01743-134">10 </span><span class="sxs-lookup"><span data-stu-id="01743-134">10</span></span>|<span data-ttu-id="01743-135">远程锁定设备</span><span class="sxs-lookup"><span data-stu-id="01743-135">Remotely lock the device</span></span>|



