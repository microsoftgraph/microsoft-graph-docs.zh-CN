---
title: 管理枚举类型
description: 管理 Microsoft Intune 中设备的状态。
author: tfitzmac
ms.openlocfilehash: 530c1fec4effeb83f6efb635cd44995d904dbdcf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361059"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="adbe7-103">管理枚举类型</span><span class="sxs-lookup"><span data-stu-id="adbe7-103">managementState enum type</span></span>

> <span data-ttu-id="adbe7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="adbe7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="adbe7-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="adbe7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="adbe7-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="adbe7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="adbe7-107">管理 Microsoft Intune 中设备的状态。</span><span class="sxs-lookup"><span data-stu-id="adbe7-107">Management state of device in Microsoft Intune.</span></span>
## <a name="members"></a><span data-ttu-id="adbe7-108">成员</span><span class="sxs-lookup"><span data-stu-id="adbe7-108">Members</span></span>
|<span data-ttu-id="adbe7-109">成员</span><span class="sxs-lookup"><span data-stu-id="adbe7-109">Member</span></span>|<span data-ttu-id="adbe7-110">值</span><span class="sxs-lookup"><span data-stu-id="adbe7-110">Value</span></span>|<span data-ttu-id="adbe7-111">说明</span><span class="sxs-lookup"><span data-stu-id="adbe7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adbe7-112">托管</span><span class="sxs-lookup"><span data-stu-id="adbe7-112">managed</span></span>|<span data-ttu-id="adbe7-113">0</span><span class="sxs-lookup"><span data-stu-id="adbe7-113">0</span></span>|<span data-ttu-id="adbe7-114">在管理下的设备位于</span><span class="sxs-lookup"><span data-stu-id="adbe7-114">The device is under management</span></span>|
|<span data-ttu-id="adbe7-115">retirePending</span><span class="sxs-lookup"><span data-stu-id="adbe7-115">retirePending</span></span>|<span data-ttu-id="adbe7-116">1</span><span class="sxs-lookup"><span data-stu-id="adbe7-116">1</span></span>|<span data-ttu-id="adbe7-117">废弃命令正在撤消设备上并且正在 unenrolling 从管理</span><span class="sxs-lookup"><span data-stu-id="adbe7-117">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="adbe7-118">retireFailed</span><span class="sxs-lookup"><span data-stu-id="adbe7-118">retireFailed</span></span>|<span data-ttu-id="adbe7-119">2</span><span class="sxs-lookup"><span data-stu-id="adbe7-119">2</span></span>|<span data-ttu-id="adbe7-120">停用命令在设备上失败</span><span class="sxs-lookup"><span data-stu-id="adbe7-120">Retire command failed on the device</span></span>|
|<span data-ttu-id="adbe7-121">wipePending</span><span class="sxs-lookup"><span data-stu-id="adbe7-121">wipePending</span></span>|<span data-ttu-id="adbe7-122">3</span><span class="sxs-lookup"><span data-stu-id="adbe7-122">3</span></span>|<span data-ttu-id="adbe7-123">擦除命令正在撤消设备上并且正在 unenrolling 从管理</span><span class="sxs-lookup"><span data-stu-id="adbe7-123">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="adbe7-124">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="adbe7-124">wipeFailed</span></span>|<span data-ttu-id="adbe7-125">4</span><span class="sxs-lookup"><span data-stu-id="adbe7-125">4</span></span>|<span data-ttu-id="adbe7-126">擦除设备上失败的命令</span><span class="sxs-lookup"><span data-stu-id="adbe7-126">Wipe command failed on the device</span></span>|
|<span data-ttu-id="adbe7-127">不正常</span><span class="sxs-lookup"><span data-stu-id="adbe7-127">unhealthy</span></span>|<span data-ttu-id="adbe7-128">5</span><span class="sxs-lookup"><span data-stu-id="adbe7-128">5</span></span>|<span data-ttu-id="adbe7-129">设备不正常。</span><span class="sxs-lookup"><span data-stu-id="adbe7-129">The device is unhealthy.</span></span>|
|<span data-ttu-id="adbe7-130">deletePending</span><span class="sxs-lookup"><span data-stu-id="adbe7-130">deletePending</span></span>|<span data-ttu-id="adbe7-131">6</span><span class="sxs-lookup"><span data-stu-id="adbe7-131">6</span></span>|<span data-ttu-id="adbe7-132">删除命令正在撤消对设备</span><span class="sxs-lookup"><span data-stu-id="adbe7-132">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="adbe7-133">retireIssued</span><span class="sxs-lookup"><span data-stu-id="adbe7-133">retireIssued</span></span>|<span data-ttu-id="adbe7-134">7</span><span class="sxs-lookup"><span data-stu-id="adbe7-134">7</span></span>|<span data-ttu-id="adbe7-135">为设备发出了废弃命令</span><span class="sxs-lookup"><span data-stu-id="adbe7-135">A retire command was issued for the device</span></span>|
|<span data-ttu-id="adbe7-136">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="adbe7-136">wipeIssued</span></span>|<span data-ttu-id="adbe7-137">8</span><span class="sxs-lookup"><span data-stu-id="adbe7-137">8</span></span>|<span data-ttu-id="adbe7-138">为设备发出了擦除命令</span><span class="sxs-lookup"><span data-stu-id="adbe7-138">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="adbe7-139">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="adbe7-139">wipeCanceled</span></span>|<span data-ttu-id="adbe7-140">9</span><span class="sxs-lookup"><span data-stu-id="adbe7-140">9</span></span>|<span data-ttu-id="adbe7-141">此设备擦除命令已被取消</span><span class="sxs-lookup"><span data-stu-id="adbe7-141">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="adbe7-142">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="adbe7-142">retireCanceled</span></span>|<span data-ttu-id="adbe7-143">10</span><span class="sxs-lookup"><span data-stu-id="adbe7-143">10</span></span>|<span data-ttu-id="adbe7-144">此设备废弃命令已被取消</span><span class="sxs-lookup"><span data-stu-id="adbe7-144">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="adbe7-145">发现</span><span class="sxs-lookup"><span data-stu-id="adbe7-145">discovered</span></span>|<span data-ttu-id="adbe7-146">11</span><span class="sxs-lookup"><span data-stu-id="adbe7-146">11</span></span>|<span data-ttu-id="adbe7-147">发现但不是完全注册的设备。</span><span class="sxs-lookup"><span data-stu-id="adbe7-147">The device is discovered but not fully enrolled.</span></span>|





