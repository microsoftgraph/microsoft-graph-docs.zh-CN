---
title: deviceThreatProtectionLevel 枚举类型
description: 设备的设备威胁保护 API 的威胁保护级别。
author: tfitzmac
ms.openlocfilehash: 755fd861196839ec261dd18f458b88aa97cf0191
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356005"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="d8e70-103">deviceThreatProtectionLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d8e70-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="d8e70-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d8e70-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8e70-105">设备的设备威胁保护 API 的威胁保护级别。</span><span class="sxs-lookup"><span data-stu-id="d8e70-105">Device threat protection levels for the Device Threat Protection API.</span></span>
## <a name="members"></a><span data-ttu-id="d8e70-106">成员</span><span class="sxs-lookup"><span data-stu-id="d8e70-106">Members</span></span>
|<span data-ttu-id="d8e70-107">成员</span><span class="sxs-lookup"><span data-stu-id="d8e70-107">Member</span></span>|<span data-ttu-id="d8e70-108">值</span><span class="sxs-lookup"><span data-stu-id="d8e70-108">Value</span></span>|<span data-ttu-id="d8e70-109">说明</span><span class="sxs-lookup"><span data-stu-id="d8e70-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8e70-110">不可用</span><span class="sxs-lookup"><span data-stu-id="d8e70-110">unavailable</span></span>|<span data-ttu-id="d8e70-111">0</span><span class="sxs-lookup"><span data-stu-id="d8e70-111">0</span></span>|<span data-ttu-id="d8e70-112">默认值。</span><span class="sxs-lookup"><span data-stu-id="d8e70-112">Default Value.</span></span> <span data-ttu-id="d8e70-113">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="d8e70-113">Do not use.</span></span>|
|<span data-ttu-id="d8e70-114">保护</span><span class="sxs-lookup"><span data-stu-id="d8e70-114">secured</span></span>|<span data-ttu-id="d8e70-115">1</span><span class="sxs-lookup"><span data-stu-id="d8e70-115">1</span></span>|<span data-ttu-id="d8e70-116">设备威胁级别要求： 安全。</span><span class="sxs-lookup"><span data-stu-id="d8e70-116">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="d8e70-117">这是最安全的级别，表示在设备上未发现任何威胁。</span><span class="sxs-lookup"><span data-stu-id="d8e70-117">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="d8e70-118">低</span><span class="sxs-lookup"><span data-stu-id="d8e70-118">low</span></span>|<span data-ttu-id="d8e70-119">2</span><span class="sxs-lookup"><span data-stu-id="d8e70-119">2</span></span>|<span data-ttu-id="d8e70-120">设备威胁保护级别要求： 低。</span><span class="sxs-lookup"><span data-stu-id="d8e70-120">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="d8e70-121">低代表严重性为会带来风险降至最低到设备或设备数据的威胁。</span><span class="sxs-lookup"><span data-stu-id="d8e70-121">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="d8e70-122">中等</span><span class="sxs-lookup"><span data-stu-id="d8e70-122">medium</span></span>|<span data-ttu-id="d8e70-123">3</span><span class="sxs-lookup"><span data-stu-id="d8e70-123">3</span></span>|<span data-ttu-id="d8e70-124">设备威胁保护级别要求： 中等。</span><span class="sxs-lookup"><span data-stu-id="d8e70-124">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="d8e70-125">中等代表严重性为威胁带来中等风险到的设备或设备数据。</span><span class="sxs-lookup"><span data-stu-id="d8e70-125">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="d8e70-126">高</span><span class="sxs-lookup"><span data-stu-id="d8e70-126">high</span></span>|<span data-ttu-id="d8e70-127">4</span><span class="sxs-lookup"><span data-stu-id="d8e70-127">4</span></span>|<span data-ttu-id="d8e70-128">设备威胁保护级别要求： 高。</span><span class="sxs-lookup"><span data-stu-id="d8e70-128">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="d8e70-129">高代表严重性为会造成严重到设备或设备数据风险的威胁。</span><span class="sxs-lookup"><span data-stu-id="d8e70-129">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="d8e70-130">notSet</span><span class="sxs-lookup"><span data-stu-id="d8e70-130">notSet</span></span>|<span data-ttu-id="d8e70-131">10</span><span class="sxs-lookup"><span data-stu-id="d8e70-131">10</span></span>|<span data-ttu-id="d8e70-132">设备威胁保护级别要求： 未设置。</span><span class="sxs-lookup"><span data-stu-id="d8e70-132">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="d8e70-133">不是设备，以满足了威胁保护级别不要求集代表。</span><span class="sxs-lookup"><span data-stu-id="d8e70-133">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|



