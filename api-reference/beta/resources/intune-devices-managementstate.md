---
title: managementState 枚举类型
description: Microsoft Intune 中设备的管理状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8e348caee303ba1aeccedbfe787cb2c030f06c7b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528524"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="f7820-103">managementState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f7820-103">managementState enum type</span></span>

<span data-ttu-id="f7820-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f7820-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7820-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f7820-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7820-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7820-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7820-107">Microsoft Intune 中设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="f7820-107">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="f7820-108">成员</span><span class="sxs-lookup"><span data-stu-id="f7820-108">Members</span></span>
|<span data-ttu-id="f7820-109">成员</span><span class="sxs-lookup"><span data-stu-id="f7820-109">Member</span></span>|<span data-ttu-id="f7820-110">值</span><span class="sxs-lookup"><span data-stu-id="f7820-110">Value</span></span>|<span data-ttu-id="f7820-111">说明</span><span class="sxs-lookup"><span data-stu-id="f7820-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7820-112">managed</span><span class="sxs-lookup"><span data-stu-id="f7820-112">managed</span></span>|<span data-ttu-id="f7820-113">0</span><span class="sxs-lookup"><span data-stu-id="f7820-113">0</span></span>|<span data-ttu-id="f7820-114">设备正在管理中</span><span class="sxs-lookup"><span data-stu-id="f7820-114">The device is under management</span></span>|
|<span data-ttu-id="f7820-115">retirePending</span><span class="sxs-lookup"><span data-stu-id="f7820-115">retirePending</span></span>|<span data-ttu-id="f7820-116">1 </span><span class="sxs-lookup"><span data-stu-id="f7820-116">1</span></span>|<span data-ttu-id="f7820-117">设备和 unenrolling 从管理中的过程中发生停用命令</span><span class="sxs-lookup"><span data-stu-id="f7820-117">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="f7820-118">retireFailed</span><span class="sxs-lookup"><span data-stu-id="f7820-118">retireFailed</span></span>|<span data-ttu-id="f7820-119">2 </span><span class="sxs-lookup"><span data-stu-id="f7820-119">2</span></span>|<span data-ttu-id="f7820-120">设备上的停用命令失败</span><span class="sxs-lookup"><span data-stu-id="f7820-120">Retire command failed on the device</span></span>|
|<span data-ttu-id="f7820-121">wipePending</span><span class="sxs-lookup"><span data-stu-id="f7820-121">wipePending</span></span>|<span data-ttu-id="f7820-122">3 </span><span class="sxs-lookup"><span data-stu-id="f7820-122">3</span></span>|<span data-ttu-id="f7820-123">设备和 unenrolling 中的 "擦除" 命令在管理过程中发生</span><span class="sxs-lookup"><span data-stu-id="f7820-123">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="f7820-124">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="f7820-124">wipeFailed</span></span>|<span data-ttu-id="f7820-125">4 </span><span class="sxs-lookup"><span data-stu-id="f7820-125">4</span></span>|<span data-ttu-id="f7820-126">设备上的擦除命令失败</span><span class="sxs-lookup"><span data-stu-id="f7820-126">Wipe command failed on the device</span></span>|
|<span data-ttu-id="f7820-127">正常</span><span class="sxs-lookup"><span data-stu-id="f7820-127">unhealthy</span></span>|<span data-ttu-id="f7820-128">5 </span><span class="sxs-lookup"><span data-stu-id="f7820-128">5</span></span>|<span data-ttu-id="f7820-129">设备运行不正常。</span><span class="sxs-lookup"><span data-stu-id="f7820-129">The device is unhealthy.</span></span>|
|<span data-ttu-id="f7820-130">deletePending</span><span class="sxs-lookup"><span data-stu-id="f7820-130">deletePending</span></span>|<span data-ttu-id="f7820-131">6 </span><span class="sxs-lookup"><span data-stu-id="f7820-131">6</span></span>|<span data-ttu-id="f7820-132">在设备上发生删除命令</span><span class="sxs-lookup"><span data-stu-id="f7820-132">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="f7820-133">retireIssued</span><span class="sxs-lookup"><span data-stu-id="f7820-133">retireIssued</span></span>|<span data-ttu-id="f7820-134">7 </span><span class="sxs-lookup"><span data-stu-id="f7820-134">7</span></span>|<span data-ttu-id="f7820-135">为设备发出了停用命令</span><span class="sxs-lookup"><span data-stu-id="f7820-135">A retire command was issued for the device</span></span>|
|<span data-ttu-id="f7820-136">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="f7820-136">wipeIssued</span></span>|<span data-ttu-id="f7820-137">8 </span><span class="sxs-lookup"><span data-stu-id="f7820-137">8</span></span>|<span data-ttu-id="f7820-138">已为设备发出擦除命令</span><span class="sxs-lookup"><span data-stu-id="f7820-138">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="f7820-139">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="f7820-139">wipeCanceled</span></span>|<span data-ttu-id="f7820-140">9 </span><span class="sxs-lookup"><span data-stu-id="f7820-140">9</span></span>|<span data-ttu-id="f7820-141">已取消此设备的擦除命令</span><span class="sxs-lookup"><span data-stu-id="f7820-141">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="f7820-142">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="f7820-142">retireCanceled</span></span>|<span data-ttu-id="f7820-143">10 </span><span class="sxs-lookup"><span data-stu-id="f7820-143">10</span></span>|<span data-ttu-id="f7820-144">已取消此设备的停用命令</span><span class="sxs-lookup"><span data-stu-id="f7820-144">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="f7820-145">探索</span><span class="sxs-lookup"><span data-stu-id="f7820-145">discovered</span></span>|<span data-ttu-id="f7820-146">11 </span><span class="sxs-lookup"><span data-stu-id="f7820-146">11</span></span>|<span data-ttu-id="f7820-147">设备已被发现，但未完全注册。</span><span class="sxs-lookup"><span data-stu-id="f7820-147">The device is discovered but not fully enrolled.</span></span>|



