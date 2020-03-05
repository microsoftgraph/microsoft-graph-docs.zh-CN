---
title: deviceThreatProtectionLevel 枚举类型
description: 设备威胁防护 API 的设备威胁保护级别。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a06e0ba5c34198d181a8ba854cf20a16b1e2aeab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530112"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="2240f-103">deviceThreatProtectionLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2240f-103">deviceThreatProtectionLevel enum type</span></span>

<span data-ttu-id="2240f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2240f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2240f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2240f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2240f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2240f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2240f-107">设备威胁防护 API 的设备威胁保护级别。</span><span class="sxs-lookup"><span data-stu-id="2240f-107">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="2240f-108">成员</span><span class="sxs-lookup"><span data-stu-id="2240f-108">Members</span></span>
|<span data-ttu-id="2240f-109">成员</span><span class="sxs-lookup"><span data-stu-id="2240f-109">Member</span></span>|<span data-ttu-id="2240f-110">值</span><span class="sxs-lookup"><span data-stu-id="2240f-110">Value</span></span>|<span data-ttu-id="2240f-111">说明</span><span class="sxs-lookup"><span data-stu-id="2240f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2240f-112">才</span><span class="sxs-lookup"><span data-stu-id="2240f-112">unavailable</span></span>|<span data-ttu-id="2240f-113">0</span><span class="sxs-lookup"><span data-stu-id="2240f-113">0</span></span>|<span data-ttu-id="2240f-114">默认值。</span><span class="sxs-lookup"><span data-stu-id="2240f-114">Default Value.</span></span> <span data-ttu-id="2240f-115">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="2240f-115">Do not use.</span></span>|
|<span data-ttu-id="2240f-116">加密</span><span class="sxs-lookup"><span data-stu-id="2240f-116">secured</span></span>|<span data-ttu-id="2240f-117">1 </span><span class="sxs-lookup"><span data-stu-id="2240f-117">1</span></span>|<span data-ttu-id="2240f-118">设备威胁级别要求：安全。</span><span class="sxs-lookup"><span data-stu-id="2240f-118">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="2240f-119">这是最安全的级别，表示在设备上未发现任何威胁。</span><span class="sxs-lookup"><span data-stu-id="2240f-119">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="2240f-120">降低</span><span class="sxs-lookup"><span data-stu-id="2240f-120">low</span></span>|<span data-ttu-id="2240f-121">2 </span><span class="sxs-lookup"><span data-stu-id="2240f-121">2</span></span>|<span data-ttu-id="2240f-122">设备威胁保护级别要求：低。</span><span class="sxs-lookup"><span data-stu-id="2240f-122">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="2240f-123">Low 表示对设备或设备数据带来最小风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="2240f-123">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="2240f-124">中等</span><span class="sxs-lookup"><span data-stu-id="2240f-124">medium</span></span>|<span data-ttu-id="2240f-125">3 </span><span class="sxs-lookup"><span data-stu-id="2240f-125">3</span></span>|<span data-ttu-id="2240f-126">设备威胁保护级别要求：中。</span><span class="sxs-lookup"><span data-stu-id="2240f-126">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="2240f-127">中型代表设备或设备数据面临中等风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="2240f-127">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="2240f-128">高效</span><span class="sxs-lookup"><span data-stu-id="2240f-128">high</span></span>|<span data-ttu-id="2240f-129">4 </span><span class="sxs-lookup"><span data-stu-id="2240f-129">4</span></span>|<span data-ttu-id="2240f-130">设备威胁保护级别要求：高。</span><span class="sxs-lookup"><span data-stu-id="2240f-130">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="2240f-131">High 表示对设备或设备数据带来严重风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="2240f-131">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="2240f-132">notSet</span><span class="sxs-lookup"><span data-stu-id="2240f-132">notSet</span></span>|<span data-ttu-id="2240f-133">10 </span><span class="sxs-lookup"><span data-stu-id="2240f-133">10</span></span>|<span data-ttu-id="2240f-134">设备威胁保护级别要求：未设置。</span><span class="sxs-lookup"><span data-stu-id="2240f-134">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="2240f-135">未设置表示设备不需要满足威胁保护级别。</span><span class="sxs-lookup"><span data-stu-id="2240f-135">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|



