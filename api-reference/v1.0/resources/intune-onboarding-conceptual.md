---
title: 在 Intune 中注册设备以进行管理
description: "  (BYOD) 注册允许用户注册其个人手机、平板电脑或电脑。 企业拥有设备 (COD) 注册允许管理场景，例如远程擦除、共享设备或设备的用户相关性。"
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: d8a68ee75a267da062a462c8f015f1832494c5e1
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107744"
---
# <a name="enroll-devices-for-management-in-intune"></a><span data-ttu-id="d7e1a-104">在 Intune 中注册设备以进行管理</span><span class="sxs-lookup"><span data-stu-id="d7e1a-104">Enroll devices for management in Intune</span></span>

<span data-ttu-id="d7e1a-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7e1a-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7e1a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户 [正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d7e1a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="d7e1a-107">你可以通过 Microsoft Intune 注册设备（包括 Windows 电脑）以启用移动设备管理 (MDM)。</span><span class="sxs-lookup"><span data-stu-id="d7e1a-107">You can enroll devices, including Windows PCs, to enable mobile device management (MDM) with Microsoft Intune.</span></span> <span data-ttu-id="d7e1a-108">本主题介绍在 Intune 管理中注册移动设备的不同方法。</span><span class="sxs-lookup"><span data-stu-id="d7e1a-108">This topic describes different ways to enroll mobile devices in Intune management.</span></span> <span data-ttu-id="d7e1a-109">注册设备的方法取决于需要的设备类型、所有权和管理级别。</span><span class="sxs-lookup"><span data-stu-id="d7e1a-109">The way you enroll your devices depends on the device type, ownership, and the level of management that's needed.</span></span> <span data-ttu-id="d7e1a-110">“自带设备”(BYOD) 注册可让用户注册其个人手机、平板电脑或电脑。</span><span class="sxs-lookup"><span data-stu-id="d7e1a-110">"Bring your own device" (BYOD) enrollment lets users enroll their personal phones, tablets, or PCs.</span></span> <span data-ttu-id="d7e1a-111">企业拥有设备 (COD) 注册允许管理场景，例如远程擦除、共享设备或设备的用户相关性。</span><span class="sxs-lookup"><span data-stu-id="d7e1a-111">Corporate-owned device (COD) enrollment enables management scenarios like remote wipe, shared devices, or user affinity for a device.</span></span>

<span data-ttu-id="d7e1a-112">以下 Graph 资源可用于在 Intune 中管理注册：</span><span class="sxs-lookup"><span data-stu-id="d7e1a-112">The following Graph resources are available to manage enrollment in Intune:</span></span>  

