---
title: managedDevicePartnerReportedHealthState 枚举类型
description: 设备运行状况 API 的可用运行状况状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4c1d3166a5e55c39c5904b7bc1ac6239b3cc11cf
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751676"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a><span data-ttu-id="fcf8e-103">managedDevicePartnerReportedHealthState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fcf8e-103">managedDevicePartnerReportedHealthState enum type</span></span>

<span data-ttu-id="fcf8e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcf8e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fcf8e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fcf8e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcf8e-106">设备运行状况 API 的可用运行状况状态</span><span class="sxs-lookup"><span data-stu-id="fcf8e-106">Available health states for the Device Health API</span></span>

## <a name="members"></a><span data-ttu-id="fcf8e-107">成员</span><span class="sxs-lookup"><span data-stu-id="fcf8e-107">Members</span></span>
|<span data-ttu-id="fcf8e-108">成员</span><span class="sxs-lookup"><span data-stu-id="fcf8e-108">Member</span></span>|<span data-ttu-id="fcf8e-109">值</span><span class="sxs-lookup"><span data-stu-id="fcf8e-109">Value</span></span>|<span data-ttu-id="fcf8e-110">Description</span><span class="sxs-lookup"><span data-stu-id="fcf8e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcf8e-111">unknown</span><span class="sxs-lookup"><span data-stu-id="fcf8e-111">unknown</span></span>|<span data-ttu-id="fcf8e-112">0</span><span class="sxs-lookup"><span data-stu-id="fcf8e-112">0</span></span>|<span data-ttu-id="fcf8e-113">尚未报告设备运行状况</span><span class="sxs-lookup"><span data-stu-id="fcf8e-113">Device health state is not yet reported</span></span>|
|<span data-ttu-id="fcf8e-114">activated</span><span class="sxs-lookup"><span data-stu-id="fcf8e-114">activated</span></span>|<span data-ttu-id="fcf8e-115">1</span><span class="sxs-lookup"><span data-stu-id="fcf8e-115">1</span></span>|<span data-ttu-id="fcf8e-116">设备已由移动威胁防护合作伙伴激活，但尚未报告运行状况。</span><span class="sxs-lookup"><span data-stu-id="fcf8e-116">Device has been activated by a mobile threat defense partner, but has not yet reported health.</span></span>|
|<span data-ttu-id="fcf8e-117">deactivated</span><span class="sxs-lookup"><span data-stu-id="fcf8e-117">deactivated</span></span>|<span data-ttu-id="fcf8e-118">2</span><span class="sxs-lookup"><span data-stu-id="fcf8e-118">2</span></span>|<span data-ttu-id="fcf8e-119">设备已被移动威胁防护合作伙伴停用。</span><span class="sxs-lookup"><span data-stu-id="fcf8e-119">Device has been deactivated by a mobile threat defense partner.</span></span> <span data-ttu-id="fcf8e-120">设备运行状况未知。</span><span class="sxs-lookup"><span data-stu-id="fcf8e-120">The device health is not known.</span></span>|
|<span data-ttu-id="fcf8e-121">secured</span><span class="sxs-lookup"><span data-stu-id="fcf8e-121">secured</span></span>|<span data-ttu-id="fcf8e-122">3</span><span class="sxs-lookup"><span data-stu-id="fcf8e-122">3</span></span>|<span data-ttu-id="fcf8e-123">设备被视为受移动威胁防护合作伙伴保护。</span><span class="sxs-lookup"><span data-stu-id="fcf8e-123">Device is considered secured by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="fcf8e-124">lowSeverity</span><span class="sxs-lookup"><span data-stu-id="fcf8e-124">lowSeverity</span></span>|<span data-ttu-id="fcf8e-125">4 </span><span class="sxs-lookup"><span data-stu-id="fcf8e-125">4</span></span>|<span data-ttu-id="fcf8e-126">移动威胁防护合作伙伴将设备视为低威胁。</span><span class="sxs-lookup"><span data-stu-id="fcf8e-126">Device is considered low threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="fcf8e-127">mediumSeverity</span><span class="sxs-lookup"><span data-stu-id="fcf8e-127">mediumSeverity</span></span>|<span data-ttu-id="fcf8e-128">5 </span><span class="sxs-lookup"><span data-stu-id="fcf8e-128">5</span></span>|<span data-ttu-id="fcf8e-129">移动威胁防护合作伙伴将设备视为中等威胁。</span><span class="sxs-lookup"><span data-stu-id="fcf8e-129">Device is considered medium threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="fcf8e-130">highSeverity</span><span class="sxs-lookup"><span data-stu-id="fcf8e-130">highSeverity</span></span>|<span data-ttu-id="fcf8e-131">6 </span><span class="sxs-lookup"><span data-stu-id="fcf8e-131">6</span></span>|<span data-ttu-id="fcf8e-132">移动威胁防护合作伙伴将设备视为高威胁。</span><span class="sxs-lookup"><span data-stu-id="fcf8e-132">Device is considered high threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="fcf8e-133">unresponsive</span><span class="sxs-lookup"><span data-stu-id="fcf8e-133">unresponsive</span></span>|<span data-ttu-id="fcf8e-134">7 </span><span class="sxs-lookup"><span data-stu-id="fcf8e-134">7</span></span>|<span data-ttu-id="fcf8e-135">移动威胁防护合作伙伴认为设备没有响应。</span><span class="sxs-lookup"><span data-stu-id="fcf8e-135">Device is considered unresponsive by the mobile threat defense partner.</span></span> <span data-ttu-id="fcf8e-136">设备运行状况未知。</span><span class="sxs-lookup"><span data-stu-id="fcf8e-136">The device health is not known.</span></span>|
|<span data-ttu-id="fcf8e-137">compromised</span><span class="sxs-lookup"><span data-stu-id="fcf8e-137">compromised</span></span>|<span data-ttu-id="fcf8e-138">8 </span><span class="sxs-lookup"><span data-stu-id="fcf8e-138">8</span></span>|<span data-ttu-id="fcf8e-139">威胁防护合作伙伴认为设备遭到入侵。</span><span class="sxs-lookup"><span data-stu-id="fcf8e-139">Device is considered compromised by the Threat Defense partner.</span></span> <span data-ttu-id="fcf8e-140">这意味着设备具有活动威胁或风险，最终用户无法轻松修复此威胁或风险，用户应联系其 IT 管理员。</span><span class="sxs-lookup"><span data-stu-id="fcf8e-140">This means the device has an active Threat or Risk which cannot be easily remediated by the end user and the user should contact their IT Admin.</span></span>|
|<span data-ttu-id="fcf8e-141">misconfigured</span><span class="sxs-lookup"><span data-stu-id="fcf8e-141">misconfigured</span></span>|<span data-ttu-id="fcf8e-142">9 </span><span class="sxs-lookup"><span data-stu-id="fcf8e-142">9</span></span>|<span data-ttu-id="fcf8e-143">设备被视为与威胁防护合作伙伴配置不当。</span><span class="sxs-lookup"><span data-stu-id="fcf8e-143">Device is considered misconfigured with the Threat Defense partner.</span></span> <span data-ttu-id="fcf8e-144">这意味着设备缺少所需配置文件或配置，威胁防护合作伙伴才能正常运行，因此无法完成威胁或风险分析。</span><span class="sxs-lookup"><span data-stu-id="fcf8e-144">This means the device is missing a required profile or configuration for the Threat Defense Partner to function properly and is thus threat or risk analysis is not able to complete.</span></span>|




