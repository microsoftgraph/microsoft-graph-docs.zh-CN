---
title: deviceManagementTemplateType 枚举类型
description: 模板类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d86e9c10c0049f0835a8d4a6a73a171a3fa3989c
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538488"
---
# <a name="devicemanagementtemplatetype-enum-type"></a><span data-ttu-id="a3534-103">deviceManagementTemplateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a3534-103">deviceManagementTemplateType enum type</span></span>

> <span data-ttu-id="a3534-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a3534-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3534-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a3534-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3534-106">模板类型</span><span class="sxs-lookup"><span data-stu-id="a3534-106">Template type</span></span>

## <a name="members"></a><span data-ttu-id="a3534-107">成员</span><span class="sxs-lookup"><span data-stu-id="a3534-107">Members</span></span>
|<span data-ttu-id="a3534-108">成员</span><span class="sxs-lookup"><span data-stu-id="a3534-108">Member</span></span>|<span data-ttu-id="a3534-109">值</span><span class="sxs-lookup"><span data-stu-id="a3534-109">Value</span></span>|<span data-ttu-id="a3534-110">说明</span><span class="sxs-lookup"><span data-stu-id="a3534-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3534-111">securityBaseline</span><span class="sxs-lookup"><span data-stu-id="a3534-111">securityBaseline</span></span>|<span data-ttu-id="a3534-112">0</span><span class="sxs-lookup"><span data-stu-id="a3534-112">0</span></span>|<span data-ttu-id="a3534-113">安全基准模板</span><span class="sxs-lookup"><span data-stu-id="a3534-113">Security baseline template</span></span>|
|<span data-ttu-id="a3534-114">specializedDevices</span><span class="sxs-lookup"><span data-stu-id="a3534-114">specializedDevices</span></span>|<span data-ttu-id="a3534-115">1</span><span class="sxs-lookup"><span data-stu-id="a3534-115">1</span></span>|<span data-ttu-id="a3534-116">专用设备模板</span><span class="sxs-lookup"><span data-stu-id="a3534-116">Specialized devices template</span></span>|
|<span data-ttu-id="a3534-117">advancedThreatProtectionSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="a3534-117">advancedThreatProtectionSecurityBaseline</span></span>|<span data-ttu-id="a3534-118">双面</span><span class="sxs-lookup"><span data-stu-id="a3534-118">2</span></span>|<span data-ttu-id="a3534-119">高级威胁防护安全基准模板</span><span class="sxs-lookup"><span data-stu-id="a3534-119">Advanced Threat Protection security baseline template</span></span>|
|<span data-ttu-id="a3534-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a3534-120">deviceConfiguration</span></span>|<span data-ttu-id="a3534-121">第三章</span><span class="sxs-lookup"><span data-stu-id="a3534-121">3</span></span>|<span data-ttu-id="a3534-122">设备配置模板</span><span class="sxs-lookup"><span data-stu-id="a3534-122">Device configuration template</span></span>|
|<span data-ttu-id="a3534-123">自</span><span class="sxs-lookup"><span data-stu-id="a3534-123">custom</span></span>|<span data-ttu-id="a3534-124">4 </span><span class="sxs-lookup"><span data-stu-id="a3534-124">4</span></span>|<span data-ttu-id="a3534-125">自定义管理员定义的模板</span><span class="sxs-lookup"><span data-stu-id="a3534-125">Custom admin defined template</span></span>|
|<span data-ttu-id="a3534-126">securityTemplate</span><span class="sxs-lookup"><span data-stu-id="a3534-126">securityTemplate</span></span>|<span data-ttu-id="a3534-127">5 </span><span class="sxs-lookup"><span data-stu-id="a3534-127">5</span></span>|<span data-ttu-id="a3534-128">包含特定的安全重点设置的模板</span><span class="sxs-lookup"><span data-stu-id="a3534-128">Templates containing specific security focused settings</span></span>|
|<span data-ttu-id="a3534-129">microsoftEdgeSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="a3534-129">microsoftEdgeSecurityBaseline</span></span>|<span data-ttu-id="a3534-130">6 </span><span class="sxs-lookup"><span data-stu-id="a3534-130">6</span></span>|<span data-ttu-id="a3534-131">Microsoft Edge 安全基准模板</span><span class="sxs-lookup"><span data-stu-id="a3534-131">Microsoft Edge security baseline template</span></span>|
|<span data-ttu-id="a3534-132">microsoftOffice365ProPlusSecurityBaseline</span><span class="sxs-lookup"><span data-stu-id="a3534-132">microsoftOffice365ProPlusSecurityBaseline</span></span>|<span data-ttu-id="a3534-133">7 </span><span class="sxs-lookup"><span data-stu-id="a3534-133">7</span></span>|<span data-ttu-id="a3534-134">Microsoft Office 365 专业增强版安全基准模板</span><span class="sxs-lookup"><span data-stu-id="a3534-134">Microsoft Office 365 ProPlus security baseline template</span></span>|



