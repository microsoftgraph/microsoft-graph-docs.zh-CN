---
title: managementState 枚举类型
description: Microsoft Intune 中设备的管理状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05dc0db1ecbe88616ca36db82bad2081b4133e3f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521290"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="6fe7b-103">managementState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6fe7b-103">managementState enum type</span></span>

> <span data-ttu-id="6fe7b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6fe7b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fe7b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6fe7b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fe7b-106">Microsoft Intune 中设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="6fe7b-106">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="6fe7b-107">成员</span><span class="sxs-lookup"><span data-stu-id="6fe7b-107">Members</span></span>
|<span data-ttu-id="6fe7b-108">成员</span><span class="sxs-lookup"><span data-stu-id="6fe7b-108">Member</span></span>|<span data-ttu-id="6fe7b-109">值</span><span class="sxs-lookup"><span data-stu-id="6fe7b-109">Value</span></span>|<span data-ttu-id="6fe7b-110">说明</span><span class="sxs-lookup"><span data-stu-id="6fe7b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fe7b-111">managed</span><span class="sxs-lookup"><span data-stu-id="6fe7b-111">managed</span></span>|<span data-ttu-id="6fe7b-112">0</span><span class="sxs-lookup"><span data-stu-id="6fe7b-112">0</span></span>|<span data-ttu-id="6fe7b-113">设备正在管理中</span><span class="sxs-lookup"><span data-stu-id="6fe7b-113">The device is under management</span></span>|
|<span data-ttu-id="6fe7b-114">retirePending</span><span class="sxs-lookup"><span data-stu-id="6fe7b-114">retirePending</span></span>|<span data-ttu-id="6fe7b-115">1</span><span class="sxs-lookup"><span data-stu-id="6fe7b-115">1</span></span>|<span data-ttu-id="6fe7b-116">设备和 unenrolling 从管理中的过程中发生停用命令</span><span class="sxs-lookup"><span data-stu-id="6fe7b-116">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="6fe7b-117">retireFailed</span><span class="sxs-lookup"><span data-stu-id="6fe7b-117">retireFailed</span></span>|<span data-ttu-id="6fe7b-118">2 </span><span class="sxs-lookup"><span data-stu-id="6fe7b-118">2</span></span>|<span data-ttu-id="6fe7b-119">设备上的停用命令失败</span><span class="sxs-lookup"><span data-stu-id="6fe7b-119">Retire command failed on the device</span></span>|
|<span data-ttu-id="6fe7b-120">wipePending</span><span class="sxs-lookup"><span data-stu-id="6fe7b-120">wipePending</span></span>|<span data-ttu-id="6fe7b-121">3 </span><span class="sxs-lookup"><span data-stu-id="6fe7b-121">3</span></span>|<span data-ttu-id="6fe7b-122">设备和 unenrolling 中的 "擦除" 命令在管理过程中发生</span><span class="sxs-lookup"><span data-stu-id="6fe7b-122">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="6fe7b-123">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="6fe7b-123">wipeFailed</span></span>|<span data-ttu-id="6fe7b-124">4 </span><span class="sxs-lookup"><span data-stu-id="6fe7b-124">4</span></span>|<span data-ttu-id="6fe7b-125">设备上的擦除命令失败</span><span class="sxs-lookup"><span data-stu-id="6fe7b-125">Wipe command failed on the device</span></span>|
|<span data-ttu-id="6fe7b-126">正常</span><span class="sxs-lookup"><span data-stu-id="6fe7b-126">unhealthy</span></span>|<span data-ttu-id="6fe7b-127">5 </span><span class="sxs-lookup"><span data-stu-id="6fe7b-127">5</span></span>|<span data-ttu-id="6fe7b-128">设备运行不正常。</span><span class="sxs-lookup"><span data-stu-id="6fe7b-128">The device is unhealthy.</span></span>|
|<span data-ttu-id="6fe7b-129">deletePending</span><span class="sxs-lookup"><span data-stu-id="6fe7b-129">deletePending</span></span>|<span data-ttu-id="6fe7b-130">6 </span><span class="sxs-lookup"><span data-stu-id="6fe7b-130">6</span></span>|<span data-ttu-id="6fe7b-131">在设备上发生删除命令</span><span class="sxs-lookup"><span data-stu-id="6fe7b-131">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="6fe7b-132">retireIssued</span><span class="sxs-lookup"><span data-stu-id="6fe7b-132">retireIssued</span></span>|<span data-ttu-id="6fe7b-133">7 </span><span class="sxs-lookup"><span data-stu-id="6fe7b-133">7</span></span>|<span data-ttu-id="6fe7b-134">为设备发出了停用命令</span><span class="sxs-lookup"><span data-stu-id="6fe7b-134">A retire command was issued for the device</span></span>|
|<span data-ttu-id="6fe7b-135">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="6fe7b-135">wipeIssued</span></span>|<span data-ttu-id="6fe7b-136">8 </span><span class="sxs-lookup"><span data-stu-id="6fe7b-136">8</span></span>|<span data-ttu-id="6fe7b-137">已为设备发出擦除命令</span><span class="sxs-lookup"><span data-stu-id="6fe7b-137">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="6fe7b-138">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="6fe7b-138">wipeCanceled</span></span>|<span data-ttu-id="6fe7b-139">9 </span><span class="sxs-lookup"><span data-stu-id="6fe7b-139">9</span></span>|<span data-ttu-id="6fe7b-140">已取消此设备的擦除命令</span><span class="sxs-lookup"><span data-stu-id="6fe7b-140">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="6fe7b-141">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="6fe7b-141">retireCanceled</span></span>|<span data-ttu-id="6fe7b-142">10 </span><span class="sxs-lookup"><span data-stu-id="6fe7b-142">10</span></span>|<span data-ttu-id="6fe7b-143">已取消此设备的停用命令</span><span class="sxs-lookup"><span data-stu-id="6fe7b-143">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="6fe7b-144">探索</span><span class="sxs-lookup"><span data-stu-id="6fe7b-144">discovered</span></span>|<span data-ttu-id="6fe7b-145">11 </span><span class="sxs-lookup"><span data-stu-id="6fe7b-145">11</span></span>|<span data-ttu-id="6fe7b-146">设备已被发现, 但未完全注册。</span><span class="sxs-lookup"><span data-stu-id="6fe7b-146">The device is discovered but not fully enrolled.</span></span>|





