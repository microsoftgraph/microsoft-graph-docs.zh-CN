---
title: 管理枚举类型
description: 管理 Microsoft Intune 中设备的状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a8d0801949125f3b0cceb865ac1f8546195112e3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420015"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="7901d-103">管理枚举类型</span><span class="sxs-lookup"><span data-stu-id="7901d-103">managementState enum type</span></span>

> <span data-ttu-id="7901d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="7901d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7901d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7901d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7901d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7901d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7901d-107">管理 Microsoft Intune 中设备的状态。</span><span class="sxs-lookup"><span data-stu-id="7901d-107">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="7901d-108">成员</span><span class="sxs-lookup"><span data-stu-id="7901d-108">Members</span></span>
|<span data-ttu-id="7901d-109">成员</span><span class="sxs-lookup"><span data-stu-id="7901d-109">Member</span></span>|<span data-ttu-id="7901d-110">值</span><span class="sxs-lookup"><span data-stu-id="7901d-110">Value</span></span>|<span data-ttu-id="7901d-111">说明</span><span class="sxs-lookup"><span data-stu-id="7901d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7901d-112">托管</span><span class="sxs-lookup"><span data-stu-id="7901d-112">managed</span></span>|<span data-ttu-id="7901d-113">0</span><span class="sxs-lookup"><span data-stu-id="7901d-113">0</span></span>|<span data-ttu-id="7901d-114">在管理下的设备位于</span><span class="sxs-lookup"><span data-stu-id="7901d-114">The device is under management</span></span>|
|<span data-ttu-id="7901d-115">retirePending</span><span class="sxs-lookup"><span data-stu-id="7901d-115">retirePending</span></span>|<span data-ttu-id="7901d-116">1</span><span class="sxs-lookup"><span data-stu-id="7901d-116">1</span></span>|<span data-ttu-id="7901d-117">废弃命令正在撤消设备上并且正在 unenrolling 从管理</span><span class="sxs-lookup"><span data-stu-id="7901d-117">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="7901d-118">retireFailed</span><span class="sxs-lookup"><span data-stu-id="7901d-118">retireFailed</span></span>|<span data-ttu-id="7901d-119">2</span><span class="sxs-lookup"><span data-stu-id="7901d-119">2</span></span>|<span data-ttu-id="7901d-120">停用命令在设备上失败</span><span class="sxs-lookup"><span data-stu-id="7901d-120">Retire command failed on the device</span></span>|
|<span data-ttu-id="7901d-121">wipePending</span><span class="sxs-lookup"><span data-stu-id="7901d-121">wipePending</span></span>|<span data-ttu-id="7901d-122">3</span><span class="sxs-lookup"><span data-stu-id="7901d-122">3</span></span>|<span data-ttu-id="7901d-123">擦除命令正在撤消设备上并且正在 unenrolling 从管理</span><span class="sxs-lookup"><span data-stu-id="7901d-123">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="7901d-124">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="7901d-124">wipeFailed</span></span>|<span data-ttu-id="7901d-125">4</span><span class="sxs-lookup"><span data-stu-id="7901d-125">4</span></span>|<span data-ttu-id="7901d-126">擦除设备上失败的命令</span><span class="sxs-lookup"><span data-stu-id="7901d-126">Wipe command failed on the device</span></span>|
|<span data-ttu-id="7901d-127">不正常</span><span class="sxs-lookup"><span data-stu-id="7901d-127">unhealthy</span></span>|<span data-ttu-id="7901d-128">5</span><span class="sxs-lookup"><span data-stu-id="7901d-128">5</span></span>|<span data-ttu-id="7901d-129">设备不正常。</span><span class="sxs-lookup"><span data-stu-id="7901d-129">The device is unhealthy.</span></span>|
|<span data-ttu-id="7901d-130">deletePending</span><span class="sxs-lookup"><span data-stu-id="7901d-130">deletePending</span></span>|<span data-ttu-id="7901d-131">6</span><span class="sxs-lookup"><span data-stu-id="7901d-131">6</span></span>|<span data-ttu-id="7901d-132">删除命令正在撤消对设备</span><span class="sxs-lookup"><span data-stu-id="7901d-132">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="7901d-133">retireIssued</span><span class="sxs-lookup"><span data-stu-id="7901d-133">retireIssued</span></span>|<span data-ttu-id="7901d-134">7</span><span class="sxs-lookup"><span data-stu-id="7901d-134">7</span></span>|<span data-ttu-id="7901d-135">为设备发出了废弃命令</span><span class="sxs-lookup"><span data-stu-id="7901d-135">A retire command was issued for the device</span></span>|
|<span data-ttu-id="7901d-136">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="7901d-136">wipeIssued</span></span>|<span data-ttu-id="7901d-137">8</span><span class="sxs-lookup"><span data-stu-id="7901d-137">8</span></span>|<span data-ttu-id="7901d-138">为设备发出了擦除命令</span><span class="sxs-lookup"><span data-stu-id="7901d-138">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="7901d-139">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="7901d-139">wipeCanceled</span></span>|<span data-ttu-id="7901d-140">9</span><span class="sxs-lookup"><span data-stu-id="7901d-140">9</span></span>|<span data-ttu-id="7901d-141">此设备擦除命令已被取消</span><span class="sxs-lookup"><span data-stu-id="7901d-141">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="7901d-142">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="7901d-142">retireCanceled</span></span>|<span data-ttu-id="7901d-143">10</span><span class="sxs-lookup"><span data-stu-id="7901d-143">10</span></span>|<span data-ttu-id="7901d-144">此设备废弃命令已被取消</span><span class="sxs-lookup"><span data-stu-id="7901d-144">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="7901d-145">发现</span><span class="sxs-lookup"><span data-stu-id="7901d-145">discovered</span></span>|<span data-ttu-id="7901d-146">11</span><span class="sxs-lookup"><span data-stu-id="7901d-146">11</span></span>|<span data-ttu-id="7901d-147">发现但不是完全注册的设备。</span><span class="sxs-lookup"><span data-stu-id="7901d-147">The device is discovered but not fully enrolled.</span></span>|




