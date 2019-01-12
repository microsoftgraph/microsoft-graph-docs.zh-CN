---
title: managedDevicePartnerReportedHealthState 枚举类型
description: 可用的运行状况状态的设备运行状况 API
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 14fe3c6769e717abb3d899e6ce7da33215a04a78
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991760"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a><span data-ttu-id="e02eb-103">managedDevicePartnerReportedHealthState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e02eb-103">managedDevicePartnerReportedHealthState enum type</span></span>

> <span data-ttu-id="e02eb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e02eb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e02eb-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e02eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e02eb-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e02eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e02eb-107">可用的运行状况状态的设备运行状况 API</span><span class="sxs-lookup"><span data-stu-id="e02eb-107">Available health states for the Device Health API</span></span>
## <a name="members"></a><span data-ttu-id="e02eb-108">成员</span><span class="sxs-lookup"><span data-stu-id="e02eb-108">Members</span></span>
|<span data-ttu-id="e02eb-109">成员</span><span class="sxs-lookup"><span data-stu-id="e02eb-109">Member</span></span>|<span data-ttu-id="e02eb-110">值</span><span class="sxs-lookup"><span data-stu-id="e02eb-110">Value</span></span>|<span data-ttu-id="e02eb-111">说明</span><span class="sxs-lookup"><span data-stu-id="e02eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e02eb-112">unknown</span><span class="sxs-lookup"><span data-stu-id="e02eb-112">unknown</span></span>|<span data-ttu-id="e02eb-113">0</span><span class="sxs-lookup"><span data-stu-id="e02eb-113">0</span></span>|<span data-ttu-id="e02eb-114">设备运行状况不尚未报告</span><span class="sxs-lookup"><span data-stu-id="e02eb-114">Device health state is not yet reported</span></span>|
|<span data-ttu-id="e02eb-115">激活</span><span class="sxs-lookup"><span data-stu-id="e02eb-115">activated</span></span>|<span data-ttu-id="e02eb-116">1</span><span class="sxs-lookup"><span data-stu-id="e02eb-116">1</span></span>|<span data-ttu-id="e02eb-117">设备已激活通过移动的威胁防御合作伙伴，但不是报告运行状况。</span><span class="sxs-lookup"><span data-stu-id="e02eb-117">Device has been activated by a mobile threat defense partner, but has not yet reported health.</span></span>|
|<span data-ttu-id="e02eb-118">停用</span><span class="sxs-lookup"><span data-stu-id="e02eb-118">deactivated</span></span>|<span data-ttu-id="e02eb-119">2</span><span class="sxs-lookup"><span data-stu-id="e02eb-119">2</span></span>|<span data-ttu-id="e02eb-120">已由移动的威胁防御合作伙伴停用设备。</span><span class="sxs-lookup"><span data-stu-id="e02eb-120">Device has been deactivated by a mobile threat defense partner.</span></span> <span data-ttu-id="e02eb-121">未知设备运行状况。</span><span class="sxs-lookup"><span data-stu-id="e02eb-121">The device health is not known.</span></span>|
|<span data-ttu-id="e02eb-122">保护</span><span class="sxs-lookup"><span data-stu-id="e02eb-122">secured</span></span>|<span data-ttu-id="e02eb-123">3</span><span class="sxs-lookup"><span data-stu-id="e02eb-123">3</span></span>|<span data-ttu-id="e02eb-124">设备被视为受移动的威胁防御合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="e02eb-124">Device is considered secured by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="e02eb-125">lowSeverity</span><span class="sxs-lookup"><span data-stu-id="e02eb-125">lowSeverity</span></span>|<span data-ttu-id="e02eb-126">4</span><span class="sxs-lookup"><span data-stu-id="e02eb-126">4</span></span>|<span data-ttu-id="e02eb-127">设备通过移动的威胁防御合作伙伴视为低威胁。</span><span class="sxs-lookup"><span data-stu-id="e02eb-127">Device is considered low threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="e02eb-128">mediumSeverity</span><span class="sxs-lookup"><span data-stu-id="e02eb-128">mediumSeverity</span></span>|<span data-ttu-id="e02eb-129">5</span><span class="sxs-lookup"><span data-stu-id="e02eb-129">5</span></span>|<span data-ttu-id="e02eb-130">设备通过移动的威胁防御合作伙伴视为中型威胁。</span><span class="sxs-lookup"><span data-stu-id="e02eb-130">Device is considered medium threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="e02eb-131">highSeverity</span><span class="sxs-lookup"><span data-stu-id="e02eb-131">highSeverity</span></span>|<span data-ttu-id="e02eb-132">6</span><span class="sxs-lookup"><span data-stu-id="e02eb-132">6</span></span>|<span data-ttu-id="e02eb-133">设备通过移动的威胁防御合作伙伴视为高威胁。</span><span class="sxs-lookup"><span data-stu-id="e02eb-133">Device is considered high threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="e02eb-134">未响应</span><span class="sxs-lookup"><span data-stu-id="e02eb-134">unresponsive</span></span>|<span data-ttu-id="e02eb-135">7</span><span class="sxs-lookup"><span data-stu-id="e02eb-135">7</span></span>|<span data-ttu-id="e02eb-136">移动的威胁防御合作伙伴被视为设备未响应。</span><span class="sxs-lookup"><span data-stu-id="e02eb-136">Device is considered unresponsive by the mobile threat defense partner.</span></span> <span data-ttu-id="e02eb-137">未知设备运行状况。</span><span class="sxs-lookup"><span data-stu-id="e02eb-137">The device health is not known.</span></span>|
|<span data-ttu-id="e02eb-138">威胁</span><span class="sxs-lookup"><span data-stu-id="e02eb-138">compromised</span></span>|<span data-ttu-id="e02eb-139">8</span><span class="sxs-lookup"><span data-stu-id="e02eb-139">8</span></span>|<span data-ttu-id="e02eb-140">设备被视为受到威胁防御合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="e02eb-140">Device is considered compromised by the Threat Defense partner.</span></span> <span data-ttu-id="e02eb-141">这意味着设备具有活动的威胁或无法由最终用户轻松修正风险和用户应联系其 IT 管理员。</span><span class="sxs-lookup"><span data-stu-id="e02eb-141">This means the device has an active Threat or Risk which cannot be easily remediated by the end user and the user should contact their IT Admin.</span></span>|
|<span data-ttu-id="e02eb-142">配置错误</span><span class="sxs-lookup"><span data-stu-id="e02eb-142">misconfigured</span></span>|<span data-ttu-id="e02eb-143">9</span><span class="sxs-lookup"><span data-stu-id="e02eb-143">9</span></span>|<span data-ttu-id="e02eb-144">设备被视为与威胁防御合作伙伴配置正确。</span><span class="sxs-lookup"><span data-stu-id="e02eb-144">Device is considered misconfigured with the Threat Defense partner.</span></span> <span data-ttu-id="e02eb-145">这意味着设备缺少必需的配置文件或配置威胁防御伙伴能够正常工作，因此威胁或不能完成风险分析。</span><span class="sxs-lookup"><span data-stu-id="e02eb-145">This means the device is missing a required profile or configuration for the Threat Defense Partner to function properly and is thus threat or risk analysis is not able to complete.</span></span>|





