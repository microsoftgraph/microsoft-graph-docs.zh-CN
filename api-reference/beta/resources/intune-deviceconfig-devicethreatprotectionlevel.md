---
title: deviceThreatProtectionLevel 枚举类型
description: 设备的设备威胁保护 API 的威胁保护级别。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3b7cab18c53b08256d358be98fc7c66edef7ae82
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866288"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="696f5-103">deviceThreatProtectionLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="696f5-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="696f5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="696f5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="696f5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="696f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="696f5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="696f5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="696f5-107">设备的设备威胁保护 API 的威胁保护级别。</span><span class="sxs-lookup"><span data-stu-id="696f5-107">Device threat protection levels for the Device Threat Protection API.</span></span>
## <a name="members"></a><span data-ttu-id="696f5-108">成员</span><span class="sxs-lookup"><span data-stu-id="696f5-108">Members</span></span>
|<span data-ttu-id="696f5-109">成员</span><span class="sxs-lookup"><span data-stu-id="696f5-109">Member</span></span>|<span data-ttu-id="696f5-110">值</span><span class="sxs-lookup"><span data-stu-id="696f5-110">Value</span></span>|<span data-ttu-id="696f5-111">Description</span><span class="sxs-lookup"><span data-stu-id="696f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="696f5-112">不可用</span><span class="sxs-lookup"><span data-stu-id="696f5-112">unavailable</span></span>|<span data-ttu-id="696f5-113">0</span><span class="sxs-lookup"><span data-stu-id="696f5-113">0</span></span>|<span data-ttu-id="696f5-114">默认值。</span><span class="sxs-lookup"><span data-stu-id="696f5-114">Default Value.</span></span> <span data-ttu-id="696f5-115">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="696f5-115">Do not use.</span></span>|
|<span data-ttu-id="696f5-116">保护</span><span class="sxs-lookup"><span data-stu-id="696f5-116">secured</span></span>|<span data-ttu-id="696f5-117">1</span><span class="sxs-lookup"><span data-stu-id="696f5-117">1</span></span>|<span data-ttu-id="696f5-118">设备威胁级别要求： 安全。</span><span class="sxs-lookup"><span data-stu-id="696f5-118">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="696f5-119">这是最安全的级别，表示在设备上未发现任何威胁。</span><span class="sxs-lookup"><span data-stu-id="696f5-119">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="696f5-120">低</span><span class="sxs-lookup"><span data-stu-id="696f5-120">low</span></span>|<span data-ttu-id="696f5-121">2</span><span class="sxs-lookup"><span data-stu-id="696f5-121">2</span></span>|<span data-ttu-id="696f5-122">设备威胁保护级别要求： 低。</span><span class="sxs-lookup"><span data-stu-id="696f5-122">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="696f5-123">低代表严重性为会带来风险降至最低到设备或设备数据的威胁。</span><span class="sxs-lookup"><span data-stu-id="696f5-123">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="696f5-124">中等</span><span class="sxs-lookup"><span data-stu-id="696f5-124">medium</span></span>|<span data-ttu-id="696f5-125">3</span><span class="sxs-lookup"><span data-stu-id="696f5-125">3</span></span>|<span data-ttu-id="696f5-126">设备威胁保护级别要求： 中等。</span><span class="sxs-lookup"><span data-stu-id="696f5-126">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="696f5-127">中等代表严重性为威胁带来中等风险到的设备或设备数据。</span><span class="sxs-lookup"><span data-stu-id="696f5-127">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="696f5-128">高</span><span class="sxs-lookup"><span data-stu-id="696f5-128">high</span></span>|<span data-ttu-id="696f5-129">4</span><span class="sxs-lookup"><span data-stu-id="696f5-129">4</span></span>|<span data-ttu-id="696f5-130">设备威胁保护级别要求： 高。</span><span class="sxs-lookup"><span data-stu-id="696f5-130">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="696f5-131">高代表严重性为会造成严重到设备或设备数据风险的威胁。</span><span class="sxs-lookup"><span data-stu-id="696f5-131">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="696f5-132">notSet</span><span class="sxs-lookup"><span data-stu-id="696f5-132">notSet</span></span>|<span data-ttu-id="696f5-133">10</span><span class="sxs-lookup"><span data-stu-id="696f5-133">10</span></span>|<span data-ttu-id="696f5-134">设备威胁保护级别要求： 未设置。</span><span class="sxs-lookup"><span data-stu-id="696f5-134">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="696f5-135">不是设备，以满足了威胁保护级别不要求集代表。</span><span class="sxs-lookup"><span data-stu-id="696f5-135">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|





