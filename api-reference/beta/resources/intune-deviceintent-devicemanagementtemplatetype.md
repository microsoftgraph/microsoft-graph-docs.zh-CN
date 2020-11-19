---
title: deviceManagementTemplateType 枚举类型
description: 模板类型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 29cda57dbbc1652dc4cc004e973871f283476571
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49209435"
---
# <a name="devicemanagementtemplatetype-enum-type"></a><span data-ttu-id="3370d-103">deviceManagementTemplateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3370d-103">deviceManagementTemplateType enum type</span></span>

<span data-ttu-id="3370d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3370d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3370d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3370d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3370d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3370d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3370d-107">模板类型</span><span class="sxs-lookup"><span data-stu-id="3370d-107">Template type</span></span>

## <a name="members"></a><span data-ttu-id="3370d-108">成员</span><span class="sxs-lookup"><span data-stu-id="3370d-108">Members</span></span>
|<span data-ttu-id="3370d-109">成员</span><span class="sxs-lookup"><span data-stu-id="3370d-109">Member</span></span>|<span data-ttu-id="3370d-110">值</span><span class="sxs-lookup"><span data-stu-id="3370d-110">Value</span></span>|<span data-ttu-id="3370d-111">说明</span><span class="sxs-lookup"><span data-stu-id="3370d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3370d-112">securityBaseline</span><span class="sxs-lookup"><span data-stu-id="3370d-112">securityBaseline</span></span>|<span data-ttu-id="3370d-113">0</span><span class="sxs-lookup"><span data-stu-id="3370d-113">0</span></span>|<span data-ttu-id="3370d-114">安全基准模板</span><span class="sxs-lookup"><span data-stu-id="3370d-114">Security baseline template</span></span>|
|<span data-ttu-id="3370d-115">specializedDevices</span><span class="sxs-lookup"><span data-stu-id="3370d-115">specializedDevices</span></span>|<span data-ttu-id="3370d-116">1</span><span class="sxs-lookup"><span data-stu-id="3370d-116">1</span></span>|<span data-ttu-id="3370d-117">专用设备模板</span><span class="sxs-lookup"><span data-stu-id="3370d-117">Specialized devices template</span></span>|
|<span data-ttu-id="3370d-118">advancedThreatProtectionSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="3370d-118">advancedThreatProtectionSecurityBaseline</span></span>|<span data-ttu-id="3370d-119">双面</span><span class="sxs-lookup"><span data-stu-id="3370d-119">2</span></span>|<span data-ttu-id="3370d-120">高级威胁防护安全基准模板</span><span class="sxs-lookup"><span data-stu-id="3370d-120">Advanced Threat Protection security baseline template</span></span>|
|<span data-ttu-id="3370d-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3370d-121">deviceConfiguration</span></span>|<span data-ttu-id="3370d-122">第三章</span><span class="sxs-lookup"><span data-stu-id="3370d-122">3</span></span>|<span data-ttu-id="3370d-123">设备配置模板</span><span class="sxs-lookup"><span data-stu-id="3370d-123">Device configuration template</span></span>|
|<span data-ttu-id="3370d-124">自</span><span class="sxs-lookup"><span data-stu-id="3370d-124">custom</span></span>|<span data-ttu-id="3370d-125">4 </span><span class="sxs-lookup"><span data-stu-id="3370d-125">4</span></span>|<span data-ttu-id="3370d-126">自定义管理员定义的模板</span><span class="sxs-lookup"><span data-stu-id="3370d-126">Custom admin defined template</span></span>|
|<span data-ttu-id="3370d-127">securityTemplate</span><span class="sxs-lookup"><span data-stu-id="3370d-127">securityTemplate</span></span>|<span data-ttu-id="3370d-128">5 </span><span class="sxs-lookup"><span data-stu-id="3370d-128">5</span></span>|<span data-ttu-id="3370d-129">包含特定的安全重点设置的模板</span><span class="sxs-lookup"><span data-stu-id="3370d-129">Templates containing specific security focused settings</span></span>|
|<span data-ttu-id="3370d-130">microsoftEdgeSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="3370d-130">microsoftEdgeSecurityBaseline</span></span>|<span data-ttu-id="3370d-131">6 </span><span class="sxs-lookup"><span data-stu-id="3370d-131">6</span></span>|<span data-ttu-id="3370d-132">Microsoft Edge 安全基准模板</span><span class="sxs-lookup"><span data-stu-id="3370d-132">Microsoft Edge security baseline template</span></span>|
|<span data-ttu-id="3370d-133">microsoftOffice365ProPlusSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="3370d-133">microsoftOffice365ProPlusSecurityBaseline</span></span>|<span data-ttu-id="3370d-134">7 </span><span class="sxs-lookup"><span data-stu-id="3370d-134">7</span></span>|<span data-ttu-id="3370d-135">Microsoft Office 365 专业增强版安全基准模板</span><span class="sxs-lookup"><span data-stu-id="3370d-135">Microsoft Office 365 ProPlus security baseline template</span></span>|
|<span data-ttu-id="3370d-136">deviceCompliance</span><span class="sxs-lookup"><span data-stu-id="3370d-136">deviceCompliance</span></span>|<span data-ttu-id="3370d-137">8 </span><span class="sxs-lookup"><span data-stu-id="3370d-137">8</span></span>|<span data-ttu-id="3370d-138">设备合规性模板</span><span class="sxs-lookup"><span data-stu-id="3370d-138">Device compliance template</span></span>|
|<span data-ttu-id="3370d-139">deviceConfigurationForOffice365</span><span class="sxs-lookup"><span data-stu-id="3370d-139">deviceConfigurationForOffice365</span></span>|<span data-ttu-id="3370d-140">9 </span><span class="sxs-lookup"><span data-stu-id="3370d-140">9</span></span>|<span data-ttu-id="3370d-141">Microsoft Office 365 设置的设备配置</span><span class="sxs-lookup"><span data-stu-id="3370d-141">Device Configuration for Microsoft Office 365 settings</span></span>|
|<span data-ttu-id="3370d-142">cloudPC</span><span class="sxs-lookup"><span data-stu-id="3370d-142">cloudPC</span></span>|<span data-ttu-id="3370d-143">10  </span><span class="sxs-lookup"><span data-stu-id="3370d-143">10</span></span>|<span data-ttu-id="3370d-144">云电脑安全基准模板</span><span class="sxs-lookup"><span data-stu-id="3370d-144">Cloud PC security baseline template</span></span>|
|<span data-ttu-id="3370d-145">firewallSharedSettings</span><span class="sxs-lookup"><span data-stu-id="3370d-145">firewallSharedSettings</span></span>|<span data-ttu-id="3370d-146">11 </span><span class="sxs-lookup"><span data-stu-id="3370d-146">11</span></span>|<span data-ttu-id="3370d-147">用于参考设置的防火墙共享对象模板</span><span class="sxs-lookup"><span data-stu-id="3370d-147">Firewall Shared Object templates for reference settings</span></span>|




