---
title: managedDevicePartnerReportedHealthState 枚举类型
description: 设备运行状况 API 的可用运行状况状态
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b99c32061bd49e05f765dbd10f6ebdb16b0d8185
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366536"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a><span data-ttu-id="959b9-103">managedDevicePartnerReportedHealthState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="959b9-103">managedDevicePartnerReportedHealthState enum type</span></span>

> <span data-ttu-id="959b9-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="959b9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="959b9-105">设备运行状况 API 的可用运行状况状态</span><span class="sxs-lookup"><span data-stu-id="959b9-105">Available health states for the Device Health API</span></span>

## <a name="members"></a><span data-ttu-id="959b9-106">成员</span><span class="sxs-lookup"><span data-stu-id="959b9-106">Members</span></span>
|<span data-ttu-id="959b9-107">成员</span><span class="sxs-lookup"><span data-stu-id="959b9-107">Member</span></span>|<span data-ttu-id="959b9-108">值</span><span class="sxs-lookup"><span data-stu-id="959b9-108">Value</span></span>|<span data-ttu-id="959b9-109">说明</span><span class="sxs-lookup"><span data-stu-id="959b9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="959b9-110">unknown</span><span class="sxs-lookup"><span data-stu-id="959b9-110">unknown</span></span>|<span data-ttu-id="959b9-111">0</span><span class="sxs-lookup"><span data-stu-id="959b9-111">0</span></span>|<span data-ttu-id="959b9-112">尚未报告设备运行状况状态</span><span class="sxs-lookup"><span data-stu-id="959b9-112">Device health state is not yet reported</span></span>|
|<span data-ttu-id="959b9-113">已</span><span class="sxs-lookup"><span data-stu-id="959b9-113">activated</span></span>|<span data-ttu-id="959b9-114">1</span><span class="sxs-lookup"><span data-stu-id="959b9-114">1</span></span>|<span data-ttu-id="959b9-115">设备已由移动威胁防护合作伙伴激活，但尚未报告运行状况。</span><span class="sxs-lookup"><span data-stu-id="959b9-115">Device has been activated by a mobile threat defense partner, but has not yet reported health.</span></span>|
|<span data-ttu-id="959b9-116">失效</span><span class="sxs-lookup"><span data-stu-id="959b9-116">deactivated</span></span>|<span data-ttu-id="959b9-117">双面</span><span class="sxs-lookup"><span data-stu-id="959b9-117">2</span></span>|<span data-ttu-id="959b9-118">设备已被移动威胁防护合作伙伴停用。</span><span class="sxs-lookup"><span data-stu-id="959b9-118">Device has been deactivated by a mobile threat defense partner.</span></span> <span data-ttu-id="959b9-119">设备运行状况未知。</span><span class="sxs-lookup"><span data-stu-id="959b9-119">The device health is not known.</span></span>|
|<span data-ttu-id="959b9-120">加密</span><span class="sxs-lookup"><span data-stu-id="959b9-120">secured</span></span>|<span data-ttu-id="959b9-121">第三章</span><span class="sxs-lookup"><span data-stu-id="959b9-121">3</span></span>|<span data-ttu-id="959b9-122">移动威胁防护合作伙伴认为设备受安全保护。</span><span class="sxs-lookup"><span data-stu-id="959b9-122">Device is considered secured by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="959b9-123">lowSeverity</span><span class="sxs-lookup"><span data-stu-id="959b9-123">lowSeverity</span></span>|<span data-ttu-id="959b9-124">4</span><span class="sxs-lookup"><span data-stu-id="959b9-124">4</span></span>|<span data-ttu-id="959b9-125">移动威胁防护合作伙伴将设备视为低威胁。</span><span class="sxs-lookup"><span data-stu-id="959b9-125">Device is considered low threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="959b9-126">mediumSeverity</span><span class="sxs-lookup"><span data-stu-id="959b9-126">mediumSeverity</span></span>|<span data-ttu-id="959b9-127">5</span><span class="sxs-lookup"><span data-stu-id="959b9-127">5</span></span>|<span data-ttu-id="959b9-128">移动威胁防护合作伙伴认为设备是中型威胁。</span><span class="sxs-lookup"><span data-stu-id="959b9-128">Device is considered medium threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="959b9-129">highSeverity</span><span class="sxs-lookup"><span data-stu-id="959b9-129">highSeverity</span></span>|<span data-ttu-id="959b9-130">型</span><span class="sxs-lookup"><span data-stu-id="959b9-130">6</span></span>|<span data-ttu-id="959b9-131">移动威胁防护合作伙伴将设备视为高威胁。</span><span class="sxs-lookup"><span data-stu-id="959b9-131">Device is considered high threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="959b9-132">无</span><span class="sxs-lookup"><span data-stu-id="959b9-132">unresponsive</span></span>|<span data-ttu-id="959b9-133">步</span><span class="sxs-lookup"><span data-stu-id="959b9-133">7</span></span>|<span data-ttu-id="959b9-134">移动威胁防护合作伙伴认为设备无响应。</span><span class="sxs-lookup"><span data-stu-id="959b9-134">Device is considered unresponsive by the mobile threat defense partner.</span></span> <span data-ttu-id="959b9-135">设备运行状况未知。</span><span class="sxs-lookup"><span data-stu-id="959b9-135">The device health is not known.</span></span>|
|<span data-ttu-id="959b9-136">威胁</span><span class="sxs-lookup"><span data-stu-id="959b9-136">compromised</span></span>|<span data-ttu-id="959b9-137">utf-8</span><span class="sxs-lookup"><span data-stu-id="959b9-137">8</span></span>|<span data-ttu-id="959b9-138">威胁防御合作伙伴认为设备受到威胁。</span><span class="sxs-lookup"><span data-stu-id="959b9-138">Device is considered compromised by the Threat Defense partner.</span></span> <span data-ttu-id="959b9-139">这意味着该设备具有活跃的威胁或风险，最终用户无法轻松修正该设备，并且用户应联系其 IT 管理员。</span><span class="sxs-lookup"><span data-stu-id="959b9-139">This means the device has an active Threat or Risk which cannot be easily remediated by the end user and the user should contact their IT Admin.</span></span>|
|<span data-ttu-id="959b9-140">配置错误</span><span class="sxs-lookup"><span data-stu-id="959b9-140">misconfigured</span></span>|<span data-ttu-id="959b9-141">第</span><span class="sxs-lookup"><span data-stu-id="959b9-141">9</span></span>|<span data-ttu-id="959b9-142">将设备视为与威胁防护合作伙伴配置不正确。</span><span class="sxs-lookup"><span data-stu-id="959b9-142">Device is considered misconfigured with the Threat Defense partner.</span></span> <span data-ttu-id="959b9-143">这意味着设备缺少必需的配置文件或配置以使威胁防护合作伙伴正常运行，因此威胁或风险分析无法完成。</span><span class="sxs-lookup"><span data-stu-id="959b9-143">This means the device is missing a required profile or configuration for the Threat Defense Partner to function properly and is thus threat or risk analysis is not able to complete.</span></span>|




