---
title: deviceManagementTemplateType 枚举类型
description: 模板类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 595dd535b46657872f76c7a0571d5005cc65db38
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528755"
---
# <a name="devicemanagementtemplatetype-enum-type"></a><span data-ttu-id="d1135-103">deviceManagementTemplateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d1135-103">deviceManagementTemplateType enum type</span></span>

<span data-ttu-id="d1135-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d1135-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1135-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d1135-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1135-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1135-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1135-107">模板类型</span><span class="sxs-lookup"><span data-stu-id="d1135-107">Template type</span></span>

## <a name="members"></a><span data-ttu-id="d1135-108">成员</span><span class="sxs-lookup"><span data-stu-id="d1135-108">Members</span></span>
|<span data-ttu-id="d1135-109">成员</span><span class="sxs-lookup"><span data-stu-id="d1135-109">Member</span></span>|<span data-ttu-id="d1135-110">值</span><span class="sxs-lookup"><span data-stu-id="d1135-110">Value</span></span>|<span data-ttu-id="d1135-111">说明</span><span class="sxs-lookup"><span data-stu-id="d1135-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1135-112">securityBaseline</span><span class="sxs-lookup"><span data-stu-id="d1135-112">securityBaseline</span></span>|<span data-ttu-id="d1135-113">0</span><span class="sxs-lookup"><span data-stu-id="d1135-113">0</span></span>|<span data-ttu-id="d1135-114">安全基准模板</span><span class="sxs-lookup"><span data-stu-id="d1135-114">Security baseline template</span></span>|
|<span data-ttu-id="d1135-115">specializedDevices</span><span class="sxs-lookup"><span data-stu-id="d1135-115">specializedDevices</span></span>|<span data-ttu-id="d1135-116">1 </span><span class="sxs-lookup"><span data-stu-id="d1135-116">1</span></span>|<span data-ttu-id="d1135-117">专用设备模板</span><span class="sxs-lookup"><span data-stu-id="d1135-117">Specialized devices template</span></span>|
|<span data-ttu-id="d1135-118">advancedThreatProtectionSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="d1135-118">advancedThreatProtectionSecurityBaseline</span></span>|<span data-ttu-id="d1135-119">2 </span><span class="sxs-lookup"><span data-stu-id="d1135-119">2</span></span>|<span data-ttu-id="d1135-120">高级威胁防护安全基准模板</span><span class="sxs-lookup"><span data-stu-id="d1135-120">Advanced Threat Protection security baseline template</span></span>|
|<span data-ttu-id="d1135-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d1135-121">deviceConfiguration</span></span>|<span data-ttu-id="d1135-122">3 </span><span class="sxs-lookup"><span data-stu-id="d1135-122">3</span></span>|<span data-ttu-id="d1135-123">设备配置模板</span><span class="sxs-lookup"><span data-stu-id="d1135-123">Device configuration template</span></span>|
|<span data-ttu-id="d1135-124">自</span><span class="sxs-lookup"><span data-stu-id="d1135-124">custom</span></span>|<span data-ttu-id="d1135-125">4 </span><span class="sxs-lookup"><span data-stu-id="d1135-125">4</span></span>|<span data-ttu-id="d1135-126">自定义管理员定义的模板</span><span class="sxs-lookup"><span data-stu-id="d1135-126">Custom admin defined template</span></span>|
|<span data-ttu-id="d1135-127">securityTemplate</span><span class="sxs-lookup"><span data-stu-id="d1135-127">securityTemplate</span></span>|<span data-ttu-id="d1135-128">5 </span><span class="sxs-lookup"><span data-stu-id="d1135-128">5</span></span>|<span data-ttu-id="d1135-129">包含特定的安全重点设置的模板</span><span class="sxs-lookup"><span data-stu-id="d1135-129">Templates containing specific security focused settings</span></span>|
|<span data-ttu-id="d1135-130">microsoftEdgeSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="d1135-130">microsoftEdgeSecurityBaseline</span></span>|<span data-ttu-id="d1135-131">6 </span><span class="sxs-lookup"><span data-stu-id="d1135-131">6</span></span>|<span data-ttu-id="d1135-132">Microsoft Edge 安全基准模板</span><span class="sxs-lookup"><span data-stu-id="d1135-132">Microsoft Edge security baseline template</span></span>|
|<span data-ttu-id="d1135-133">microsoftOffice365ProPlusSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="d1135-133">microsoftOffice365ProPlusSecurityBaseline</span></span>|<span data-ttu-id="d1135-134">7 </span><span class="sxs-lookup"><span data-stu-id="d1135-134">7</span></span>|<span data-ttu-id="d1135-135">Microsoft Office 365 专业增强版安全基准模板</span><span class="sxs-lookup"><span data-stu-id="d1135-135">Microsoft Office 365 ProPlus security baseline template</span></span>|
|<span data-ttu-id="d1135-136">deviceCompliance</span><span class="sxs-lookup"><span data-stu-id="d1135-136">deviceCompliance</span></span>|<span data-ttu-id="d1135-137">8 </span><span class="sxs-lookup"><span data-stu-id="d1135-137">8</span></span>|<span data-ttu-id="d1135-138">设备合规性模板</span><span class="sxs-lookup"><span data-stu-id="d1135-138">Device compliance template</span></span>|



