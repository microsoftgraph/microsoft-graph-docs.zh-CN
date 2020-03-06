---
title: deviceThreatProtectionLevel 枚举类型
description: 设备威胁防护 API 的设备威胁保护级别。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 12bf8aad0e6aed54a4bb991052201997e2872da3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530755"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="65cb4-103">deviceThreatProtectionLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="65cb4-103">deviceThreatProtectionLevel enum type</span></span>

<span data-ttu-id="65cb4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65cb4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65cb4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65cb4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65cb4-106">设备威胁防护 API 的设备威胁保护级别。</span><span class="sxs-lookup"><span data-stu-id="65cb4-106">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="65cb4-107">成员</span><span class="sxs-lookup"><span data-stu-id="65cb4-107">Members</span></span>
|<span data-ttu-id="65cb4-108">成员</span><span class="sxs-lookup"><span data-stu-id="65cb4-108">Member</span></span>|<span data-ttu-id="65cb4-109">值</span><span class="sxs-lookup"><span data-stu-id="65cb4-109">Value</span></span>|<span data-ttu-id="65cb4-110">说明</span><span class="sxs-lookup"><span data-stu-id="65cb4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65cb4-111">才</span><span class="sxs-lookup"><span data-stu-id="65cb4-111">unavailable</span></span>|<span data-ttu-id="65cb4-112">0</span><span class="sxs-lookup"><span data-stu-id="65cb4-112">0</span></span>|<span data-ttu-id="65cb4-113">默认值。</span><span class="sxs-lookup"><span data-stu-id="65cb4-113">Default Value.</span></span> <span data-ttu-id="65cb4-114">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="65cb4-114">Do not use.</span></span>|
|<span data-ttu-id="65cb4-115">加密</span><span class="sxs-lookup"><span data-stu-id="65cb4-115">secured</span></span>|<span data-ttu-id="65cb4-116">1 </span><span class="sxs-lookup"><span data-stu-id="65cb4-116">1</span></span>|<span data-ttu-id="65cb4-117">设备威胁级别要求：安全。</span><span class="sxs-lookup"><span data-stu-id="65cb4-117">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="65cb4-118">这是最安全的级别，表示在设备上未发现任何威胁。</span><span class="sxs-lookup"><span data-stu-id="65cb4-118">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="65cb4-119">降低</span><span class="sxs-lookup"><span data-stu-id="65cb4-119">low</span></span>|<span data-ttu-id="65cb4-120">2 </span><span class="sxs-lookup"><span data-stu-id="65cb4-120">2</span></span>|<span data-ttu-id="65cb4-121">设备威胁保护级别要求：低。</span><span class="sxs-lookup"><span data-stu-id="65cb4-121">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="65cb4-122">Low 表示对设备或设备数据带来最小风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="65cb4-122">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="65cb4-123">中等</span><span class="sxs-lookup"><span data-stu-id="65cb4-123">medium</span></span>|<span data-ttu-id="65cb4-124">3 </span><span class="sxs-lookup"><span data-stu-id="65cb4-124">3</span></span>|<span data-ttu-id="65cb4-125">设备威胁保护级别要求：中。</span><span class="sxs-lookup"><span data-stu-id="65cb4-125">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="65cb4-126">中型代表设备或设备数据面临中等风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="65cb4-126">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="65cb4-127">高效</span><span class="sxs-lookup"><span data-stu-id="65cb4-127">high</span></span>|<span data-ttu-id="65cb4-128">4 </span><span class="sxs-lookup"><span data-stu-id="65cb4-128">4</span></span>|<span data-ttu-id="65cb4-129">设备威胁保护级别要求：高。</span><span class="sxs-lookup"><span data-stu-id="65cb4-129">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="65cb4-130">High 表示对设备或设备数据带来严重风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="65cb4-130">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="65cb4-131">notSet</span><span class="sxs-lookup"><span data-stu-id="65cb4-131">notSet</span></span>|<span data-ttu-id="65cb4-132">10 </span><span class="sxs-lookup"><span data-stu-id="65cb4-132">10</span></span>|<span data-ttu-id="65cb4-133">设备威胁保护级别要求：未设置。</span><span class="sxs-lookup"><span data-stu-id="65cb4-133">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="65cb4-134">未设置表示设备不需要满足威胁保护级别。</span><span class="sxs-lookup"><span data-stu-id="65cb4-134">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|




