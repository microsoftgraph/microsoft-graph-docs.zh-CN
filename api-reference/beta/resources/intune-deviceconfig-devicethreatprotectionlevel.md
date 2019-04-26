---
title: deviceThreatProtectionLevel 枚举类型
description: 设备威胁防护 API 的设备威胁保护级别。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 311a2e9a8db68d41d3c4a55f9691446b4e96c2d3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567212"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="3f395-103">deviceThreatProtectionLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3f395-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="3f395-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3f395-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f395-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3f395-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f395-106">设备威胁防护 API 的设备威胁保护级别。</span><span class="sxs-lookup"><span data-stu-id="3f395-106">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="3f395-107">成员</span><span class="sxs-lookup"><span data-stu-id="3f395-107">Members</span></span>
|<span data-ttu-id="3f395-108">成员</span><span class="sxs-lookup"><span data-stu-id="3f395-108">Member</span></span>|<span data-ttu-id="3f395-109">值</span><span class="sxs-lookup"><span data-stu-id="3f395-109">Value</span></span>|<span data-ttu-id="3f395-110">说明</span><span class="sxs-lookup"><span data-stu-id="3f395-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f395-111">才</span><span class="sxs-lookup"><span data-stu-id="3f395-111">unavailable</span></span>|<span data-ttu-id="3f395-112">0</span><span class="sxs-lookup"><span data-stu-id="3f395-112">0</span></span>|<span data-ttu-id="3f395-113">默认值。</span><span class="sxs-lookup"><span data-stu-id="3f395-113">Default Value.</span></span> <span data-ttu-id="3f395-114">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="3f395-114">Do not use.</span></span>|
|<span data-ttu-id="3f395-115">加密</span><span class="sxs-lookup"><span data-stu-id="3f395-115">secured</span></span>|<span data-ttu-id="3f395-116">1</span><span class="sxs-lookup"><span data-stu-id="3f395-116">1</span></span>|<span data-ttu-id="3f395-117">设备威胁级别要求: 安全。</span><span class="sxs-lookup"><span data-stu-id="3f395-117">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="3f395-118">这是最安全的级别, 表示在设备上未发现任何威胁。</span><span class="sxs-lookup"><span data-stu-id="3f395-118">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="3f395-119">降低</span><span class="sxs-lookup"><span data-stu-id="3f395-119">low</span></span>|<span data-ttu-id="3f395-120">2 </span><span class="sxs-lookup"><span data-stu-id="3f395-120">2</span></span>|<span data-ttu-id="3f395-121">设备威胁保护级别要求: 低。</span><span class="sxs-lookup"><span data-stu-id="3f395-121">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="3f395-122">Low 表示对设备或设备数据带来最小风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="3f395-122">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="3f395-123">中等</span><span class="sxs-lookup"><span data-stu-id="3f395-123">medium</span></span>|<span data-ttu-id="3f395-124">3 </span><span class="sxs-lookup"><span data-stu-id="3f395-124">3</span></span>|<span data-ttu-id="3f395-125">设备威胁保护级别要求: 中。</span><span class="sxs-lookup"><span data-stu-id="3f395-125">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="3f395-126">中型代表设备或设备数据面临中等风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="3f395-126">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="3f395-127">高效</span><span class="sxs-lookup"><span data-stu-id="3f395-127">high</span></span>|<span data-ttu-id="3f395-128">4 </span><span class="sxs-lookup"><span data-stu-id="3f395-128">4</span></span>|<span data-ttu-id="3f395-129">设备威胁保护级别要求: 高。</span><span class="sxs-lookup"><span data-stu-id="3f395-129">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="3f395-130">High 表示对设备或设备数据带来严重风险的威胁的严重程度。</span><span class="sxs-lookup"><span data-stu-id="3f395-130">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="3f395-131">notSet</span><span class="sxs-lookup"><span data-stu-id="3f395-131">notSet</span></span>|<span data-ttu-id="3f395-132">10 </span><span class="sxs-lookup"><span data-stu-id="3f395-132">10</span></span>|<span data-ttu-id="3f395-133">设备威胁保护级别要求: 未设置。</span><span class="sxs-lookup"><span data-stu-id="3f395-133">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="3f395-134">未设置表示设备不需要满足威胁保护级别。</span><span class="sxs-lookup"><span data-stu-id="3f395-134">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|





