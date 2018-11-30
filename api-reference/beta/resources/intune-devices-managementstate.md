---
title: 管理枚举类型
description: 管理 Microsoft Intune 中设备的状态。
ms.openlocfilehash: 554e06ff32102285d4851a19350c7c44d11d1fb4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047549"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="3796d-103">管理枚举类型</span><span class="sxs-lookup"><span data-stu-id="3796d-103">managementState enum type</span></span>

> <span data-ttu-id="3796d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3796d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3796d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3796d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3796d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3796d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3796d-107">管理 Microsoft Intune 中设备的状态。</span><span class="sxs-lookup"><span data-stu-id="3796d-107">Management state of device in Microsoft Intune.</span></span>
## <a name="members"></a><span data-ttu-id="3796d-108">成员</span><span class="sxs-lookup"><span data-stu-id="3796d-108">Members</span></span>
|<span data-ttu-id="3796d-109">成员</span><span class="sxs-lookup"><span data-stu-id="3796d-109">Member</span></span>|<span data-ttu-id="3796d-110">值</span><span class="sxs-lookup"><span data-stu-id="3796d-110">Value</span></span>|<span data-ttu-id="3796d-111">说明</span><span class="sxs-lookup"><span data-stu-id="3796d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3796d-112">托管</span><span class="sxs-lookup"><span data-stu-id="3796d-112">managed</span></span>|<span data-ttu-id="3796d-113">0</span><span class="sxs-lookup"><span data-stu-id="3796d-113">0</span></span>|<span data-ttu-id="3796d-114">在管理下的设备位于</span><span class="sxs-lookup"><span data-stu-id="3796d-114">The device is under management</span></span>|
|<span data-ttu-id="3796d-115">retirePending</span><span class="sxs-lookup"><span data-stu-id="3796d-115">retirePending</span></span>|<span data-ttu-id="3796d-116">1</span><span class="sxs-lookup"><span data-stu-id="3796d-116">1</span></span>|<span data-ttu-id="3796d-117">废弃命令正在撤消设备上并且正在 unenrolling 从管理</span><span class="sxs-lookup"><span data-stu-id="3796d-117">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="3796d-118">retireFailed</span><span class="sxs-lookup"><span data-stu-id="3796d-118">retireFailed</span></span>|<span data-ttu-id="3796d-119">2</span><span class="sxs-lookup"><span data-stu-id="3796d-119">2</span></span>|<span data-ttu-id="3796d-120">停用命令在设备上失败</span><span class="sxs-lookup"><span data-stu-id="3796d-120">Retire command failed on the device</span></span>|
|<span data-ttu-id="3796d-121">wipePending</span><span class="sxs-lookup"><span data-stu-id="3796d-121">wipePending</span></span>|<span data-ttu-id="3796d-122">3</span><span class="sxs-lookup"><span data-stu-id="3796d-122">3</span></span>|<span data-ttu-id="3796d-123">擦除命令正在撤消设备上并且正在 unenrolling 从管理</span><span class="sxs-lookup"><span data-stu-id="3796d-123">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="3796d-124">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="3796d-124">wipeFailed</span></span>|<span data-ttu-id="3796d-125">4</span><span class="sxs-lookup"><span data-stu-id="3796d-125">4</span></span>|<span data-ttu-id="3796d-126">擦除设备上失败的命令</span><span class="sxs-lookup"><span data-stu-id="3796d-126">Wipe command failed on the device</span></span>|
|<span data-ttu-id="3796d-127">不正常</span><span class="sxs-lookup"><span data-stu-id="3796d-127">unhealthy</span></span>|<span data-ttu-id="3796d-128">5</span><span class="sxs-lookup"><span data-stu-id="3796d-128">5</span></span>|<span data-ttu-id="3796d-129">设备不正常。</span><span class="sxs-lookup"><span data-stu-id="3796d-129">The device is unhealthy.</span></span>|
|<span data-ttu-id="3796d-130">deletePending</span><span class="sxs-lookup"><span data-stu-id="3796d-130">deletePending</span></span>|<span data-ttu-id="3796d-131">6</span><span class="sxs-lookup"><span data-stu-id="3796d-131">6</span></span>|<span data-ttu-id="3796d-132">删除命令正在撤消对设备</span><span class="sxs-lookup"><span data-stu-id="3796d-132">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="3796d-133">retireIssued</span><span class="sxs-lookup"><span data-stu-id="3796d-133">retireIssued</span></span>|<span data-ttu-id="3796d-134">7</span><span class="sxs-lookup"><span data-stu-id="3796d-134">7</span></span>|<span data-ttu-id="3796d-135">为设备发出了废弃命令</span><span class="sxs-lookup"><span data-stu-id="3796d-135">A retire command was issued for the device</span></span>|
|<span data-ttu-id="3796d-136">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="3796d-136">wipeIssued</span></span>|<span data-ttu-id="3796d-137">8</span><span class="sxs-lookup"><span data-stu-id="3796d-137">8</span></span>|<span data-ttu-id="3796d-138">为设备发出了擦除命令</span><span class="sxs-lookup"><span data-stu-id="3796d-138">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="3796d-139">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="3796d-139">wipeCanceled</span></span>|<span data-ttu-id="3796d-140">9</span><span class="sxs-lookup"><span data-stu-id="3796d-140">9</span></span>|<span data-ttu-id="3796d-141">此设备擦除命令已被取消</span><span class="sxs-lookup"><span data-stu-id="3796d-141">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="3796d-142">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="3796d-142">retireCanceled</span></span>|<span data-ttu-id="3796d-143">10</span><span class="sxs-lookup"><span data-stu-id="3796d-143">10</span></span>|<span data-ttu-id="3796d-144">此设备废弃命令已被取消</span><span class="sxs-lookup"><span data-stu-id="3796d-144">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="3796d-145">发现</span><span class="sxs-lookup"><span data-stu-id="3796d-145">discovered</span></span>|<span data-ttu-id="3796d-146">11</span><span class="sxs-lookup"><span data-stu-id="3796d-146">11</span></span>|<span data-ttu-id="3796d-147">发现但不是完全注册的设备。</span><span class="sxs-lookup"><span data-stu-id="3796d-147">The device is discovered but not fully enrolled.</span></span>|





