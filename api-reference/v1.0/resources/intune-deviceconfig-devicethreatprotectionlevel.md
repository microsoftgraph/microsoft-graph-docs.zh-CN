---
title: deviceThreatProtectionLevel 枚举类型
description: 设备威胁防护 API 的设备威胁防护级别。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 21147e2be838bef34bc61eb401f57e1c650028d5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755089"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="72f09-103">deviceThreatProtectionLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="72f09-103">deviceThreatProtectionLevel enum type</span></span>

<span data-ttu-id="72f09-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72f09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72f09-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="72f09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72f09-106">设备威胁防护 API 的设备威胁防护级别。</span><span class="sxs-lookup"><span data-stu-id="72f09-106">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="72f09-107">成员</span><span class="sxs-lookup"><span data-stu-id="72f09-107">Members</span></span>
|<span data-ttu-id="72f09-108">成员</span><span class="sxs-lookup"><span data-stu-id="72f09-108">Member</span></span>|<span data-ttu-id="72f09-109">值</span><span class="sxs-lookup"><span data-stu-id="72f09-109">Value</span></span>|<span data-ttu-id="72f09-110">说明</span><span class="sxs-lookup"><span data-stu-id="72f09-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72f09-111">不可用</span><span class="sxs-lookup"><span data-stu-id="72f09-111">unavailable</span></span>|<span data-ttu-id="72f09-112">0</span><span class="sxs-lookup"><span data-stu-id="72f09-112">0</span></span>|<span data-ttu-id="72f09-113">默认值。</span><span class="sxs-lookup"><span data-stu-id="72f09-113">Default Value.</span></span> <span data-ttu-id="72f09-114">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="72f09-114">Do not use.</span></span>|
|<span data-ttu-id="72f09-115">secured</span><span class="sxs-lookup"><span data-stu-id="72f09-115">secured</span></span>|<span data-ttu-id="72f09-116">1</span><span class="sxs-lookup"><span data-stu-id="72f09-116">1</span></span>|<span data-ttu-id="72f09-117">设备威胁级别要求：安全。</span><span class="sxs-lookup"><span data-stu-id="72f09-117">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="72f09-118">这是最安全级别，表示未在设备上发现任何威胁。</span><span class="sxs-lookup"><span data-stu-id="72f09-118">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="72f09-119">low</span><span class="sxs-lookup"><span data-stu-id="72f09-119">low</span></span>|<span data-ttu-id="72f09-120">2</span><span class="sxs-lookup"><span data-stu-id="72f09-120">2</span></span>|<span data-ttu-id="72f09-121">设备威胁防护级别要求：低。</span><span class="sxs-lookup"><span data-stu-id="72f09-121">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="72f09-122">低表示威胁的严重性，对设备或设备数据带来的风险最小。</span><span class="sxs-lookup"><span data-stu-id="72f09-122">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="72f09-123">中等</span><span class="sxs-lookup"><span data-stu-id="72f09-123">medium</span></span>|<span data-ttu-id="72f09-124">3</span><span class="sxs-lookup"><span data-stu-id="72f09-124">3</span></span>|<span data-ttu-id="72f09-125">设备威胁防护级别要求：中等。</span><span class="sxs-lookup"><span data-stu-id="72f09-125">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="72f09-126">中等表示威胁的严重性，对设备或设备数据带来中等风险。</span><span class="sxs-lookup"><span data-stu-id="72f09-126">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="72f09-127">high</span><span class="sxs-lookup"><span data-stu-id="72f09-127">high</span></span>|<span data-ttu-id="72f09-128">4 </span><span class="sxs-lookup"><span data-stu-id="72f09-128">4</span></span>|<span data-ttu-id="72f09-129">设备威胁防护级别要求：高。</span><span class="sxs-lookup"><span data-stu-id="72f09-129">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="72f09-130">高表示威胁的严重性，对设备或设备数据带来高风险。</span><span class="sxs-lookup"><span data-stu-id="72f09-130">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="72f09-131">notSet</span><span class="sxs-lookup"><span data-stu-id="72f09-131">notSet</span></span>|<span data-ttu-id="72f09-132">10  </span><span class="sxs-lookup"><span data-stu-id="72f09-132">10</span></span>|<span data-ttu-id="72f09-133">设备威胁防护级别要求：未设置。</span><span class="sxs-lookup"><span data-stu-id="72f09-133">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="72f09-134">未设置表示设备无需满足威胁防护级别。</span><span class="sxs-lookup"><span data-stu-id="72f09-134">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|




