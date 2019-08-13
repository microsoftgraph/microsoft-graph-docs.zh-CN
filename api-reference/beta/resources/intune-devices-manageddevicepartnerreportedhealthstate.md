---
title: managedDevicePartnerReportedHealthState 枚举类型
description: 设备运行状况 API 的可用运行状况状态
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2e9565d1d5dcf08cccfb141cd9947a20805882bf
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372186"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a><span data-ttu-id="38df9-103">managedDevicePartnerReportedHealthState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="38df9-103">managedDevicePartnerReportedHealthState enum type</span></span>

> <span data-ttu-id="38df9-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="38df9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38df9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="38df9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38df9-106">设备运行状况 API 的可用运行状况状态</span><span class="sxs-lookup"><span data-stu-id="38df9-106">Available health states for the Device Health API</span></span>

## <a name="members"></a><span data-ttu-id="38df9-107">成员</span><span class="sxs-lookup"><span data-stu-id="38df9-107">Members</span></span>
|<span data-ttu-id="38df9-108">成员</span><span class="sxs-lookup"><span data-stu-id="38df9-108">Member</span></span>|<span data-ttu-id="38df9-109">值</span><span class="sxs-lookup"><span data-stu-id="38df9-109">Value</span></span>|<span data-ttu-id="38df9-110">说明</span><span class="sxs-lookup"><span data-stu-id="38df9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38df9-111">unknown</span><span class="sxs-lookup"><span data-stu-id="38df9-111">unknown</span></span>|<span data-ttu-id="38df9-112">0</span><span class="sxs-lookup"><span data-stu-id="38df9-112">0</span></span>|<span data-ttu-id="38df9-113">尚未报告设备运行状况状态</span><span class="sxs-lookup"><span data-stu-id="38df9-113">Device health state is not yet reported</span></span>|
|<span data-ttu-id="38df9-114">已</span><span class="sxs-lookup"><span data-stu-id="38df9-114">activated</span></span>|<span data-ttu-id="38df9-115">1</span><span class="sxs-lookup"><span data-stu-id="38df9-115">1</span></span>|<span data-ttu-id="38df9-116">设备已由移动威胁防护合作伙伴激活, 但尚未报告运行状况。</span><span class="sxs-lookup"><span data-stu-id="38df9-116">Device has been activated by a mobile threat defense partner, but has not yet reported health.</span></span>|
|<span data-ttu-id="38df9-117">失效</span><span class="sxs-lookup"><span data-stu-id="38df9-117">deactivated</span></span>|<span data-ttu-id="38df9-118">双面</span><span class="sxs-lookup"><span data-stu-id="38df9-118">2</span></span>|<span data-ttu-id="38df9-119">设备已被移动威胁防护合作伙伴停用。</span><span class="sxs-lookup"><span data-stu-id="38df9-119">Device has been deactivated by a mobile threat defense partner.</span></span> <span data-ttu-id="38df9-120">设备运行状况未知。</span><span class="sxs-lookup"><span data-stu-id="38df9-120">The device health is not known.</span></span>|
|<span data-ttu-id="38df9-121">加密</span><span class="sxs-lookup"><span data-stu-id="38df9-121">secured</span></span>|<span data-ttu-id="38df9-122">第三章</span><span class="sxs-lookup"><span data-stu-id="38df9-122">3</span></span>|<span data-ttu-id="38df9-123">移动威胁防护合作伙伴认为设备受安全保护。</span><span class="sxs-lookup"><span data-stu-id="38df9-123">Device is considered secured by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="38df9-124">lowSeverity</span><span class="sxs-lookup"><span data-stu-id="38df9-124">lowSeverity</span></span>|<span data-ttu-id="38df9-125">4</span><span class="sxs-lookup"><span data-stu-id="38df9-125">4</span></span>|<span data-ttu-id="38df9-126">移动威胁防护合作伙伴将设备视为低威胁。</span><span class="sxs-lookup"><span data-stu-id="38df9-126">Device is considered low threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="38df9-127">mediumSeverity</span><span class="sxs-lookup"><span data-stu-id="38df9-127">mediumSeverity</span></span>|<span data-ttu-id="38df9-128">5</span><span class="sxs-lookup"><span data-stu-id="38df9-128">5</span></span>|<span data-ttu-id="38df9-129">移动威胁防护合作伙伴认为设备是中型威胁。</span><span class="sxs-lookup"><span data-stu-id="38df9-129">Device is considered medium threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="38df9-130">highSeverity</span><span class="sxs-lookup"><span data-stu-id="38df9-130">highSeverity</span></span>|<span data-ttu-id="38df9-131">型</span><span class="sxs-lookup"><span data-stu-id="38df9-131">6</span></span>|<span data-ttu-id="38df9-132">移动威胁防护合作伙伴将设备视为高威胁。</span><span class="sxs-lookup"><span data-stu-id="38df9-132">Device is considered high threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="38df9-133">无</span><span class="sxs-lookup"><span data-stu-id="38df9-133">unresponsive</span></span>|<span data-ttu-id="38df9-134">步</span><span class="sxs-lookup"><span data-stu-id="38df9-134">7</span></span>|<span data-ttu-id="38df9-135">移动威胁防护合作伙伴认为设备无响应。</span><span class="sxs-lookup"><span data-stu-id="38df9-135">Device is considered unresponsive by the mobile threat defense partner.</span></span> <span data-ttu-id="38df9-136">设备运行状况未知。</span><span class="sxs-lookup"><span data-stu-id="38df9-136">The device health is not known.</span></span>|
|<span data-ttu-id="38df9-137">威胁</span><span class="sxs-lookup"><span data-stu-id="38df9-137">compromised</span></span>|<span data-ttu-id="38df9-138">utf-8</span><span class="sxs-lookup"><span data-stu-id="38df9-138">8</span></span>|<span data-ttu-id="38df9-139">威胁防御合作伙伴认为设备受到威胁。</span><span class="sxs-lookup"><span data-stu-id="38df9-139">Device is considered compromised by the Threat Defense partner.</span></span> <span data-ttu-id="38df9-140">这意味着该设备具有活跃的威胁或风险, 最终用户无法轻松修正该设备, 并且用户应联系其 IT 管理员。</span><span class="sxs-lookup"><span data-stu-id="38df9-140">This means the device has an active Threat or Risk which cannot be easily remediated by the end user and the user should contact their IT Admin.</span></span>|
|<span data-ttu-id="38df9-141">配置错误</span><span class="sxs-lookup"><span data-stu-id="38df9-141">misconfigured</span></span>|<span data-ttu-id="38df9-142">第</span><span class="sxs-lookup"><span data-stu-id="38df9-142">9</span></span>|<span data-ttu-id="38df9-143">将设备视为与威胁防护合作伙伴配置不正确。</span><span class="sxs-lookup"><span data-stu-id="38df9-143">Device is considered misconfigured with the Threat Defense partner.</span></span> <span data-ttu-id="38df9-144">这意味着设备缺少必需的配置文件或配置以使威胁防护合作伙伴正常运行, 因此威胁或风险分析无法完成。</span><span class="sxs-lookup"><span data-stu-id="38df9-144">This means the device is missing a required profile or configuration for the Threat Defense Partner to function properly and is thus threat or risk analysis is not able to complete.</span></span>|



