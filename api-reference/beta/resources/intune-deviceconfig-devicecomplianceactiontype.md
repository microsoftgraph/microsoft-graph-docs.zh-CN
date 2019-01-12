---
title: deviceComplianceActionType 枚举类型
description: 计划操作类型枚举
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f1856847cb8a8ecf48ee6d13067bd24515326d89
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973207"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="0a022-103">deviceComplianceActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0a022-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="0a022-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0a022-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a022-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0a022-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a022-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0a022-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a022-107">计划操作类型枚举</span><span class="sxs-lookup"><span data-stu-id="0a022-107">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="0a022-108">成员</span><span class="sxs-lookup"><span data-stu-id="0a022-108">Members</span></span>
|<span data-ttu-id="0a022-109">成员</span><span class="sxs-lookup"><span data-stu-id="0a022-109">Member</span></span>|<span data-ttu-id="0a022-110">值</span><span class="sxs-lookup"><span data-stu-id="0a022-110">Value</span></span>|<span data-ttu-id="0a022-111">说明</span><span class="sxs-lookup"><span data-stu-id="0a022-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a022-112">noAction</span><span class="sxs-lookup"><span data-stu-id="0a022-112">noAction</span></span>|<span data-ttu-id="0a022-113">0</span><span class="sxs-lookup"><span data-stu-id="0a022-113">0</span></span>|<span data-ttu-id="0a022-114">任何操作</span><span class="sxs-lookup"><span data-stu-id="0a022-114">No Action</span></span>|
|<span data-ttu-id="0a022-115">通知</span><span class="sxs-lookup"><span data-stu-id="0a022-115">notification</span></span>|<span data-ttu-id="0a022-116">1</span><span class="sxs-lookup"><span data-stu-id="0a022-116">1</span></span>|<span data-ttu-id="0a022-117">发送通知</span><span class="sxs-lookup"><span data-stu-id="0a022-117">Send Notification</span></span>|
|<span data-ttu-id="0a022-118">阻止</span><span class="sxs-lookup"><span data-stu-id="0a022-118">block</span></span>|<span data-ttu-id="0a022-119">2</span><span class="sxs-lookup"><span data-stu-id="0a022-119">2</span></span>|<span data-ttu-id="0a022-120">阻止 AAD 中的设备</span><span class="sxs-lookup"><span data-stu-id="0a022-120">Block the device in AAD</span></span>|
|<span data-ttu-id="0a022-121">停用</span><span class="sxs-lookup"><span data-stu-id="0a022-121">retire</span></span>|<span data-ttu-id="0a022-122">3</span><span class="sxs-lookup"><span data-stu-id="0a022-122">3</span></span>|<span data-ttu-id="0a022-123">停用设备</span><span class="sxs-lookup"><span data-stu-id="0a022-123">Retire the device</span></span>|
|<span data-ttu-id="0a022-124">擦除</span><span class="sxs-lookup"><span data-stu-id="0a022-124">wipe</span></span>|<span data-ttu-id="0a022-125">4</span><span class="sxs-lookup"><span data-stu-id="0a022-125">4</span></span>|<span data-ttu-id="0a022-126">擦除设备</span><span class="sxs-lookup"><span data-stu-id="0a022-126">Wipe the device</span></span>|
|<span data-ttu-id="0a022-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="0a022-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="0a022-128">5</span><span class="sxs-lookup"><span data-stu-id="0a022-128">5</span></span>|<span data-ttu-id="0a022-129">从设备中删除资源访问配置文件</span><span class="sxs-lookup"><span data-stu-id="0a022-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="0a022-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="0a022-130">pushNotification</span></span>|<span data-ttu-id="0a022-131">9</span><span class="sxs-lookup"><span data-stu-id="0a022-131">9</span></span>|<span data-ttu-id="0a022-132">向设备发送推送通知</span><span class="sxs-lookup"><span data-stu-id="0a022-132">Send push notification to device</span></span>|
|<span data-ttu-id="0a022-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="0a022-133">remoteLock</span></span>|<span data-ttu-id="0a022-134">10</span><span class="sxs-lookup"><span data-stu-id="0a022-134">10</span></span>|<span data-ttu-id="0a022-135">远程锁定设备</span><span class="sxs-lookup"><span data-stu-id="0a022-135">Remotely lock the device</span></span>|





