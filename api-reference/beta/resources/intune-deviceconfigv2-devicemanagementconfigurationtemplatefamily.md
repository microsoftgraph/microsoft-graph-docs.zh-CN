---
title: deviceManagementConfigurationTemplateFamily 枚举类型
description: 描述 Template 实体的 TemplateFamily
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 088e1ccd80e59b95419c17d532c82c1ea9c388bc
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666686"
---
# <a name="devicemanagementconfigurationtemplatefamily-enum-type"></a><span data-ttu-id="2b528-103">deviceManagementConfigurationTemplateFamily 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2b528-103">deviceManagementConfigurationTemplateFamily enum type</span></span>

<span data-ttu-id="2b528-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b528-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b528-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2b528-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b528-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2b528-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b528-107">描述 Template 实体的 TemplateFamily</span><span class="sxs-lookup"><span data-stu-id="2b528-107">Describes the TemplateFamily for the Template entity</span></span>

## <a name="members"></a><span data-ttu-id="2b528-108">成员</span><span class="sxs-lookup"><span data-stu-id="2b528-108">Members</span></span>
|<span data-ttu-id="2b528-109">成员</span><span class="sxs-lookup"><span data-stu-id="2b528-109">Member</span></span>|<span data-ttu-id="2b528-110">值</span><span class="sxs-lookup"><span data-stu-id="2b528-110">Value</span></span>|<span data-ttu-id="2b528-111">说明</span><span class="sxs-lookup"><span data-stu-id="2b528-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b528-112">无</span><span class="sxs-lookup"><span data-stu-id="2b528-112">none</span></span>|<span data-ttu-id="2b528-113">0</span><span class="sxs-lookup"><span data-stu-id="2b528-113">0</span></span>|<span data-ttu-id="2b528-114">策略未链接到模板时，模板系列默认为</span><span class="sxs-lookup"><span data-stu-id="2b528-114">Default for Template Family when Policy is not linked to a Template</span></span>|
|<span data-ttu-id="2b528-115">endpointSecurityAntivirus</span><span class="sxs-lookup"><span data-stu-id="2b528-115">endpointSecurityAntivirus</span></span>|<span data-ttu-id="2b528-116">10  </span><span class="sxs-lookup"><span data-stu-id="2b528-116">10</span></span>|<span data-ttu-id="2b528-117">EndpointSecurity 防病毒的模板系列，用于管理托管设备的离散防病毒设置组</span><span class="sxs-lookup"><span data-stu-id="2b528-117">Template Family for EndpointSecurityAntivirus that manages the discrete group of antivirus settings for managed devices</span></span>|
|<span data-ttu-id="2b528-118">endpointSecurityDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="2b528-118">endpointSecurityDiskEncryption</span></span>|<span data-ttu-id="2b528-119">11</span><span class="sxs-lookup"><span data-stu-id="2b528-119">11</span></span>|<span data-ttu-id="2b528-120">EndpointSecurityDiskEncryption 的模板系列，提供与设备内置加密方法（如 FileVault 或 BitLocker</span><span class="sxs-lookup"><span data-stu-id="2b528-120">Template Family for EndpointSecurityDiskEncryption that provides settings that are relevant for a devices built-in encryption  method, like FileVault or BitLocker</span></span>|
|<span data-ttu-id="2b528-121">endpointSecurityFirewall</span><span class="sxs-lookup"><span data-stu-id="2b528-121">endpointSecurityFirewall</span></span>|<span data-ttu-id="2b528-122">12 </span><span class="sxs-lookup"><span data-stu-id="2b528-122">12</span></span>|<span data-ttu-id="2b528-123">EndpointSecurityFirewall 的模板系列，可帮助为运行 macOS 和 Windows 10</span><span class="sxs-lookup"><span data-stu-id="2b528-123">Template Family for EndpointSecurityFirewall that helps configure a devices built-in firewall for device that run macOS and Windows 10</span></span>|
|<span data-ttu-id="2b528-124">endpointSecurityEndpointDetectionAndResponse</span><span class="sxs-lookup"><span data-stu-id="2b528-124">endpointSecurityEndpointDetectionAndResponse</span></span>|<span data-ttu-id="2b528-125">13</span><span class="sxs-lookup"><span data-stu-id="2b528-125">13</span></span>|<span data-ttu-id="2b528-126">EndpointSecurityEndpointDectionAndResponse 的模板系列，便于管理 EDR 设置，以及将设备载入 Microsoft Defender for Endpoint</span><span class="sxs-lookup"><span data-stu-id="2b528-126">Template Family for EndpointSecurityEndpointDectionAndResponse that facilitates management of the EDR settings and onboard devices to Microsoft Defender for Endpoint</span></span>|
|<span data-ttu-id="2b528-127">endpointSecurityAttackSurfaceReduction</span><span class="sxs-lookup"><span data-stu-id="2b528-127">endpointSecurityAttackSurfaceReduction</span></span>|<span data-ttu-id="2b528-128">14 </span><span class="sxs-lookup"><span data-stu-id="2b528-128">14</span></span>|<span data-ttu-id="2b528-129">EndpointSecurityAttackSurfaceReduction 的模板系列，通过最大程度地减少组织易受网络威胁和攻击的位置，帮助减少攻击面</span><span class="sxs-lookup"><span data-stu-id="2b528-129">Template Family for EndpointSecurityAttackSurfaceReduction that help reduce your attack surfaces, by minimizing the places where your organization is vulnerable to cyberthreats and attacks</span></span>|
|<span data-ttu-id="2b528-130">endpointSecurityAccountProtection</span><span class="sxs-lookup"><span data-stu-id="2b528-130">endpointSecurityAccountProtection</span></span>|<span data-ttu-id="2b528-131">15</span><span class="sxs-lookup"><span data-stu-id="2b528-131">15</span></span>|<span data-ttu-id="2b528-132">EndpointSecurityAccountProtection 的模板系列，有助于保护用户的标识和帐户</span><span class="sxs-lookup"><span data-stu-id="2b528-132">Template Family for EndpointSecurityAccountProtection that facilitates protecting the identity and accounts of users</span></span>|
|<span data-ttu-id="2b528-133">endpointSecurityApplicationControl</span><span class="sxs-lookup"><span data-stu-id="2b528-133">endpointSecurityApplicationControl</span></span>|<span data-ttu-id="2b528-134">16 </span><span class="sxs-lookup"><span data-stu-id="2b528-134">16</span></span>|<span data-ttu-id="2b528-135">ApplicationControl 的模板系列，通过限制用户可以运行的应用程序和在 System Core 中运行的代码来减少安全威胁， (内核) </span><span class="sxs-lookup"><span data-stu-id="2b528-135">Template Family for ApplicationControl that helps mitigate security threats by restricting the applications that users can run and the code that runs in the System Core (kernel)</span></span>|




