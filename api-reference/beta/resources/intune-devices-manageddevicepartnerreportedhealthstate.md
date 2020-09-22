---
title: managedDevicePartnerReportedHealthState 枚举类型
description: 设备运行状况 API 的可用运行状况状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ec4ea50b41ee9e5f9788b512c903d4e92502aeb5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081151"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a><span data-ttu-id="1a9ae-103">managedDevicePartnerReportedHealthState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1a9ae-103">managedDevicePartnerReportedHealthState enum type</span></span>

<span data-ttu-id="1a9ae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a9ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a9ae-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1a9ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a9ae-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a9ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a9ae-107">设备运行状况 API 的可用运行状况状态</span><span class="sxs-lookup"><span data-stu-id="1a9ae-107">Available health states for the Device Health API</span></span>

## <a name="members"></a><span data-ttu-id="1a9ae-108">成员</span><span class="sxs-lookup"><span data-stu-id="1a9ae-108">Members</span></span>
|<span data-ttu-id="1a9ae-109">成员</span><span class="sxs-lookup"><span data-stu-id="1a9ae-109">Member</span></span>|<span data-ttu-id="1a9ae-110">值</span><span class="sxs-lookup"><span data-stu-id="1a9ae-110">Value</span></span>|<span data-ttu-id="1a9ae-111">说明</span><span class="sxs-lookup"><span data-stu-id="1a9ae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a9ae-112">unknown</span><span class="sxs-lookup"><span data-stu-id="1a9ae-112">unknown</span></span>|<span data-ttu-id="1a9ae-113">0</span><span class="sxs-lookup"><span data-stu-id="1a9ae-113">0</span></span>|<span data-ttu-id="1a9ae-114">尚未报告设备运行状况状态</span><span class="sxs-lookup"><span data-stu-id="1a9ae-114">Device health state is not yet reported</span></span>|
|<span data-ttu-id="1a9ae-115">已</span><span class="sxs-lookup"><span data-stu-id="1a9ae-115">activated</span></span>|<span data-ttu-id="1a9ae-116">1 </span><span class="sxs-lookup"><span data-stu-id="1a9ae-116">1</span></span>|<span data-ttu-id="1a9ae-117">设备已由移动威胁防护合作伙伴激活，但尚未报告运行状况。</span><span class="sxs-lookup"><span data-stu-id="1a9ae-117">Device has been activated by a mobile threat defense partner, but has not yet reported health.</span></span>|
|<span data-ttu-id="1a9ae-118">失效</span><span class="sxs-lookup"><span data-stu-id="1a9ae-118">deactivated</span></span>|<span data-ttu-id="1a9ae-119">2 </span><span class="sxs-lookup"><span data-stu-id="1a9ae-119">2</span></span>|<span data-ttu-id="1a9ae-120">设备已被移动威胁防护合作伙伴停用。</span><span class="sxs-lookup"><span data-stu-id="1a9ae-120">Device has been deactivated by a mobile threat defense partner.</span></span> <span data-ttu-id="1a9ae-121">设备运行状况未知。</span><span class="sxs-lookup"><span data-stu-id="1a9ae-121">The device health is not known.</span></span>|
|<span data-ttu-id="1a9ae-122">加密</span><span class="sxs-lookup"><span data-stu-id="1a9ae-122">secured</span></span>|<span data-ttu-id="1a9ae-123">第三章</span><span class="sxs-lookup"><span data-stu-id="1a9ae-123">3</span></span>|<span data-ttu-id="1a9ae-124">移动威胁防护合作伙伴认为设备受安全保护。</span><span class="sxs-lookup"><span data-stu-id="1a9ae-124">Device is considered secured by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="1a9ae-125">lowSeverity</span><span class="sxs-lookup"><span data-stu-id="1a9ae-125">lowSeverity</span></span>|<span data-ttu-id="1a9ae-126">4 </span><span class="sxs-lookup"><span data-stu-id="1a9ae-126">4</span></span>|<span data-ttu-id="1a9ae-127">移动威胁防护合作伙伴将设备视为低威胁。</span><span class="sxs-lookup"><span data-stu-id="1a9ae-127">Device is considered low threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="1a9ae-128">mediumSeverity</span><span class="sxs-lookup"><span data-stu-id="1a9ae-128">mediumSeverity</span></span>|<span data-ttu-id="1a9ae-129">5 </span><span class="sxs-lookup"><span data-stu-id="1a9ae-129">5</span></span>|<span data-ttu-id="1a9ae-130">移动威胁防护合作伙伴认为设备是中型威胁。</span><span class="sxs-lookup"><span data-stu-id="1a9ae-130">Device is considered medium threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="1a9ae-131">highSeverity</span><span class="sxs-lookup"><span data-stu-id="1a9ae-131">highSeverity</span></span>|<span data-ttu-id="1a9ae-132">6 </span><span class="sxs-lookup"><span data-stu-id="1a9ae-132">6</span></span>|<span data-ttu-id="1a9ae-133">移动威胁防护合作伙伴将设备视为高威胁。</span><span class="sxs-lookup"><span data-stu-id="1a9ae-133">Device is considered high threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="1a9ae-134">无</span><span class="sxs-lookup"><span data-stu-id="1a9ae-134">unresponsive</span></span>|<span data-ttu-id="1a9ae-135">7 </span><span class="sxs-lookup"><span data-stu-id="1a9ae-135">7</span></span>|<span data-ttu-id="1a9ae-136">移动威胁防护合作伙伴认为设备无响应。</span><span class="sxs-lookup"><span data-stu-id="1a9ae-136">Device is considered unresponsive by the mobile threat defense partner.</span></span> <span data-ttu-id="1a9ae-137">设备运行状况未知。</span><span class="sxs-lookup"><span data-stu-id="1a9ae-137">The device health is not known.</span></span>|
|<span data-ttu-id="1a9ae-138">威胁</span><span class="sxs-lookup"><span data-stu-id="1a9ae-138">compromised</span></span>|<span data-ttu-id="1a9ae-139">8 </span><span class="sxs-lookup"><span data-stu-id="1a9ae-139">8</span></span>|<span data-ttu-id="1a9ae-140">威胁防御合作伙伴认为设备受到威胁。</span><span class="sxs-lookup"><span data-stu-id="1a9ae-140">Device is considered compromised by the Threat Defense partner.</span></span> <span data-ttu-id="1a9ae-141">这意味着该设备具有活跃的威胁或风险，最终用户无法轻松修正该设备，并且用户应联系其 IT 管理员。</span><span class="sxs-lookup"><span data-stu-id="1a9ae-141">This means the device has an active Threat or Risk which cannot be easily remediated by the end user and the user should contact their IT Admin.</span></span>|
|<span data-ttu-id="1a9ae-142">配置错误</span><span class="sxs-lookup"><span data-stu-id="1a9ae-142">misconfigured</span></span>|<span data-ttu-id="1a9ae-143">9 </span><span class="sxs-lookup"><span data-stu-id="1a9ae-143">9</span></span>|<span data-ttu-id="1a9ae-144">将设备视为与威胁防护合作伙伴配置不正确。</span><span class="sxs-lookup"><span data-stu-id="1a9ae-144">Device is considered misconfigured with the Threat Defense partner.</span></span> <span data-ttu-id="1a9ae-145">这意味着设备缺少必需的配置文件或配置以使威胁防护合作伙伴正常运行，因此威胁或风险分析无法完成。</span><span class="sxs-lookup"><span data-stu-id="1a9ae-145">This means the device is missing a required profile or configuration for the Threat Defense Partner to function properly and is thus threat or risk analysis is not able to complete.</span></span>|






