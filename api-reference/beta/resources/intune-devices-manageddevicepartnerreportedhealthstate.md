---
title: managedDevicePartnerReportedHealthState 枚举类型
description: 设备运行状况 API 的可用运行状况状态
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60a3071094e2667b896401c6df29977f9923884c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143769"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a><span data-ttu-id="19509-103">managedDevicePartnerReportedHealthState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="19509-103">managedDevicePartnerReportedHealthState enum type</span></span>

> <span data-ttu-id="19509-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="19509-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19509-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="19509-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19509-106">设备运行状况 API 的可用运行状况状态</span><span class="sxs-lookup"><span data-stu-id="19509-106">Available health states for the Device Health API</span></span>

## <a name="members"></a><span data-ttu-id="19509-107">成员</span><span class="sxs-lookup"><span data-stu-id="19509-107">Members</span></span>
|<span data-ttu-id="19509-108">成员</span><span class="sxs-lookup"><span data-stu-id="19509-108">Member</span></span>|<span data-ttu-id="19509-109">值</span><span class="sxs-lookup"><span data-stu-id="19509-109">Value</span></span>|<span data-ttu-id="19509-110">说明</span><span class="sxs-lookup"><span data-stu-id="19509-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19509-111">unknown</span><span class="sxs-lookup"><span data-stu-id="19509-111">unknown</span></span>|<span data-ttu-id="19509-112">0</span><span class="sxs-lookup"><span data-stu-id="19509-112">0</span></span>|<span data-ttu-id="19509-113">尚未报告设备运行状况状态</span><span class="sxs-lookup"><span data-stu-id="19509-113">Device health state is not yet reported</span></span>|
|<span data-ttu-id="19509-114">已</span><span class="sxs-lookup"><span data-stu-id="19509-114">activated</span></span>|<span data-ttu-id="19509-115">1</span><span class="sxs-lookup"><span data-stu-id="19509-115">1</span></span>|<span data-ttu-id="19509-116">设备已由移动威胁防护合作伙伴激活, 但尚未报告运行状况。</span><span class="sxs-lookup"><span data-stu-id="19509-116">Device has been activated by a mobile threat defense partner, but has not yet reported health.</span></span>|
|<span data-ttu-id="19509-117">失效</span><span class="sxs-lookup"><span data-stu-id="19509-117">deactivated</span></span>|<span data-ttu-id="19509-118">双面</span><span class="sxs-lookup"><span data-stu-id="19509-118">2</span></span>|<span data-ttu-id="19509-119">设备已被移动威胁防护合作伙伴停用。</span><span class="sxs-lookup"><span data-stu-id="19509-119">Device has been deactivated by a mobile threat defense partner.</span></span> <span data-ttu-id="19509-120">设备运行状况未知。</span><span class="sxs-lookup"><span data-stu-id="19509-120">The device health is not known.</span></span>|
|<span data-ttu-id="19509-121">加密</span><span class="sxs-lookup"><span data-stu-id="19509-121">secured</span></span>|<span data-ttu-id="19509-122">第三章</span><span class="sxs-lookup"><span data-stu-id="19509-122">3</span></span>|<span data-ttu-id="19509-123">移动威胁防护合作伙伴认为设备受安全保护。</span><span class="sxs-lookup"><span data-stu-id="19509-123">Device is considered secured by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="19509-124">lowSeverity</span><span class="sxs-lookup"><span data-stu-id="19509-124">lowSeverity</span></span>|<span data-ttu-id="19509-125">4</span><span class="sxs-lookup"><span data-stu-id="19509-125">4</span></span>|<span data-ttu-id="19509-126">移动威胁防护合作伙伴将设备视为低威胁。</span><span class="sxs-lookup"><span data-stu-id="19509-126">Device is considered low threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="19509-127">mediumSeverity</span><span class="sxs-lookup"><span data-stu-id="19509-127">mediumSeverity</span></span>|<span data-ttu-id="19509-128">5</span><span class="sxs-lookup"><span data-stu-id="19509-128">5</span></span>|<span data-ttu-id="19509-129">移动威胁防护合作伙伴认为设备是中型威胁。</span><span class="sxs-lookup"><span data-stu-id="19509-129">Device is considered medium threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="19509-130">highSeverity</span><span class="sxs-lookup"><span data-stu-id="19509-130">highSeverity</span></span>|<span data-ttu-id="19509-131">型</span><span class="sxs-lookup"><span data-stu-id="19509-131">6</span></span>|<span data-ttu-id="19509-132">移动威胁防护合作伙伴将设备视为高威胁。</span><span class="sxs-lookup"><span data-stu-id="19509-132">Device is considered high threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="19509-133">无</span><span class="sxs-lookup"><span data-stu-id="19509-133">unresponsive</span></span>|<span data-ttu-id="19509-134">步</span><span class="sxs-lookup"><span data-stu-id="19509-134">7</span></span>|<span data-ttu-id="19509-135">移动威胁防护合作伙伴认为设备无响应。</span><span class="sxs-lookup"><span data-stu-id="19509-135">Device is considered unresponsive by the mobile threat defense partner.</span></span> <span data-ttu-id="19509-136">设备运行状况未知。</span><span class="sxs-lookup"><span data-stu-id="19509-136">The device health is not known.</span></span>|
|<span data-ttu-id="19509-137">威胁</span><span class="sxs-lookup"><span data-stu-id="19509-137">compromised</span></span>|<span data-ttu-id="19509-138">utf-8</span><span class="sxs-lookup"><span data-stu-id="19509-138">8</span></span>|<span data-ttu-id="19509-139">威胁防御合作伙伴认为设备受到威胁。</span><span class="sxs-lookup"><span data-stu-id="19509-139">Device is considered compromised by the Threat Defense partner.</span></span> <span data-ttu-id="19509-140">这意味着该设备具有活跃的威胁或风险, 最终用户无法轻松修正该设备, 并且用户应联系其 IT 管理员。</span><span class="sxs-lookup"><span data-stu-id="19509-140">This means the device has an active Threat or Risk which cannot be easily remediated by the end user and the user should contact their IT Admin.</span></span>|
|<span data-ttu-id="19509-141">配置错误</span><span class="sxs-lookup"><span data-stu-id="19509-141">misconfigured</span></span>|<span data-ttu-id="19509-142">第</span><span class="sxs-lookup"><span data-stu-id="19509-142">9</span></span>|<span data-ttu-id="19509-143">将设备视为与威胁防护合作伙伴配置不正确。</span><span class="sxs-lookup"><span data-stu-id="19509-143">Device is considered misconfigured with the Threat Defense partner.</span></span> <span data-ttu-id="19509-144">这意味着设备缺少必需的配置文件或配置以使威胁防护合作伙伴正常运行, 因此威胁或风险分析无法完成。</span><span class="sxs-lookup"><span data-stu-id="19509-144">This means the device is missing a required profile or configuration for the Threat Defense Partner to function properly and is thus threat or risk analysis is not able to complete.</span></span>|




