---
title: deviceThreatProtectionLevel 枚举类型
description: 设备的设备威胁保护 API 的威胁保护级别。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a5b908b3d978c6a05897f466e43651b50f9931b2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974976"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="047c2-103">deviceThreatProtectionLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="047c2-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="047c2-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="047c2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="047c2-105">设备的设备威胁保护 API 的威胁保护级别。</span><span class="sxs-lookup"><span data-stu-id="047c2-105">Device threat protection levels for the Device Threat Protection API.</span></span>
## <a name="members"></a><span data-ttu-id="047c2-106">成员</span><span class="sxs-lookup"><span data-stu-id="047c2-106">Members</span></span>
|<span data-ttu-id="047c2-107">成员</span><span class="sxs-lookup"><span data-stu-id="047c2-107">Member</span></span>|<span data-ttu-id="047c2-108">值</span><span class="sxs-lookup"><span data-stu-id="047c2-108">Value</span></span>|<span data-ttu-id="047c2-109">说明</span><span class="sxs-lookup"><span data-stu-id="047c2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="047c2-110">不可用</span><span class="sxs-lookup"><span data-stu-id="047c2-110">unavailable</span></span>|<span data-ttu-id="047c2-111">0</span><span class="sxs-lookup"><span data-stu-id="047c2-111">0</span></span>|<span data-ttu-id="047c2-112">默认值。</span><span class="sxs-lookup"><span data-stu-id="047c2-112">Default Value.</span></span> <span data-ttu-id="047c2-113">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="047c2-113">Do not use.</span></span>|
|<span data-ttu-id="047c2-114">保护</span><span class="sxs-lookup"><span data-stu-id="047c2-114">secured</span></span>|<span data-ttu-id="047c2-115">1</span><span class="sxs-lookup"><span data-stu-id="047c2-115">1</span></span>|<span data-ttu-id="047c2-116">设备威胁级别要求： 安全。</span><span class="sxs-lookup"><span data-stu-id="047c2-116">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="047c2-117">这是最安全的级别，表示在设备上未发现任何威胁。</span><span class="sxs-lookup"><span data-stu-id="047c2-117">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="047c2-118">低</span><span class="sxs-lookup"><span data-stu-id="047c2-118">low</span></span>|<span data-ttu-id="047c2-119">2</span><span class="sxs-lookup"><span data-stu-id="047c2-119">2</span></span>|<span data-ttu-id="047c2-120">设备威胁保护级别要求： 低。</span><span class="sxs-lookup"><span data-stu-id="047c2-120">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="047c2-121">低代表严重性为会带来风险降至最低到设备或设备数据的威胁。</span><span class="sxs-lookup"><span data-stu-id="047c2-121">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="047c2-122">中等</span><span class="sxs-lookup"><span data-stu-id="047c2-122">medium</span></span>|<span data-ttu-id="047c2-123">3</span><span class="sxs-lookup"><span data-stu-id="047c2-123">3</span></span>|<span data-ttu-id="047c2-124">设备威胁保护级别要求： 中等。</span><span class="sxs-lookup"><span data-stu-id="047c2-124">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="047c2-125">中等代表严重性为威胁带来中等风险到的设备或设备数据。</span><span class="sxs-lookup"><span data-stu-id="047c2-125">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="047c2-126">高</span><span class="sxs-lookup"><span data-stu-id="047c2-126">high</span></span>|<span data-ttu-id="047c2-127">4</span><span class="sxs-lookup"><span data-stu-id="047c2-127">4</span></span>|<span data-ttu-id="047c2-128">设备威胁保护级别要求： 高。</span><span class="sxs-lookup"><span data-stu-id="047c2-128">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="047c2-129">高代表严重性为会造成严重到设备或设备数据风险的威胁。</span><span class="sxs-lookup"><span data-stu-id="047c2-129">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="047c2-130">notSet</span><span class="sxs-lookup"><span data-stu-id="047c2-130">notSet</span></span>|<span data-ttu-id="047c2-131">10</span><span class="sxs-lookup"><span data-stu-id="047c2-131">10</span></span>|<span data-ttu-id="047c2-132">设备威胁保护级别要求： 未设置。</span><span class="sxs-lookup"><span data-stu-id="047c2-132">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="047c2-133">不是设备，以满足了威胁保护级别不要求集代表。</span><span class="sxs-lookup"><span data-stu-id="047c2-133">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|



