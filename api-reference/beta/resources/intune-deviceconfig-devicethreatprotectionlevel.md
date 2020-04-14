---
title: deviceThreatProtectionLevel 枚举类型
description: 设备威胁防护 API 的设备威胁保护级别。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b78118e624898c90e3bd2e0e4c281bf0a0a4ca41
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469222"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="e1869-103">deviceThreatProtectionLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e1869-103">deviceThreatProtectionLevel enum type</span></span>

<span data-ttu-id="e1869-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1869-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1869-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e1869-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1869-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e1869-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1869-107">设备威胁防护 API 的设备威胁保护级别。</span><span class="sxs-lookup"><span data-stu-id="e1869-107">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="e1869-108">成员</span><span class="sxs-lookup"><span data-stu-id="e1869-108">Members</span></span>
|<span data-ttu-id="e1869-109">成员</span><span class="sxs-lookup"><span data-stu-id="e1869-109">Member</span></span>|<span data-ttu-id="e1869-110">值</span><span class="sxs-lookup"><span data-stu-id="e1869-110">Value</span></span>|<span data-ttu-id="e1869-111">说明</span><span class="sxs-lookup"><span data-stu-id="e1869-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1869-112">才</span><span class="sxs-lookup"><span data-stu-id="e1869-112">unavailable</span></span>|<span data-ttu-id="e1869-113">0</span><span class="sxs-lookup"><span data-stu-id="e1869-113">0</span></span>|<span data-ttu-id="e1869-114">默认值。</span><span class="sxs-lookup"><span data-stu-id="e1869-114">Default Value.</span></span> <span data-ttu-id="e1869-115">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="e1869-115">Do not use.</span></span>|
|<span data-ttu-id="e1869-116">加密</span><span class="sxs-lookup"><span data-stu-id="e1869-116">secured</span></span>|<span data-ttu-id="e1869-117">1</span><span class="sxs-lookup"><span data-stu-id="e1869-117">1</span></span>|<span data-ttu-id="e1869-118">设备威胁级别要求：安全。</span><span class="sxs-lookup"><span data-stu-id="e1869-118">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="e1869-119">这是最安全的级别，表示在设备上未发现任何威胁。</span><span class="sxs-lookup"><span data-stu-id="e1869-119">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="e1869-120">降低</span><span class="sxs-lookup"><span data-stu-id="e1869-120">low</span></span>|<span data-ttu-id="e1869-121">双面</span><span class="sxs-lookup"><span data-stu-id="e1869-121">2</span></span>|<span data-ttu-id="e1869-122">设备威胁保护级别要求：低。</span><span class="sxs-lookup"><span data-stu-id="e1869-122">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="e1869-123">Low 表示对设备或设备数据带来最小风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="e1869-123">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="e1869-124">中等</span><span class="sxs-lookup"><span data-stu-id="e1869-124">medium</span></span>|<span data-ttu-id="e1869-125">第三章</span><span class="sxs-lookup"><span data-stu-id="e1869-125">3</span></span>|<span data-ttu-id="e1869-126">设备威胁保护级别要求：中。</span><span class="sxs-lookup"><span data-stu-id="e1869-126">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="e1869-127">中型代表设备或设备数据面临中等风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="e1869-127">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="e1869-128">高效</span><span class="sxs-lookup"><span data-stu-id="e1869-128">high</span></span>|<span data-ttu-id="e1869-129">4 </span><span class="sxs-lookup"><span data-stu-id="e1869-129">4</span></span>|<span data-ttu-id="e1869-130">设备威胁保护级别要求：高。</span><span class="sxs-lookup"><span data-stu-id="e1869-130">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="e1869-131">High 表示对设备或设备数据带来严重风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="e1869-131">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="e1869-132">notSet</span><span class="sxs-lookup"><span data-stu-id="e1869-132">notSet</span></span>|<span data-ttu-id="e1869-133">10 </span><span class="sxs-lookup"><span data-stu-id="e1869-133">10</span></span>|<span data-ttu-id="e1869-134">设备威胁保护级别要求：未设置。</span><span class="sxs-lookup"><span data-stu-id="e1869-134">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="e1869-135">未设置表示设备不需要满足威胁保护级别。</span><span class="sxs-lookup"><span data-stu-id="e1869-135">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|



