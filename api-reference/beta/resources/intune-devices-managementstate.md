---
title: managementState 枚举类型
description: Microsoft Intune 中设备的管理状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0ce5fc93bfd48d4beaccac1552573c228f1e6f09
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725440"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="b8095-103">managementState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b8095-103">managementState enum type</span></span>

<span data-ttu-id="b8095-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8095-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8095-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b8095-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8095-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b8095-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8095-107">Microsoft Intune 中设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="b8095-107">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="b8095-108">成员</span><span class="sxs-lookup"><span data-stu-id="b8095-108">Members</span></span>
|<span data-ttu-id="b8095-109">成员</span><span class="sxs-lookup"><span data-stu-id="b8095-109">Member</span></span>|<span data-ttu-id="b8095-110">值</span><span class="sxs-lookup"><span data-stu-id="b8095-110">Value</span></span>|<span data-ttu-id="b8095-111">说明</span><span class="sxs-lookup"><span data-stu-id="b8095-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8095-112">managed</span><span class="sxs-lookup"><span data-stu-id="b8095-112">managed</span></span>|<span data-ttu-id="b8095-113">0</span><span class="sxs-lookup"><span data-stu-id="b8095-113">0</span></span>|<span data-ttu-id="b8095-114">设备正在管理中</span><span class="sxs-lookup"><span data-stu-id="b8095-114">The device is under management</span></span>|
|<span data-ttu-id="b8095-115">retirePending</span><span class="sxs-lookup"><span data-stu-id="b8095-115">retirePending</span></span>|<span data-ttu-id="b8095-116">1</span><span class="sxs-lookup"><span data-stu-id="b8095-116">1</span></span>|<span data-ttu-id="b8095-117">设备和 unenrolling 从管理中的过程中发生停用命令</span><span class="sxs-lookup"><span data-stu-id="b8095-117">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="b8095-118">retireFailed</span><span class="sxs-lookup"><span data-stu-id="b8095-118">retireFailed</span></span>|<span data-ttu-id="b8095-119">双面</span><span class="sxs-lookup"><span data-stu-id="b8095-119">2</span></span>|<span data-ttu-id="b8095-120">设备上的停用命令失败</span><span class="sxs-lookup"><span data-stu-id="b8095-120">Retire command failed on the device</span></span>|
|<span data-ttu-id="b8095-121">wipePending</span><span class="sxs-lookup"><span data-stu-id="b8095-121">wipePending</span></span>|<span data-ttu-id="b8095-122">第三章</span><span class="sxs-lookup"><span data-stu-id="b8095-122">3</span></span>|<span data-ttu-id="b8095-123">设备和 unenrolling 中的 "擦除" 命令在管理过程中发生</span><span class="sxs-lookup"><span data-stu-id="b8095-123">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="b8095-124">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="b8095-124">wipeFailed</span></span>|<span data-ttu-id="b8095-125">4 </span><span class="sxs-lookup"><span data-stu-id="b8095-125">4</span></span>|<span data-ttu-id="b8095-126">设备上的擦除命令失败</span><span class="sxs-lookup"><span data-stu-id="b8095-126">Wipe command failed on the device</span></span>|
|<span data-ttu-id="b8095-127">正常</span><span class="sxs-lookup"><span data-stu-id="b8095-127">unhealthy</span></span>|<span data-ttu-id="b8095-128">5 </span><span class="sxs-lookup"><span data-stu-id="b8095-128">5</span></span>|<span data-ttu-id="b8095-129">设备运行不正常。</span><span class="sxs-lookup"><span data-stu-id="b8095-129">The device is unhealthy.</span></span>|
|<span data-ttu-id="b8095-130">deletePending</span><span class="sxs-lookup"><span data-stu-id="b8095-130">deletePending</span></span>|<span data-ttu-id="b8095-131">6 </span><span class="sxs-lookup"><span data-stu-id="b8095-131">6</span></span>|<span data-ttu-id="b8095-132">在设备上发生删除命令</span><span class="sxs-lookup"><span data-stu-id="b8095-132">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="b8095-133">retireIssued</span><span class="sxs-lookup"><span data-stu-id="b8095-133">retireIssued</span></span>|<span data-ttu-id="b8095-134">7 </span><span class="sxs-lookup"><span data-stu-id="b8095-134">7</span></span>|<span data-ttu-id="b8095-135">为设备发出了停用命令</span><span class="sxs-lookup"><span data-stu-id="b8095-135">A retire command was issued for the device</span></span>|
|<span data-ttu-id="b8095-136">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="b8095-136">wipeIssued</span></span>|<span data-ttu-id="b8095-137">8 </span><span class="sxs-lookup"><span data-stu-id="b8095-137">8</span></span>|<span data-ttu-id="b8095-138">已为设备发出擦除命令</span><span class="sxs-lookup"><span data-stu-id="b8095-138">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="b8095-139">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="b8095-139">wipeCanceled</span></span>|<span data-ttu-id="b8095-140">9 </span><span class="sxs-lookup"><span data-stu-id="b8095-140">9</span></span>|<span data-ttu-id="b8095-141">已取消此设备的擦除命令</span><span class="sxs-lookup"><span data-stu-id="b8095-141">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="b8095-142">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="b8095-142">retireCanceled</span></span>|<span data-ttu-id="b8095-143">10  </span><span class="sxs-lookup"><span data-stu-id="b8095-143">10</span></span>|<span data-ttu-id="b8095-144">已取消此设备的停用命令</span><span class="sxs-lookup"><span data-stu-id="b8095-144">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="b8095-145">探索</span><span class="sxs-lookup"><span data-stu-id="b8095-145">discovered</span></span>|<span data-ttu-id="b8095-146">11x17</span><span class="sxs-lookup"><span data-stu-id="b8095-146">11</span></span>|<span data-ttu-id="b8095-147">设备已被发现，但未完全注册。</span><span class="sxs-lookup"><span data-stu-id="b8095-147">The device is discovered but not fully enrolled.</span></span>|





