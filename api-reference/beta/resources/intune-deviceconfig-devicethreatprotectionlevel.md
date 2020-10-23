---
title: deviceThreatProtectionLevel 枚举类型
description: 设备威胁防护 API 的设备威胁保护级别。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 799448f79975cfa2a4879528770f85c3e862c365
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707799"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="bb573-103">deviceThreatProtectionLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="bb573-103">deviceThreatProtectionLevel enum type</span></span>

<span data-ttu-id="bb573-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb573-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb573-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb573-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb573-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb573-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb573-107">设备威胁防护 API 的设备威胁保护级别。</span><span class="sxs-lookup"><span data-stu-id="bb573-107">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="bb573-108">成员</span><span class="sxs-lookup"><span data-stu-id="bb573-108">Members</span></span>
|<span data-ttu-id="bb573-109">成员</span><span class="sxs-lookup"><span data-stu-id="bb573-109">Member</span></span>|<span data-ttu-id="bb573-110">值</span><span class="sxs-lookup"><span data-stu-id="bb573-110">Value</span></span>|<span data-ttu-id="bb573-111">说明</span><span class="sxs-lookup"><span data-stu-id="bb573-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb573-112">才</span><span class="sxs-lookup"><span data-stu-id="bb573-112">unavailable</span></span>|<span data-ttu-id="bb573-113">0</span><span class="sxs-lookup"><span data-stu-id="bb573-113">0</span></span>|<span data-ttu-id="bb573-114">默认值。</span><span class="sxs-lookup"><span data-stu-id="bb573-114">Default Value.</span></span> <span data-ttu-id="bb573-115">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="bb573-115">Do not use.</span></span>|
|<span data-ttu-id="bb573-116">加密</span><span class="sxs-lookup"><span data-stu-id="bb573-116">secured</span></span>|<span data-ttu-id="bb573-117">1</span><span class="sxs-lookup"><span data-stu-id="bb573-117">1</span></span>|<span data-ttu-id="bb573-118">设备威胁级别要求：安全。</span><span class="sxs-lookup"><span data-stu-id="bb573-118">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="bb573-119">这是最安全的级别，表示在设备上未发现任何威胁。</span><span class="sxs-lookup"><span data-stu-id="bb573-119">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="bb573-120">降低</span><span class="sxs-lookup"><span data-stu-id="bb573-120">low</span></span>|<span data-ttu-id="bb573-121">双面</span><span class="sxs-lookup"><span data-stu-id="bb573-121">2</span></span>|<span data-ttu-id="bb573-122">设备威胁保护级别要求：低。</span><span class="sxs-lookup"><span data-stu-id="bb573-122">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="bb573-123">Low 表示对设备或设备数据带来最小风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="bb573-123">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="bb573-124">中等</span><span class="sxs-lookup"><span data-stu-id="bb573-124">medium</span></span>|<span data-ttu-id="bb573-125">第三章</span><span class="sxs-lookup"><span data-stu-id="bb573-125">3</span></span>|<span data-ttu-id="bb573-126">设备威胁保护级别要求：中。</span><span class="sxs-lookup"><span data-stu-id="bb573-126">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="bb573-127">中型代表设备或设备数据面临中等风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="bb573-127">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="bb573-128">高效</span><span class="sxs-lookup"><span data-stu-id="bb573-128">high</span></span>|<span data-ttu-id="bb573-129">4 </span><span class="sxs-lookup"><span data-stu-id="bb573-129">4</span></span>|<span data-ttu-id="bb573-130">设备威胁保护级别要求：高。</span><span class="sxs-lookup"><span data-stu-id="bb573-130">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="bb573-131">High 表示对设备或设备数据带来严重风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="bb573-131">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="bb573-132">notSet</span><span class="sxs-lookup"><span data-stu-id="bb573-132">notSet</span></span>|<span data-ttu-id="bb573-133">10  </span><span class="sxs-lookup"><span data-stu-id="bb573-133">10</span></span>|<span data-ttu-id="bb573-134">设备威胁保护级别要求：未设置。</span><span class="sxs-lookup"><span data-stu-id="bb573-134">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="bb573-135">未设置表示设备不需要满足威胁保护级别。</span><span class="sxs-lookup"><span data-stu-id="bb573-135">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|





