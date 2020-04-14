---
title: managementState 枚举类型
description: Microsoft Intune 中设备的管理状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 88aef8765229a573818267c78e653000e3160dd3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443868"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="9a040-103">managementState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9a040-103">managementState enum type</span></span>

<span data-ttu-id="9a040-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a040-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a040-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9a040-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a040-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9a040-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a040-107">Microsoft Intune 中设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="9a040-107">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="9a040-108">成员</span><span class="sxs-lookup"><span data-stu-id="9a040-108">Members</span></span>
|<span data-ttu-id="9a040-109">成员</span><span class="sxs-lookup"><span data-stu-id="9a040-109">Member</span></span>|<span data-ttu-id="9a040-110">值</span><span class="sxs-lookup"><span data-stu-id="9a040-110">Value</span></span>|<span data-ttu-id="9a040-111">说明</span><span class="sxs-lookup"><span data-stu-id="9a040-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a040-112">managed</span><span class="sxs-lookup"><span data-stu-id="9a040-112">managed</span></span>|<span data-ttu-id="9a040-113">0</span><span class="sxs-lookup"><span data-stu-id="9a040-113">0</span></span>|<span data-ttu-id="9a040-114">设备正在管理中</span><span class="sxs-lookup"><span data-stu-id="9a040-114">The device is under management</span></span>|
|<span data-ttu-id="9a040-115">retirePending</span><span class="sxs-lookup"><span data-stu-id="9a040-115">retirePending</span></span>|<span data-ttu-id="9a040-116">1</span><span class="sxs-lookup"><span data-stu-id="9a040-116">1</span></span>|<span data-ttu-id="9a040-117">设备和 unenrolling 从管理中的过程中发生停用命令</span><span class="sxs-lookup"><span data-stu-id="9a040-117">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="9a040-118">retireFailed</span><span class="sxs-lookup"><span data-stu-id="9a040-118">retireFailed</span></span>|<span data-ttu-id="9a040-119">双面</span><span class="sxs-lookup"><span data-stu-id="9a040-119">2</span></span>|<span data-ttu-id="9a040-120">设备上的停用命令失败</span><span class="sxs-lookup"><span data-stu-id="9a040-120">Retire command failed on the device</span></span>|
|<span data-ttu-id="9a040-121">wipePending</span><span class="sxs-lookup"><span data-stu-id="9a040-121">wipePending</span></span>|<span data-ttu-id="9a040-122">第三章</span><span class="sxs-lookup"><span data-stu-id="9a040-122">3</span></span>|<span data-ttu-id="9a040-123">设备和 unenrolling 中的 "擦除" 命令在管理过程中发生</span><span class="sxs-lookup"><span data-stu-id="9a040-123">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="9a040-124">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="9a040-124">wipeFailed</span></span>|<span data-ttu-id="9a040-125">4 </span><span class="sxs-lookup"><span data-stu-id="9a040-125">4</span></span>|<span data-ttu-id="9a040-126">设备上的擦除命令失败</span><span class="sxs-lookup"><span data-stu-id="9a040-126">Wipe command failed on the device</span></span>|
|<span data-ttu-id="9a040-127">正常</span><span class="sxs-lookup"><span data-stu-id="9a040-127">unhealthy</span></span>|<span data-ttu-id="9a040-128">5 </span><span class="sxs-lookup"><span data-stu-id="9a040-128">5</span></span>|<span data-ttu-id="9a040-129">设备运行不正常。</span><span class="sxs-lookup"><span data-stu-id="9a040-129">The device is unhealthy.</span></span>|
|<span data-ttu-id="9a040-130">deletePending</span><span class="sxs-lookup"><span data-stu-id="9a040-130">deletePending</span></span>|<span data-ttu-id="9a040-131">6 </span><span class="sxs-lookup"><span data-stu-id="9a040-131">6</span></span>|<span data-ttu-id="9a040-132">在设备上发生删除命令</span><span class="sxs-lookup"><span data-stu-id="9a040-132">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="9a040-133">retireIssued</span><span class="sxs-lookup"><span data-stu-id="9a040-133">retireIssued</span></span>|<span data-ttu-id="9a040-134">7 </span><span class="sxs-lookup"><span data-stu-id="9a040-134">7</span></span>|<span data-ttu-id="9a040-135">为设备发出了停用命令</span><span class="sxs-lookup"><span data-stu-id="9a040-135">A retire command was issued for the device</span></span>|
|<span data-ttu-id="9a040-136">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="9a040-136">wipeIssued</span></span>|<span data-ttu-id="9a040-137">8 </span><span class="sxs-lookup"><span data-stu-id="9a040-137">8</span></span>|<span data-ttu-id="9a040-138">已为设备发出擦除命令</span><span class="sxs-lookup"><span data-stu-id="9a040-138">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="9a040-139">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="9a040-139">wipeCanceled</span></span>|<span data-ttu-id="9a040-140">9 </span><span class="sxs-lookup"><span data-stu-id="9a040-140">9</span></span>|<span data-ttu-id="9a040-141">已取消此设备的擦除命令</span><span class="sxs-lookup"><span data-stu-id="9a040-141">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="9a040-142">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="9a040-142">retireCanceled</span></span>|<span data-ttu-id="9a040-143">10 </span><span class="sxs-lookup"><span data-stu-id="9a040-143">10</span></span>|<span data-ttu-id="9a040-144">已取消此设备的停用命令</span><span class="sxs-lookup"><span data-stu-id="9a040-144">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="9a040-145">探索</span><span class="sxs-lookup"><span data-stu-id="9a040-145">discovered</span></span>|<span data-ttu-id="9a040-146">11x17</span><span class="sxs-lookup"><span data-stu-id="9a040-146">11</span></span>|<span data-ttu-id="9a040-147">设备已被发现，但未完全注册。</span><span class="sxs-lookup"><span data-stu-id="9a040-147">The device is discovered but not fully enrolled.</span></span>|



