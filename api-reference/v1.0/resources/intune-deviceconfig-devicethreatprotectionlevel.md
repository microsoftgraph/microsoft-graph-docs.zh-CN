---
title: deviceThreatProtectionLevel 枚举类型
description: 设备威胁防护 API 的设备威胁保护级别。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e64bc6465e190e4e5da3629b6d638dc82813a2bb
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359381"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="ad96d-103">deviceThreatProtectionLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ad96d-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="ad96d-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ad96d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad96d-105">设备威胁防护 API 的设备威胁保护级别。</span><span class="sxs-lookup"><span data-stu-id="ad96d-105">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="ad96d-106">成员</span><span class="sxs-lookup"><span data-stu-id="ad96d-106">Members</span></span>
|<span data-ttu-id="ad96d-107">成员</span><span class="sxs-lookup"><span data-stu-id="ad96d-107">Member</span></span>|<span data-ttu-id="ad96d-108">值</span><span class="sxs-lookup"><span data-stu-id="ad96d-108">Value</span></span>|<span data-ttu-id="ad96d-109">说明</span><span class="sxs-lookup"><span data-stu-id="ad96d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad96d-110">才</span><span class="sxs-lookup"><span data-stu-id="ad96d-110">unavailable</span></span>|<span data-ttu-id="ad96d-111">0</span><span class="sxs-lookup"><span data-stu-id="ad96d-111">0</span></span>|<span data-ttu-id="ad96d-112">默认值。</span><span class="sxs-lookup"><span data-stu-id="ad96d-112">Default Value.</span></span> <span data-ttu-id="ad96d-113">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="ad96d-113">Do not use.</span></span>|
|<span data-ttu-id="ad96d-114">加密</span><span class="sxs-lookup"><span data-stu-id="ad96d-114">secured</span></span>|<span data-ttu-id="ad96d-115">1</span><span class="sxs-lookup"><span data-stu-id="ad96d-115">1</span></span>|<span data-ttu-id="ad96d-116">设备威胁级别要求：安全。</span><span class="sxs-lookup"><span data-stu-id="ad96d-116">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="ad96d-117">这是最安全的级别，表示在设备上未发现任何威胁。</span><span class="sxs-lookup"><span data-stu-id="ad96d-117">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="ad96d-118">降低</span><span class="sxs-lookup"><span data-stu-id="ad96d-118">low</span></span>|<span data-ttu-id="ad96d-119">双面</span><span class="sxs-lookup"><span data-stu-id="ad96d-119">2</span></span>|<span data-ttu-id="ad96d-120">设备威胁保护级别要求：低。</span><span class="sxs-lookup"><span data-stu-id="ad96d-120">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="ad96d-121">Low 表示对设备或设备数据带来最小风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="ad96d-121">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="ad96d-122">中等</span><span class="sxs-lookup"><span data-stu-id="ad96d-122">medium</span></span>|<span data-ttu-id="ad96d-123">第三章</span><span class="sxs-lookup"><span data-stu-id="ad96d-123">3</span></span>|<span data-ttu-id="ad96d-124">设备威胁保护级别要求：中。</span><span class="sxs-lookup"><span data-stu-id="ad96d-124">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="ad96d-125">中型代表设备或设备数据面临中等风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="ad96d-125">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="ad96d-126">高效</span><span class="sxs-lookup"><span data-stu-id="ad96d-126">high</span></span>|<span data-ttu-id="ad96d-127">4</span><span class="sxs-lookup"><span data-stu-id="ad96d-127">4</span></span>|<span data-ttu-id="ad96d-128">设备威胁保护级别要求：高。</span><span class="sxs-lookup"><span data-stu-id="ad96d-128">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="ad96d-129">High 表示对设备或设备数据带来严重风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="ad96d-129">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="ad96d-130">notSet</span><span class="sxs-lookup"><span data-stu-id="ad96d-130">notSet</span></span>|<span data-ttu-id="ad96d-131">10 </span><span class="sxs-lookup"><span data-stu-id="ad96d-131">10</span></span>|<span data-ttu-id="ad96d-132">设备威胁保护级别要求：未设置。</span><span class="sxs-lookup"><span data-stu-id="ad96d-132">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="ad96d-133">未设置表示设备不需要满足威胁保护级别。</span><span class="sxs-lookup"><span data-stu-id="ad96d-133">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|




