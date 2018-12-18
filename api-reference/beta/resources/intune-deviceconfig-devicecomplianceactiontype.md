---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: tfitzmac
ms.openlocfilehash: 9fd0a8bd045ad04fe0acf55f899e693d7fcce5d0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335684"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="09b5e-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="09b5e-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="09b5e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="09b5e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09b5e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="09b5e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09b5e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="09b5e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09b5e-107">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="09b5e-107">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="09b5e-108">成员</span><span class="sxs-lookup"><span data-stu-id="09b5e-108">Members</span></span>
|<span data-ttu-id="09b5e-109">成员</span><span class="sxs-lookup"><span data-stu-id="09b5e-109">Member</span></span>|<span data-ttu-id="09b5e-110">值</span><span class="sxs-lookup"><span data-stu-id="09b5e-110">Value</span></span>|<span data-ttu-id="09b5e-111">说明</span><span class="sxs-lookup"><span data-stu-id="09b5e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09b5e-112">noAction</span><span class="sxs-lookup"><span data-stu-id="09b5e-112">noAction</span></span>|<span data-ttu-id="09b5e-113">0</span><span class="sxs-lookup"><span data-stu-id="09b5e-113">0</span></span>|<span data-ttu-id="09b5e-114">任何操作</span><span class="sxs-lookup"><span data-stu-id="09b5e-114">No Action</span></span>|
|<span data-ttu-id="09b5e-115">通知</span><span class="sxs-lookup"><span data-stu-id="09b5e-115">notification</span></span>|<span data-ttu-id="09b5e-116">1</span><span class="sxs-lookup"><span data-stu-id="09b5e-116">1</span></span>|<span data-ttu-id="09b5e-117">发送通知</span><span class="sxs-lookup"><span data-stu-id="09b5e-117">Send Notification</span></span>|
|<span data-ttu-id="09b5e-118">阻止</span><span class="sxs-lookup"><span data-stu-id="09b5e-118">block</span></span>|<span data-ttu-id="09b5e-119">2</span><span class="sxs-lookup"><span data-stu-id="09b5e-119">2</span></span>|<span data-ttu-id="09b5e-120">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="09b5e-120">Block the device in AAD</span></span>|
|<span data-ttu-id="09b5e-121">停用</span><span class="sxs-lookup"><span data-stu-id="09b5e-121">retire</span></span>|<span data-ttu-id="09b5e-122">3</span><span class="sxs-lookup"><span data-stu-id="09b5e-122">3</span></span>|<span data-ttu-id="09b5e-123">停用设备</span><span class="sxs-lookup"><span data-stu-id="09b5e-123">Retire the device</span></span>|
|<span data-ttu-id="09b5e-124">擦除</span><span class="sxs-lookup"><span data-stu-id="09b5e-124">wipe</span></span>|<span data-ttu-id="09b5e-125">4</span><span class="sxs-lookup"><span data-stu-id="09b5e-125">4</span></span>|<span data-ttu-id="09b5e-126">擦除设备</span><span class="sxs-lookup"><span data-stu-id="09b5e-126">Wipe the device</span></span>|
|<span data-ttu-id="09b5e-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="09b5e-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="09b5e-128">5</span><span class="sxs-lookup"><span data-stu-id="09b5e-128">5</span></span>|<span data-ttu-id="09b5e-129">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="09b5e-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="09b5e-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="09b5e-130">pushNotification</span></span>|<span data-ttu-id="09b5e-131">9</span><span class="sxs-lookup"><span data-stu-id="09b5e-131">9</span></span>|<span data-ttu-id="09b5e-132">向设备发送推送通知</span><span class="sxs-lookup"><span data-stu-id="09b5e-132">Send push notification to device</span></span>|
|<span data-ttu-id="09b5e-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="09b5e-133">remoteLock</span></span>|<span data-ttu-id="09b5e-134">10</span><span class="sxs-lookup"><span data-stu-id="09b5e-134">10</span></span>|<span data-ttu-id="09b5e-135">远程锁定设备</span><span class="sxs-lookup"><span data-stu-id="09b5e-135">Remotely lock the device</span></span>|





