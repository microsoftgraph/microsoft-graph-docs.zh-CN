---
title: deviceManagementTemplateType 枚举类型
description: 模板类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 93541ab234b1733ca08d5a3da1c5a3dd39819f62
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636628"
---
# <a name="devicemanagementtemplatetype-enum-type"></a><span data-ttu-id="e57df-103">deviceManagementTemplateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e57df-103">deviceManagementTemplateType enum type</span></span>

> <span data-ttu-id="e57df-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e57df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e57df-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e57df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e57df-106">模板类型</span><span class="sxs-lookup"><span data-stu-id="e57df-106">Template type</span></span>

## <a name="members"></a><span data-ttu-id="e57df-107">成员</span><span class="sxs-lookup"><span data-stu-id="e57df-107">Members</span></span>
|<span data-ttu-id="e57df-108">成员</span><span class="sxs-lookup"><span data-stu-id="e57df-108">Member</span></span>|<span data-ttu-id="e57df-109">值</span><span class="sxs-lookup"><span data-stu-id="e57df-109">Value</span></span>|<span data-ttu-id="e57df-110">Description</span><span class="sxs-lookup"><span data-stu-id="e57df-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e57df-111">securityBaseline</span><span class="sxs-lookup"><span data-stu-id="e57df-111">securityBaseline</span></span>|<span data-ttu-id="e57df-112">0</span><span class="sxs-lookup"><span data-stu-id="e57df-112">0</span></span>|<span data-ttu-id="e57df-113">安全基准模板</span><span class="sxs-lookup"><span data-stu-id="e57df-113">Security baseline template</span></span>|
|<span data-ttu-id="e57df-114">specializedDevices</span><span class="sxs-lookup"><span data-stu-id="e57df-114">specializedDevices</span></span>|<span data-ttu-id="e57df-115">1 </span><span class="sxs-lookup"><span data-stu-id="e57df-115">1</span></span>|<span data-ttu-id="e57df-116">专用设备模板</span><span class="sxs-lookup"><span data-stu-id="e57df-116">Specialized devices template</span></span>|
|<span data-ttu-id="e57df-117">advancedThreatProtectionSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="e57df-117">advancedThreatProtectionSecurityBaseline</span></span>|<span data-ttu-id="e57df-118">2 </span><span class="sxs-lookup"><span data-stu-id="e57df-118">2</span></span>|<span data-ttu-id="e57df-119">高级威胁防护安全基准模板</span><span class="sxs-lookup"><span data-stu-id="e57df-119">Advanced Threat Protection security baseline template</span></span>|
|<span data-ttu-id="e57df-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e57df-120">deviceConfiguration</span></span>|<span data-ttu-id="e57df-121">3 </span><span class="sxs-lookup"><span data-stu-id="e57df-121">3</span></span>|<span data-ttu-id="e57df-122">设备配置模板</span><span class="sxs-lookup"><span data-stu-id="e57df-122">Device configuration template</span></span>|
|<span data-ttu-id="e57df-123">自</span><span class="sxs-lookup"><span data-stu-id="e57df-123">custom</span></span>|<span data-ttu-id="e57df-124">4 </span><span class="sxs-lookup"><span data-stu-id="e57df-124">4</span></span>|<span data-ttu-id="e57df-125">自定义管理员定义的模板</span><span class="sxs-lookup"><span data-stu-id="e57df-125">Custom admin defined template</span></span>|
|<span data-ttu-id="e57df-126">securityTemplate</span><span class="sxs-lookup"><span data-stu-id="e57df-126">securityTemplate</span></span>|<span data-ttu-id="e57df-127">5 </span><span class="sxs-lookup"><span data-stu-id="e57df-127">5</span></span>|<span data-ttu-id="e57df-128">包含特定的安全重点设置的模板</span><span class="sxs-lookup"><span data-stu-id="e57df-128">Templates containing specific security focused settings</span></span>|
|<span data-ttu-id="e57df-129">microsoftEdgeSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="e57df-129">microsoftEdgeSecurityBaseline</span></span>|<span data-ttu-id="e57df-130">6 </span><span class="sxs-lookup"><span data-stu-id="e57df-130">6</span></span>|<span data-ttu-id="e57df-131">Microsoft Edge 安全基准模板</span><span class="sxs-lookup"><span data-stu-id="e57df-131">Microsoft Edge security baseline template</span></span>|
|<span data-ttu-id="e57df-132">microsoftOffice365ProPlusSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="e57df-132">microsoftOffice365ProPlusSecurityBaseline</span></span>|<span data-ttu-id="e57df-133">7 </span><span class="sxs-lookup"><span data-stu-id="e57df-133">7</span></span>|<span data-ttu-id="e57df-134">Microsoft Office 365 专业增强版安全基准模板</span><span class="sxs-lookup"><span data-stu-id="e57df-134">Microsoft Office 365 ProPlus security baseline template</span></span>|
|<span data-ttu-id="e57df-135">deviceCompliance</span><span class="sxs-lookup"><span data-stu-id="e57df-135">deviceCompliance</span></span>|<span data-ttu-id="e57df-136">8 </span><span class="sxs-lookup"><span data-stu-id="e57df-136">8</span></span>|<span data-ttu-id="e57df-137">设备合规性模板</span><span class="sxs-lookup"><span data-stu-id="e57df-137">Device compliance template</span></span>|