- [<span data-ttu-id="d7e1a-113">合规性管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="d7e1a-113">Compliance management partner</span></span>](intune-onboarding-compliancemanagementpartner.md)
- [<span data-ttu-id="d7e1a-114">合规性管理合作伙伴分配</span><span class="sxs-lookup"><span data-stu-id="d7e1a-114">Compliance management partner assignment</span></span>](intune-onboarding-compliancemanagementpartnerassignment.md)
- [<span data-ttu-id="d7e1a-115">设备应用管理</span><span class="sxs-lookup"><span data-stu-id="d7e1a-115">Device app management</span></span>](intune-onboarding-deviceappmanagement.md)
- [<span data-ttu-id="d7e1a-116">设备类别</span><span class="sxs-lookup"><span data-stu-id="d7e1a-116">Device category</span></span>](intune-onboarding-devicecategory.md)
- [<span data-ttu-id="d7e1a-117">设备注册配置</span><span class="sxs-lookup"><span data-stu-id="d7e1a-117">Device enrollment configuration</span></span>](intune-onboarding-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="d7e1a-118">设备注册限制配置</span><span class="sxs-lookup"><span data-stu-id="d7e1a-118">Device enrollment limit configuration</span></span>](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [<span data-ttu-id="d7e1a-119">设备注册平台限制</span><span class="sxs-lookup"><span data-stu-id="d7e1a-119">Device enrollment platform restriction</span></span>](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [<span data-ttu-id="d7e1a-120">设备注册平台限制配置</span><span class="sxs-lookup"><span data-stu-id="d7e1a-120">Device enrollment platform restrictions configuration</span></span>](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [<span data-ttu-id="d7e1a-121">设备注册 Windows Hello 企业版配置</span><span class="sxs-lookup"><span data-stu-id="d7e1a-121">Device enrollment Windows Hello for business configuration</span></span>](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [<span data-ttu-id="d7e1a-122">设备管理</span><span class="sxs-lookup"><span data-stu-id="d7e1a-122">Device management</span></span>](intune-onboarding-devicemanagement.md)
- [<span data-ttu-id="d7e1a-123">设备管理 Exchange 连接器</span><span class="sxs-lookup"><span data-stu-id="d7e1a-123">Device management exchange connector</span></span>](intune-onboarding-devicemanagementexchangeconnector.md)
- [<span data-ttu-id="d7e1a-124">设备管理 Exchange 连接器状态</span><span class="sxs-lookup"><span data-stu-id="d7e1a-124">Device management exchange connector status</span></span>](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [<span data-ttu-id="d7e1a-125">设备管理 Exchange 连接器同步类型</span><span class="sxs-lookup"><span data-stu-id="d7e1a-125">Device management exchange connector sync type</span></span>](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [<span data-ttu-id="d7e1a-126">设备管理 Exchange 连接器类型</span><span class="sxs-lookup"><span data-stu-id="d7e1a-126">Device management exchange connector type</span></span>](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [<span data-ttu-id="d7e1a-127">设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="d7e1a-127">Device management partner</span></span>](intune-onboarding-devicemanagementpartner.md)
- [<span data-ttu-id="d7e1a-128">设备管理合作伙伴应用类型</span><span class="sxs-lookup"><span data-stu-id="d7e1a-128">Device management partner app type</span></span>](intune-onboarding-devicemanagementpartnerapptype.md)
- [<span data-ttu-id="d7e1a-129">设备管理合作伙伴租户状态</span><span class="sxs-lookup"><span data-stu-id="d7e1a-129">Device management partner tenant state</span></span>](intune-onboarding-devicemanagementpartnertenantstate.md)
- [<span data-ttu-id="d7e1a-130">支持</span><span class="sxs-lookup"><span data-stu-id="d7e1a-130">Enablement</span></span>](intune-onboarding-enablement.md)
- [<span data-ttu-id="d7e1a-131">注册配置分配</span><span class="sxs-lookup"><span data-stu-id="d7e1a-131">Enrollment configuration assignment</span></span>](intune-onboarding-enrollmentconfigurationassignment.md)
- [<span data-ttu-id="d7e1a-132">Intune 品牌</span><span class="sxs-lookup"><span data-stu-id="d7e1a-132">Intune brand</span></span>](intune-onboarding-intunebrand.md)
- [<span data-ttu-id="d7e1a-133">MDM 颁发机构</span><span class="sxs-lookup"><span data-stu-id="d7e1a-133">MDM authority</span></span>](intune-onboarding-mdmauthority.md)
- [<span data-ttu-id="d7e1a-134">移动威胁防护连接器</span><span class="sxs-lookup"><span data-stu-id="d7e1a-134">Mobile threat defense connector</span></span>](intune-onboarding-mobilethreatdefenseconnector.md)
- [<span data-ttu-id="d7e1a-135">移动威胁合作伙伴租户状态</span><span class="sxs-lookup"><span data-stu-id="d7e1a-135">Mobile threat partner tenant state</span></span>](intune-onboarding-mobilethreatpartnertenantstate.md)
- [<span data-ttu-id="d7e1a-136">本地条件访问设置</span><span class="sxs-lookup"><span data-stu-id="d7e1a-136">On-premises conditional access settings</span></span>](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [<span data-ttu-id="d7e1a-137">组织</span><span class="sxs-lookup"><span data-stu-id="d7e1a-137">Organization</span></span>](intune-onboarding-organization.md)
- [<span data-ttu-id="d7e1a-138">RGB 颜色</span><span class="sxs-lookup"><span data-stu-id="d7e1a-138">RGB color</span></span>](intune-onboarding-rgbcolor.md)
- [<span data-ttu-id="d7e1a-139">用户</span><span class="sxs-lookup"><span data-stu-id="d7e1a-139">User</span></span>](intune-onboarding-user.md)
- [<span data-ttu-id="d7e1a-140">VPP 令牌</span><span class="sxs-lookup"><span data-stu-id="d7e1a-140">VPP token</span></span>](intune-onboarding-vpptoken.md)
- [<span data-ttu-id="d7e1a-141">VPP 令牌状态</span><span class="sxs-lookup"><span data-stu-id="d7e1a-141">VPP token state</span></span>](intune-onboarding-vpptokenstate.md)
- [<span data-ttu-id="d7e1a-142">VPP 令牌同步状态</span><span class="sxs-lookup"><span data-stu-id="d7e1a-142">VPP token sync status</span></span>](intune-onboarding-vpptokensyncstatus.md)
- [<span data-ttu-id="d7e1a-143">Windows Hello 企业版 PIN 使用情况</span><span class="sxs-lookup"><span data-stu-id="d7e1a-143">Windows Hello for business PIN usage</span></span>](intune-onboarding-windowshelloforbusinesspinusage.md)