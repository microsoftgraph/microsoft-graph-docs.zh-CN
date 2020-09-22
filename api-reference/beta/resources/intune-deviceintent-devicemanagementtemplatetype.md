---
title: deviceManagementTemplateType 枚举类型
description: 模板类型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 09fdc3b7d099646dc36e6b398657962b638a7ab8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061019"
---
# <a name="devicemanagementtemplatetype-enum-type"></a><span data-ttu-id="4ca8b-103">deviceManagementTemplateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4ca8b-103">deviceManagementTemplateType enum type</span></span>

<span data-ttu-id="4ca8b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ca8b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ca8b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4ca8b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ca8b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4ca8b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ca8b-107">模板类型</span><span class="sxs-lookup"><span data-stu-id="4ca8b-107">Template type</span></span>

## <a name="members"></a><span data-ttu-id="4ca8b-108">成员</span><span class="sxs-lookup"><span data-stu-id="4ca8b-108">Members</span></span>
|<span data-ttu-id="4ca8b-109">成员</span><span class="sxs-lookup"><span data-stu-id="4ca8b-109">Member</span></span>|<span data-ttu-id="4ca8b-110">值</span><span class="sxs-lookup"><span data-stu-id="4ca8b-110">Value</span></span>|<span data-ttu-id="4ca8b-111">说明</span><span class="sxs-lookup"><span data-stu-id="4ca8b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ca8b-112">securityBaseline</span><span class="sxs-lookup"><span data-stu-id="4ca8b-112">securityBaseline</span></span>|<span data-ttu-id="4ca8b-113">0</span><span class="sxs-lookup"><span data-stu-id="4ca8b-113">0</span></span>|<span data-ttu-id="4ca8b-114">安全基准模板</span><span class="sxs-lookup"><span data-stu-id="4ca8b-114">Security baseline template</span></span>|
|<span data-ttu-id="4ca8b-115">specializedDevices</span><span class="sxs-lookup"><span data-stu-id="4ca8b-115">specializedDevices</span></span>|<span data-ttu-id="4ca8b-116">1 </span><span class="sxs-lookup"><span data-stu-id="4ca8b-116">1</span></span>|<span data-ttu-id="4ca8b-117">专用设备模板</span><span class="sxs-lookup"><span data-stu-id="4ca8b-117">Specialized devices template</span></span>|
|<span data-ttu-id="4ca8b-118">advancedThreatProtectionSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="4ca8b-118">advancedThreatProtectionSecurityBaseline</span></span>|<span data-ttu-id="4ca8b-119">2 </span><span class="sxs-lookup"><span data-stu-id="4ca8b-119">2</span></span>|<span data-ttu-id="4ca8b-120">高级威胁防护安全基准模板</span><span class="sxs-lookup"><span data-stu-id="4ca8b-120">Advanced Threat Protection security baseline template</span></span>|
|<span data-ttu-id="4ca8b-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ca8b-121">deviceConfiguration</span></span>|<span data-ttu-id="4ca8b-122">第三章</span><span class="sxs-lookup"><span data-stu-id="4ca8b-122">3</span></span>|<span data-ttu-id="4ca8b-123">设备配置模板</span><span class="sxs-lookup"><span data-stu-id="4ca8b-123">Device configuration template</span></span>|
|<span data-ttu-id="4ca8b-124">自</span><span class="sxs-lookup"><span data-stu-id="4ca8b-124">custom</span></span>|<span data-ttu-id="4ca8b-125">4 </span><span class="sxs-lookup"><span data-stu-id="4ca8b-125">4</span></span>|<span data-ttu-id="4ca8b-126">自定义管理员定义的模板</span><span class="sxs-lookup"><span data-stu-id="4ca8b-126">Custom admin defined template</span></span>|
|<span data-ttu-id="4ca8b-127">securityTemplate</span><span class="sxs-lookup"><span data-stu-id="4ca8b-127">securityTemplate</span></span>|<span data-ttu-id="4ca8b-128">5 </span><span class="sxs-lookup"><span data-stu-id="4ca8b-128">5</span></span>|<span data-ttu-id="4ca8b-129">包含特定的安全重点设置的模板</span><span class="sxs-lookup"><span data-stu-id="4ca8b-129">Templates containing specific security focused settings</span></span>|
|<span data-ttu-id="4ca8b-130">microsoftEdgeSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="4ca8b-130">microsoftEdgeSecurityBaseline</span></span>|<span data-ttu-id="4ca8b-131">6 </span><span class="sxs-lookup"><span data-stu-id="4ca8b-131">6</span></span>|<span data-ttu-id="4ca8b-132">Microsoft Edge 安全基准模板</span><span class="sxs-lookup"><span data-stu-id="4ca8b-132">Microsoft Edge security baseline template</span></span>|
|<span data-ttu-id="4ca8b-133">microsoftOffice365ProPlusSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="4ca8b-133">microsoftOffice365ProPlusSecurityBaseline</span></span>|<span data-ttu-id="4ca8b-134">7 </span><span class="sxs-lookup"><span data-stu-id="4ca8b-134">7</span></span>|<span data-ttu-id="4ca8b-135">Microsoft Office 365 专业增强版安全基准模板</span><span class="sxs-lookup"><span data-stu-id="4ca8b-135">Microsoft Office 365 ProPlus security baseline template</span></span>|
|<span data-ttu-id="4ca8b-136">deviceCompliance</span><span class="sxs-lookup"><span data-stu-id="4ca8b-136">deviceCompliance</span></span>|<span data-ttu-id="4ca8b-137">8 </span><span class="sxs-lookup"><span data-stu-id="4ca8b-137">8</span></span>|<span data-ttu-id="4ca8b-138">设备合规性模板</span><span class="sxs-lookup"><span data-stu-id="4ca8b-138">Device compliance template</span></span>|
|<span data-ttu-id="4ca8b-139">deviceConfigurationForOffice365</span><span class="sxs-lookup"><span data-stu-id="4ca8b-139">deviceConfigurationForOffice365</span></span>|<span data-ttu-id="4ca8b-140">9 </span><span class="sxs-lookup"><span data-stu-id="4ca8b-140">9</span></span>|<span data-ttu-id="4ca8b-141">Microsoft Office 365 设置的设备配置</span><span class="sxs-lookup"><span data-stu-id="4ca8b-141">Device Configuration for Microsoft Office 365 settings</span></span>|
|<span data-ttu-id="4ca8b-142">cloudPC</span><span class="sxs-lookup"><span data-stu-id="4ca8b-142">cloudPC</span></span>|<span data-ttu-id="4ca8b-143">10 </span><span class="sxs-lookup"><span data-stu-id="4ca8b-143">10</span></span>|<span data-ttu-id="4ca8b-144">云电脑安全基准模板</span><span class="sxs-lookup"><span data-stu-id="4ca8b-144">Cloud PC security baseline template</span></span>|






