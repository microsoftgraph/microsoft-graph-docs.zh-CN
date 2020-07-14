---
title: deviceManagementTemplateType 枚举类型
description: 模板类型
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1dd3a03efe602b8b9baeedcd622f6a012ca6ef3c
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124035"
---
# <a name="devicemanagementtemplatetype-enum-type"></a><span data-ttu-id="698a4-103">deviceManagementTemplateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="698a4-103">deviceManagementTemplateType enum type</span></span>

<span data-ttu-id="698a4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="698a4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="698a4-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="698a4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="698a4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="698a4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="698a4-107">模板类型</span><span class="sxs-lookup"><span data-stu-id="698a4-107">Template type</span></span>

## <a name="members"></a><span data-ttu-id="698a4-108">成员</span><span class="sxs-lookup"><span data-stu-id="698a4-108">Members</span></span>
|<span data-ttu-id="698a4-109">成员</span><span class="sxs-lookup"><span data-stu-id="698a4-109">Member</span></span>|<span data-ttu-id="698a4-110">值</span><span class="sxs-lookup"><span data-stu-id="698a4-110">Value</span></span>|<span data-ttu-id="698a4-111">说明</span><span class="sxs-lookup"><span data-stu-id="698a4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="698a4-112">securityBaseline</span><span class="sxs-lookup"><span data-stu-id="698a4-112">securityBaseline</span></span>|<span data-ttu-id="698a4-113">0</span><span class="sxs-lookup"><span data-stu-id="698a4-113">0</span></span>|<span data-ttu-id="698a4-114">安全基准模板</span><span class="sxs-lookup"><span data-stu-id="698a4-114">Security baseline template</span></span>|
|<span data-ttu-id="698a4-115">specializedDevices</span><span class="sxs-lookup"><span data-stu-id="698a4-115">specializedDevices</span></span>|<span data-ttu-id="698a4-116">1 </span><span class="sxs-lookup"><span data-stu-id="698a4-116">1</span></span>|<span data-ttu-id="698a4-117">专用设备模板</span><span class="sxs-lookup"><span data-stu-id="698a4-117">Specialized devices template</span></span>|
|<span data-ttu-id="698a4-118">advancedThreatProtectionSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="698a4-118">advancedThreatProtectionSecurityBaseline</span></span>|<span data-ttu-id="698a4-119">2 </span><span class="sxs-lookup"><span data-stu-id="698a4-119">2</span></span>|<span data-ttu-id="698a4-120">高级威胁防护安全基准模板</span><span class="sxs-lookup"><span data-stu-id="698a4-120">Advanced Threat Protection security baseline template</span></span>|
|<span data-ttu-id="698a4-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="698a4-121">deviceConfiguration</span></span>|<span data-ttu-id="698a4-122">3 </span><span class="sxs-lookup"><span data-stu-id="698a4-122">3</span></span>|<span data-ttu-id="698a4-123">设备配置模板</span><span class="sxs-lookup"><span data-stu-id="698a4-123">Device configuration template</span></span>|
|<span data-ttu-id="698a4-124">自</span><span class="sxs-lookup"><span data-stu-id="698a4-124">custom</span></span>|<span data-ttu-id="698a4-125">4 </span><span class="sxs-lookup"><span data-stu-id="698a4-125">4</span></span>|<span data-ttu-id="698a4-126">自定义管理员定义的模板</span><span class="sxs-lookup"><span data-stu-id="698a4-126">Custom admin defined template</span></span>|
|<span data-ttu-id="698a4-127">securityTemplate</span><span class="sxs-lookup"><span data-stu-id="698a4-127">securityTemplate</span></span>|<span data-ttu-id="698a4-128">5 </span><span class="sxs-lookup"><span data-stu-id="698a4-128">5</span></span>|<span data-ttu-id="698a4-129">包含特定的安全重点设置的模板</span><span class="sxs-lookup"><span data-stu-id="698a4-129">Templates containing specific security focused settings</span></span>|
|<span data-ttu-id="698a4-130">microsoftEdgeSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="698a4-130">microsoftEdgeSecurityBaseline</span></span>|<span data-ttu-id="698a4-131">6 </span><span class="sxs-lookup"><span data-stu-id="698a4-131">6</span></span>|<span data-ttu-id="698a4-132">Microsoft Edge 安全基准模板</span><span class="sxs-lookup"><span data-stu-id="698a4-132">Microsoft Edge security baseline template</span></span>|
|<span data-ttu-id="698a4-133">microsoftOffice365ProPlusSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="698a4-133">microsoftOffice365ProPlusSecurityBaseline</span></span>|<span data-ttu-id="698a4-134">7 </span><span class="sxs-lookup"><span data-stu-id="698a4-134">7</span></span>|<span data-ttu-id="698a4-135">Microsoft Office 365 专业增强版安全基准模板</span><span class="sxs-lookup"><span data-stu-id="698a4-135">Microsoft Office 365 ProPlus security baseline template</span></span>|
|<span data-ttu-id="698a4-136">deviceCompliance</span><span class="sxs-lookup"><span data-stu-id="698a4-136">deviceCompliance</span></span>|<span data-ttu-id="698a4-137">8 </span><span class="sxs-lookup"><span data-stu-id="698a4-137">8</span></span>|<span data-ttu-id="698a4-138">设备合规性模板</span><span class="sxs-lookup"><span data-stu-id="698a4-138">Device compliance template</span></span>|
|<span data-ttu-id="698a4-139">deviceConfigurationForOffice365</span><span class="sxs-lookup"><span data-stu-id="698a4-139">deviceConfigurationForOffice365</span></span>|<span data-ttu-id="698a4-140">9 </span><span class="sxs-lookup"><span data-stu-id="698a4-140">9</span></span>|<span data-ttu-id="698a4-141">Microsoft Office 365 设置的设备配置</span><span class="sxs-lookup"><span data-stu-id="698a4-141">Device Configuration for Microsoft Office 365 settings</span></span>|



