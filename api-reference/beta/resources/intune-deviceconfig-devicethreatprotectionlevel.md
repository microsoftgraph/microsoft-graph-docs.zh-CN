---
title: deviceThreatProtectionLevel 枚举类型
description: 设备的设备威胁保护 API 的威胁保护级别。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a4c9bbc599d424b91d07339a7a7cdad90b84c262
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411230"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="ce911-103">deviceThreatProtectionLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ce911-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="ce911-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="ce911-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ce911-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ce911-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce911-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ce911-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce911-107">设备的设备威胁保护 API 的威胁保护级别。</span><span class="sxs-lookup"><span data-stu-id="ce911-107">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="ce911-108">成员</span><span class="sxs-lookup"><span data-stu-id="ce911-108">Members</span></span>
|<span data-ttu-id="ce911-109">成员</span><span class="sxs-lookup"><span data-stu-id="ce911-109">Member</span></span>|<span data-ttu-id="ce911-110">值</span><span class="sxs-lookup"><span data-stu-id="ce911-110">Value</span></span>|<span data-ttu-id="ce911-111">说明</span><span class="sxs-lookup"><span data-stu-id="ce911-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce911-112">不可用</span><span class="sxs-lookup"><span data-stu-id="ce911-112">unavailable</span></span>|<span data-ttu-id="ce911-113">0</span><span class="sxs-lookup"><span data-stu-id="ce911-113">0</span></span>|<span data-ttu-id="ce911-114">默认值。</span><span class="sxs-lookup"><span data-stu-id="ce911-114">Default Value.</span></span> <span data-ttu-id="ce911-115">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="ce911-115">Do not use.</span></span>|
|<span data-ttu-id="ce911-116">保护</span><span class="sxs-lookup"><span data-stu-id="ce911-116">secured</span></span>|<span data-ttu-id="ce911-117">1</span><span class="sxs-lookup"><span data-stu-id="ce911-117">1</span></span>|<span data-ttu-id="ce911-118">设备威胁级别要求： 安全。</span><span class="sxs-lookup"><span data-stu-id="ce911-118">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="ce911-119">这是最安全的级别，表示在设备上未发现任何威胁。</span><span class="sxs-lookup"><span data-stu-id="ce911-119">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="ce911-120">低</span><span class="sxs-lookup"><span data-stu-id="ce911-120">low</span></span>|<span data-ttu-id="ce911-121">2</span><span class="sxs-lookup"><span data-stu-id="ce911-121">2</span></span>|<span data-ttu-id="ce911-122">设备威胁保护级别要求： 低。</span><span class="sxs-lookup"><span data-stu-id="ce911-122">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="ce911-123">低代表严重性为会带来风险降至最低到设备或设备数据的威胁。</span><span class="sxs-lookup"><span data-stu-id="ce911-123">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="ce911-124">中等</span><span class="sxs-lookup"><span data-stu-id="ce911-124">medium</span></span>|<span data-ttu-id="ce911-125">3</span><span class="sxs-lookup"><span data-stu-id="ce911-125">3</span></span>|<span data-ttu-id="ce911-126">设备威胁保护级别要求： 中等。</span><span class="sxs-lookup"><span data-stu-id="ce911-126">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="ce911-127">中等代表严重性为威胁带来中等风险到的设备或设备数据。</span><span class="sxs-lookup"><span data-stu-id="ce911-127">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="ce911-128">高</span><span class="sxs-lookup"><span data-stu-id="ce911-128">high</span></span>|<span data-ttu-id="ce911-129">4</span><span class="sxs-lookup"><span data-stu-id="ce911-129">4</span></span>|<span data-ttu-id="ce911-130">设备威胁保护级别要求： 高。</span><span class="sxs-lookup"><span data-stu-id="ce911-130">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="ce911-131">高代表严重性为会造成严重到设备或设备数据风险的威胁。</span><span class="sxs-lookup"><span data-stu-id="ce911-131">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="ce911-132">notSet</span><span class="sxs-lookup"><span data-stu-id="ce911-132">notSet</span></span>|<span data-ttu-id="ce911-133">10</span><span class="sxs-lookup"><span data-stu-id="ce911-133">10</span></span>|<span data-ttu-id="ce911-134">设备威胁保护级别要求： 未设置。</span><span class="sxs-lookup"><span data-stu-id="ce911-134">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="ce911-135">不是设备，以满足了威胁保护级别不要求集代表。</span><span class="sxs-lookup"><span data-stu-id="ce911-135">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|




