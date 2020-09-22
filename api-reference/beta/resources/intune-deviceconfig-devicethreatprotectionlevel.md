---
title: deviceThreatProtectionLevel 枚举类型
description: 设备威胁防护 API 的设备威胁保护级别。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e6169a6f7816a04b0e3a81065fc78869eadc3b7e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040026"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="62dee-103">deviceThreatProtectionLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="62dee-103">deviceThreatProtectionLevel enum type</span></span>

<span data-ttu-id="62dee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62dee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62dee-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="62dee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62dee-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="62dee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62dee-107">设备威胁防护 API 的设备威胁保护级别。</span><span class="sxs-lookup"><span data-stu-id="62dee-107">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="62dee-108">成员</span><span class="sxs-lookup"><span data-stu-id="62dee-108">Members</span></span>
|<span data-ttu-id="62dee-109">成员</span><span class="sxs-lookup"><span data-stu-id="62dee-109">Member</span></span>|<span data-ttu-id="62dee-110">值</span><span class="sxs-lookup"><span data-stu-id="62dee-110">Value</span></span>|<span data-ttu-id="62dee-111">说明</span><span class="sxs-lookup"><span data-stu-id="62dee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62dee-112">才</span><span class="sxs-lookup"><span data-stu-id="62dee-112">unavailable</span></span>|<span data-ttu-id="62dee-113">0</span><span class="sxs-lookup"><span data-stu-id="62dee-113">0</span></span>|<span data-ttu-id="62dee-114">默认值。</span><span class="sxs-lookup"><span data-stu-id="62dee-114">Default Value.</span></span> <span data-ttu-id="62dee-115">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="62dee-115">Do not use.</span></span>|
|<span data-ttu-id="62dee-116">加密</span><span class="sxs-lookup"><span data-stu-id="62dee-116">secured</span></span>|<span data-ttu-id="62dee-117">1 </span><span class="sxs-lookup"><span data-stu-id="62dee-117">1</span></span>|<span data-ttu-id="62dee-118">设备威胁级别要求：安全。</span><span class="sxs-lookup"><span data-stu-id="62dee-118">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="62dee-119">这是最安全的级别，表示在设备上未发现任何威胁。</span><span class="sxs-lookup"><span data-stu-id="62dee-119">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="62dee-120">降低</span><span class="sxs-lookup"><span data-stu-id="62dee-120">low</span></span>|<span data-ttu-id="62dee-121">2 </span><span class="sxs-lookup"><span data-stu-id="62dee-121">2</span></span>|<span data-ttu-id="62dee-122">设备威胁保护级别要求：低。</span><span class="sxs-lookup"><span data-stu-id="62dee-122">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="62dee-123">Low 表示对设备或设备数据带来最小风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="62dee-123">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="62dee-124">中等</span><span class="sxs-lookup"><span data-stu-id="62dee-124">medium</span></span>|<span data-ttu-id="62dee-125">第三章</span><span class="sxs-lookup"><span data-stu-id="62dee-125">3</span></span>|<span data-ttu-id="62dee-126">设备威胁保护级别要求：中。</span><span class="sxs-lookup"><span data-stu-id="62dee-126">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="62dee-127">中型代表设备或设备数据面临中等风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="62dee-127">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="62dee-128">高效</span><span class="sxs-lookup"><span data-stu-id="62dee-128">high</span></span>|<span data-ttu-id="62dee-129">4 </span><span class="sxs-lookup"><span data-stu-id="62dee-129">4</span></span>|<span data-ttu-id="62dee-130">设备威胁保护级别要求：高。</span><span class="sxs-lookup"><span data-stu-id="62dee-130">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="62dee-131">High 表示对设备或设备数据带来严重风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="62dee-131">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="62dee-132">notSet</span><span class="sxs-lookup"><span data-stu-id="62dee-132">notSet</span></span>|<span data-ttu-id="62dee-133">10 </span><span class="sxs-lookup"><span data-stu-id="62dee-133">10</span></span>|<span data-ttu-id="62dee-134">设备威胁保护级别要求：未设置。</span><span class="sxs-lookup"><span data-stu-id="62dee-134">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="62dee-135">未设置表示设备不需要满足威胁保护级别。</span><span class="sxs-lookup"><span data-stu-id="62dee-135">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|






