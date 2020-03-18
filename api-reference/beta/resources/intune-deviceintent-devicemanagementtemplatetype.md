---
title: deviceManagementTemplateType 枚举类型
description: 模板类型
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d75494230ae69e06511e7d6eb818e4592e1496b5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785230"
---
# <a name="devicemanagementtemplatetype-enum-type"></a><span data-ttu-id="75cef-103">deviceManagementTemplateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="75cef-103">deviceManagementTemplateType enum type</span></span>

> <span data-ttu-id="75cef-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="75cef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75cef-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="75cef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75cef-106">模板类型</span><span class="sxs-lookup"><span data-stu-id="75cef-106">Template type</span></span>

## <a name="members"></a><span data-ttu-id="75cef-107">成员</span><span class="sxs-lookup"><span data-stu-id="75cef-107">Members</span></span>
|<span data-ttu-id="75cef-108">成员</span><span class="sxs-lookup"><span data-stu-id="75cef-108">Member</span></span>|<span data-ttu-id="75cef-109">值</span><span class="sxs-lookup"><span data-stu-id="75cef-109">Value</span></span>|<span data-ttu-id="75cef-110">说明</span><span class="sxs-lookup"><span data-stu-id="75cef-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75cef-111">securityBaseline</span><span class="sxs-lookup"><span data-stu-id="75cef-111">securityBaseline</span></span>|<span data-ttu-id="75cef-112">0</span><span class="sxs-lookup"><span data-stu-id="75cef-112">0</span></span>|<span data-ttu-id="75cef-113">安全基准模板</span><span class="sxs-lookup"><span data-stu-id="75cef-113">Security baseline template</span></span>|
|<span data-ttu-id="75cef-114">specializedDevices</span><span class="sxs-lookup"><span data-stu-id="75cef-114">specializedDevices</span></span>|<span data-ttu-id="75cef-115">1</span><span class="sxs-lookup"><span data-stu-id="75cef-115">1</span></span>|<span data-ttu-id="75cef-116">专用设备模板</span><span class="sxs-lookup"><span data-stu-id="75cef-116">Specialized devices template</span></span>|
|<span data-ttu-id="75cef-117">advancedThreatProtectionSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="75cef-117">advancedThreatProtectionSecurityBaseline</span></span>|<span data-ttu-id="75cef-118">双面</span><span class="sxs-lookup"><span data-stu-id="75cef-118">2</span></span>|<span data-ttu-id="75cef-119">高级威胁防护安全基准模板</span><span class="sxs-lookup"><span data-stu-id="75cef-119">Advanced Threat Protection security baseline template</span></span>|
|<span data-ttu-id="75cef-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="75cef-120">deviceConfiguration</span></span>|<span data-ttu-id="75cef-121">第三章</span><span class="sxs-lookup"><span data-stu-id="75cef-121">3</span></span>|<span data-ttu-id="75cef-122">设备配置模板</span><span class="sxs-lookup"><span data-stu-id="75cef-122">Device configuration template</span></span>|
|<span data-ttu-id="75cef-123">自</span><span class="sxs-lookup"><span data-stu-id="75cef-123">custom</span></span>|<span data-ttu-id="75cef-124">4 </span><span class="sxs-lookup"><span data-stu-id="75cef-124">4</span></span>|<span data-ttu-id="75cef-125">自定义管理员定义的模板</span><span class="sxs-lookup"><span data-stu-id="75cef-125">Custom admin defined template</span></span>|
|<span data-ttu-id="75cef-126">securityTemplate</span><span class="sxs-lookup"><span data-stu-id="75cef-126">securityTemplate</span></span>|<span data-ttu-id="75cef-127">5 </span><span class="sxs-lookup"><span data-stu-id="75cef-127">5</span></span>|<span data-ttu-id="75cef-128">包含特定的安全重点设置的模板</span><span class="sxs-lookup"><span data-stu-id="75cef-128">Templates containing specific security focused settings</span></span>|
|<span data-ttu-id="75cef-129">microsoftEdgeSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="75cef-129">microsoftEdgeSecurityBaseline</span></span>|<span data-ttu-id="75cef-130">6 </span><span class="sxs-lookup"><span data-stu-id="75cef-130">6</span></span>|<span data-ttu-id="75cef-131">Microsoft Edge 安全基准模板</span><span class="sxs-lookup"><span data-stu-id="75cef-131">Microsoft Edge security baseline template</span></span>|
|<span data-ttu-id="75cef-132">microsoftOffice365ProPlusSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="75cef-132">microsoftOffice365ProPlusSecurityBaseline</span></span>|<span data-ttu-id="75cef-133">7 </span><span class="sxs-lookup"><span data-stu-id="75cef-133">7</span></span>|<span data-ttu-id="75cef-134">Microsoft Office 365 专业增强版安全基准模板</span><span class="sxs-lookup"><span data-stu-id="75cef-134">Microsoft Office 365 ProPlus security baseline template</span></span>|
|<span data-ttu-id="75cef-135">deviceCompliance</span><span class="sxs-lookup"><span data-stu-id="75cef-135">deviceCompliance</span></span>|<span data-ttu-id="75cef-136">8 </span><span class="sxs-lookup"><span data-stu-id="75cef-136">8</span></span>|<span data-ttu-id="75cef-137">设备合规性模板</span><span class="sxs-lookup"><span data-stu-id="75cef-137">Device compliance template</span></span>|



