---
title: managedDevicePartnerReportedHealthState 枚举类型
description: 可用的运行状况状态的设备运行状况 API
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cb5b13ceceab27e1e88a69310a3198159f5e24c1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418825"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a><span data-ttu-id="27d2f-103">managedDevicePartnerReportedHealthState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="27d2f-103">managedDevicePartnerReportedHealthState enum type</span></span>

> <span data-ttu-id="27d2f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="27d2f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="27d2f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="27d2f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27d2f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="27d2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27d2f-107">可用的运行状况状态的设备运行状况 API</span><span class="sxs-lookup"><span data-stu-id="27d2f-107">Available health states for the Device Health API</span></span>

## <a name="members"></a><span data-ttu-id="27d2f-108">成员</span><span class="sxs-lookup"><span data-stu-id="27d2f-108">Members</span></span>
|<span data-ttu-id="27d2f-109">成员</span><span class="sxs-lookup"><span data-stu-id="27d2f-109">Member</span></span>|<span data-ttu-id="27d2f-110">值</span><span class="sxs-lookup"><span data-stu-id="27d2f-110">Value</span></span>|<span data-ttu-id="27d2f-111">说明</span><span class="sxs-lookup"><span data-stu-id="27d2f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27d2f-112">unknown</span><span class="sxs-lookup"><span data-stu-id="27d2f-112">unknown</span></span>|<span data-ttu-id="27d2f-113">0</span><span class="sxs-lookup"><span data-stu-id="27d2f-113">0</span></span>|<span data-ttu-id="27d2f-114">设备运行状况不尚未报告</span><span class="sxs-lookup"><span data-stu-id="27d2f-114">Device health state is not yet reported</span></span>|
|<span data-ttu-id="27d2f-115">激活</span><span class="sxs-lookup"><span data-stu-id="27d2f-115">activated</span></span>|<span data-ttu-id="27d2f-116">1</span><span class="sxs-lookup"><span data-stu-id="27d2f-116">1</span></span>|<span data-ttu-id="27d2f-117">设备已激活通过移动的威胁防御合作伙伴，但不是报告运行状况。</span><span class="sxs-lookup"><span data-stu-id="27d2f-117">Device has been activated by a mobile threat defense partner, but has not yet reported health.</span></span>|
|<span data-ttu-id="27d2f-118">停用</span><span class="sxs-lookup"><span data-stu-id="27d2f-118">deactivated</span></span>|<span data-ttu-id="27d2f-119">2</span><span class="sxs-lookup"><span data-stu-id="27d2f-119">2</span></span>|<span data-ttu-id="27d2f-120">已由移动的威胁防御合作伙伴停用设备。</span><span class="sxs-lookup"><span data-stu-id="27d2f-120">Device has been deactivated by a mobile threat defense partner.</span></span> <span data-ttu-id="27d2f-121">未知设备运行状况。</span><span class="sxs-lookup"><span data-stu-id="27d2f-121">The device health is not known.</span></span>|
|<span data-ttu-id="27d2f-122">保护</span><span class="sxs-lookup"><span data-stu-id="27d2f-122">secured</span></span>|<span data-ttu-id="27d2f-123">3</span><span class="sxs-lookup"><span data-stu-id="27d2f-123">3</span></span>|<span data-ttu-id="27d2f-124">设备被视为受移动的威胁防御合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="27d2f-124">Device is considered secured by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="27d2f-125">lowSeverity</span><span class="sxs-lookup"><span data-stu-id="27d2f-125">lowSeverity</span></span>|<span data-ttu-id="27d2f-126">4</span><span class="sxs-lookup"><span data-stu-id="27d2f-126">4</span></span>|<span data-ttu-id="27d2f-127">设备通过移动的威胁防御合作伙伴视为低威胁。</span><span class="sxs-lookup"><span data-stu-id="27d2f-127">Device is considered low threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="27d2f-128">mediumSeverity</span><span class="sxs-lookup"><span data-stu-id="27d2f-128">mediumSeverity</span></span>|<span data-ttu-id="27d2f-129">5</span><span class="sxs-lookup"><span data-stu-id="27d2f-129">5</span></span>|<span data-ttu-id="27d2f-130">设备通过移动的威胁防御合作伙伴视为中型威胁。</span><span class="sxs-lookup"><span data-stu-id="27d2f-130">Device is considered medium threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="27d2f-131">highSeverity</span><span class="sxs-lookup"><span data-stu-id="27d2f-131">highSeverity</span></span>|<span data-ttu-id="27d2f-132">6</span><span class="sxs-lookup"><span data-stu-id="27d2f-132">6</span></span>|<span data-ttu-id="27d2f-133">设备通过移动的威胁防御合作伙伴视为高威胁。</span><span class="sxs-lookup"><span data-stu-id="27d2f-133">Device is considered high threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="27d2f-134">未响应</span><span class="sxs-lookup"><span data-stu-id="27d2f-134">unresponsive</span></span>|<span data-ttu-id="27d2f-135">7</span><span class="sxs-lookup"><span data-stu-id="27d2f-135">7</span></span>|<span data-ttu-id="27d2f-136">移动的威胁防御合作伙伴被视为设备未响应。</span><span class="sxs-lookup"><span data-stu-id="27d2f-136">Device is considered unresponsive by the mobile threat defense partner.</span></span> <span data-ttu-id="27d2f-137">未知设备运行状况。</span><span class="sxs-lookup"><span data-stu-id="27d2f-137">The device health is not known.</span></span>|
|<span data-ttu-id="27d2f-138">威胁</span><span class="sxs-lookup"><span data-stu-id="27d2f-138">compromised</span></span>|<span data-ttu-id="27d2f-139">8</span><span class="sxs-lookup"><span data-stu-id="27d2f-139">8</span></span>|<span data-ttu-id="27d2f-140">设备被视为受到威胁防御合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="27d2f-140">Device is considered compromised by the Threat Defense partner.</span></span> <span data-ttu-id="27d2f-141">这意味着设备具有活动的威胁或无法由最终用户轻松修正风险和用户应联系其 IT 管理员。</span><span class="sxs-lookup"><span data-stu-id="27d2f-141">This means the device has an active Threat or Risk which cannot be easily remediated by the end user and the user should contact their IT Admin.</span></span>|
|<span data-ttu-id="27d2f-142">配置错误</span><span class="sxs-lookup"><span data-stu-id="27d2f-142">misconfigured</span></span>|<span data-ttu-id="27d2f-143">9</span><span class="sxs-lookup"><span data-stu-id="27d2f-143">9</span></span>|<span data-ttu-id="27d2f-144">设备被视为与威胁防御合作伙伴配置正确。</span><span class="sxs-lookup"><span data-stu-id="27d2f-144">Device is considered misconfigured with the Threat Defense partner.</span></span> <span data-ttu-id="27d2f-145">这意味着设备缺少必需的配置文件或配置威胁防御伙伴能够正常工作，因此威胁或不能完成风险分析。</span><span class="sxs-lookup"><span data-stu-id="27d2f-145">This means the device is missing a required profile or configuration for the Threat Defense Partner to function properly and is thus threat or risk analysis is not able to complete.</span></span>|




