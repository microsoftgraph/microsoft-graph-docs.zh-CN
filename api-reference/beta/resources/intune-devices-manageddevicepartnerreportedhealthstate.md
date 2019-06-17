---
title: managedDevicePartnerReportedHealthState 枚举类型
description: 设备运行状况 API 的可用运行状况状态
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0162903f7c38662b71a283a3dde30532aeb15326
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995054"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a><span data-ttu-id="568d2-103">managedDevicePartnerReportedHealthState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="568d2-103">managedDevicePartnerReportedHealthState enum type</span></span>

> <span data-ttu-id="568d2-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="568d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="568d2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="568d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="568d2-106">设备运行状况 API 的可用运行状况状态</span><span class="sxs-lookup"><span data-stu-id="568d2-106">Available health states for the Device Health API</span></span>

## <a name="members"></a><span data-ttu-id="568d2-107">成员</span><span class="sxs-lookup"><span data-stu-id="568d2-107">Members</span></span>
|<span data-ttu-id="568d2-108">成员</span><span class="sxs-lookup"><span data-stu-id="568d2-108">Member</span></span>|<span data-ttu-id="568d2-109">值</span><span class="sxs-lookup"><span data-stu-id="568d2-109">Value</span></span>|<span data-ttu-id="568d2-110">说明</span><span class="sxs-lookup"><span data-stu-id="568d2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="568d2-111">unknown</span><span class="sxs-lookup"><span data-stu-id="568d2-111">unknown</span></span>|<span data-ttu-id="568d2-112">0</span><span class="sxs-lookup"><span data-stu-id="568d2-112">0</span></span>|<span data-ttu-id="568d2-113">尚未报告设备运行状况状态</span><span class="sxs-lookup"><span data-stu-id="568d2-113">Device health state is not yet reported</span></span>|
|<span data-ttu-id="568d2-114">已</span><span class="sxs-lookup"><span data-stu-id="568d2-114">activated</span></span>|<span data-ttu-id="568d2-115">1</span><span class="sxs-lookup"><span data-stu-id="568d2-115">1</span></span>|<span data-ttu-id="568d2-116">设备已由移动威胁防护合作伙伴激活, 但尚未报告运行状况。</span><span class="sxs-lookup"><span data-stu-id="568d2-116">Device has been activated by a mobile threat defense partner, but has not yet reported health.</span></span>|
|<span data-ttu-id="568d2-117">失效</span><span class="sxs-lookup"><span data-stu-id="568d2-117">deactivated</span></span>|<span data-ttu-id="568d2-118">双面</span><span class="sxs-lookup"><span data-stu-id="568d2-118">2</span></span>|<span data-ttu-id="568d2-119">设备已被移动威胁防护合作伙伴停用。</span><span class="sxs-lookup"><span data-stu-id="568d2-119">Device has been deactivated by a mobile threat defense partner.</span></span> <span data-ttu-id="568d2-120">设备运行状况未知。</span><span class="sxs-lookup"><span data-stu-id="568d2-120">The device health is not known.</span></span>|
|<span data-ttu-id="568d2-121">加密</span><span class="sxs-lookup"><span data-stu-id="568d2-121">secured</span></span>|<span data-ttu-id="568d2-122">第三章</span><span class="sxs-lookup"><span data-stu-id="568d2-122">3</span></span>|<span data-ttu-id="568d2-123">移动威胁防护合作伙伴认为设备受安全保护。</span><span class="sxs-lookup"><span data-stu-id="568d2-123">Device is considered secured by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="568d2-124">lowSeverity</span><span class="sxs-lookup"><span data-stu-id="568d2-124">lowSeverity</span></span>|<span data-ttu-id="568d2-125">4</span><span class="sxs-lookup"><span data-stu-id="568d2-125">4</span></span>|<span data-ttu-id="568d2-126">移动威胁防护合作伙伴将设备视为低威胁。</span><span class="sxs-lookup"><span data-stu-id="568d2-126">Device is considered low threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="568d2-127">mediumSeverity</span><span class="sxs-lookup"><span data-stu-id="568d2-127">mediumSeverity</span></span>|<span data-ttu-id="568d2-128">5</span><span class="sxs-lookup"><span data-stu-id="568d2-128">5</span></span>|<span data-ttu-id="568d2-129">移动威胁防护合作伙伴认为设备是中型威胁。</span><span class="sxs-lookup"><span data-stu-id="568d2-129">Device is considered medium threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="568d2-130">highSeverity</span><span class="sxs-lookup"><span data-stu-id="568d2-130">highSeverity</span></span>|<span data-ttu-id="568d2-131">型</span><span class="sxs-lookup"><span data-stu-id="568d2-131">6</span></span>|<span data-ttu-id="568d2-132">移动威胁防护合作伙伴将设备视为高威胁。</span><span class="sxs-lookup"><span data-stu-id="568d2-132">Device is considered high threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="568d2-133">无</span><span class="sxs-lookup"><span data-stu-id="568d2-133">unresponsive</span></span>|<span data-ttu-id="568d2-134">步</span><span class="sxs-lookup"><span data-stu-id="568d2-134">7</span></span>|<span data-ttu-id="568d2-135">移动威胁防护合作伙伴认为设备无响应。</span><span class="sxs-lookup"><span data-stu-id="568d2-135">Device is considered unresponsive by the mobile threat defense partner.</span></span> <span data-ttu-id="568d2-136">设备运行状况未知。</span><span class="sxs-lookup"><span data-stu-id="568d2-136">The device health is not known.</span></span>|
|<span data-ttu-id="568d2-137">威胁</span><span class="sxs-lookup"><span data-stu-id="568d2-137">compromised</span></span>|<span data-ttu-id="568d2-138">utf-8</span><span class="sxs-lookup"><span data-stu-id="568d2-138">8</span></span>|<span data-ttu-id="568d2-139">威胁防御合作伙伴认为设备受到威胁。</span><span class="sxs-lookup"><span data-stu-id="568d2-139">Device is considered compromised by the Threat Defense partner.</span></span> <span data-ttu-id="568d2-140">这意味着该设备具有活跃的威胁或风险, 最终用户无法轻松修正该设备, 并且用户应联系其 IT 管理员。</span><span class="sxs-lookup"><span data-stu-id="568d2-140">This means the device has an active Threat or Risk which cannot be easily remediated by the end user and the user should contact their IT Admin.</span></span>|
|<span data-ttu-id="568d2-141">配置错误</span><span class="sxs-lookup"><span data-stu-id="568d2-141">misconfigured</span></span>|<span data-ttu-id="568d2-142">第</span><span class="sxs-lookup"><span data-stu-id="568d2-142">9</span></span>|<span data-ttu-id="568d2-143">将设备视为与威胁防护合作伙伴配置不正确。</span><span class="sxs-lookup"><span data-stu-id="568d2-143">Device is considered misconfigured with the Threat Defense partner.</span></span> <span data-ttu-id="568d2-144">这意味着设备缺少必需的配置文件或配置以使威胁防护合作伙伴正常运行, 因此威胁或风险分析无法完成。</span><span class="sxs-lookup"><span data-stu-id="568d2-144">This means the device is missing a required profile or configuration for the Threat Defense Partner to function properly and is thus threat or risk analysis is not able to complete.</span></span>|





