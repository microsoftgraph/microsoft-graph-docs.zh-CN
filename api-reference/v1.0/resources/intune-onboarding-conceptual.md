---
title: 在 Intune 中注册设备以进行管理
description: " （BYOD）注册允许用户注册其个人电话、平板电脑或电脑。 企业拥有设备 (COD) 注册允许管理场景，例如远程擦除、共享设备或设备的用户相关性。"
localization_priority: Normal
author: davidmu1
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 54a2a8bb3901f1a6938401963e8efcbd9e02f194
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360585"
---
# <a name="enroll-devices-for-management-in-intune"></a><span data-ttu-id="50d5e-104">在 Intune 中注册设备以进行管理</span><span class="sxs-lookup"><span data-stu-id="50d5e-104">Enroll devices for management in Intune</span></span>

> <span data-ttu-id="50d5e-105">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="50d5e-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="50d5e-106">你可以通过 Microsoft Intune 注册设备（包括 Windows 电脑）以启用移动设备管理 (MDM)。</span><span class="sxs-lookup"><span data-stu-id="50d5e-106">You can enroll devices, including Windows PCs, to enable mobile device management (MDM) with Microsoft Intune.</span></span> <span data-ttu-id="50d5e-107">本主题介绍在 Intune 管理中注册移动设备的不同方法。</span><span class="sxs-lookup"><span data-stu-id="50d5e-107">This topic describes different ways to enroll mobile devices in Intune management.</span></span> <span data-ttu-id="50d5e-108">注册设备的方法取决于需要的设备类型、所有权和管理级别。</span><span class="sxs-lookup"><span data-stu-id="50d5e-108">The way you enroll your devices depends on the device type, ownership, and the level of management that's needed.</span></span> <span data-ttu-id="50d5e-109">“自带设备”(BYOD) 注册可让用户注册其个人手机、平板电脑或电脑。</span><span class="sxs-lookup"><span data-stu-id="50d5e-109">"Bring your own device" (BYOD) enrollment lets users enroll their personal phones, tablets, or PCs.</span></span> <span data-ttu-id="50d5e-110">企业拥有设备 (COD) 注册允许管理场景，例如远程擦除、共享设备或设备的用户相关性。</span><span class="sxs-lookup"><span data-stu-id="50d5e-110">Corporate-owned device (COD) enrollment enables management scenarios like remote wipe, shared devices, or user affinity for a device.</span></span>

<span data-ttu-id="50d5e-111">以下 Graph 资源可用于在 Intune 中管理注册：</span><span class="sxs-lookup"><span data-stu-id="50d5e-111">The following Graph resources are available to manage enrollment in Intune:</span></span>  

- [<span data-ttu-id="50d5e-112">设备注册配置</span><span class="sxs-lookup"><span data-stu-id="50d5e-112">Device enrollment configuration</span></span>](intune-onboarding-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="50d5e-113">设备注册限制配置</span><span class="sxs-lookup"><span data-stu-id="50d5e-113">Device enrollment limit configuration</span></span>](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [<span data-ttu-id="50d5e-114">设备注册平台限制</span><span class="sxs-lookup"><span data-stu-id="50d5e-114">Device enrollment platform restriction</span></span>](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [<span data-ttu-id="50d5e-115">设备注册平台限制配置</span><span class="sxs-lookup"><span data-stu-id="50d5e-115">Device enrollment platform restrictions configuration</span></span>](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [<span data-ttu-id="50d5e-116">设备注册 Windows Hello 企业版配置</span><span class="sxs-lookup"><span data-stu-id="50d5e-116">Device enrollment Windows Hello for business configuration</span></span>](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [<span data-ttu-id="50d5e-117">设备管理 Exchange 连接器</span><span class="sxs-lookup"><span data-stu-id="50d5e-117">Device management exchange connector</span></span>](intune-onboarding-devicemanagementexchangeconnector.md)
- [<span data-ttu-id="50d5e-118">设备管理 Exchange 连接器状态</span><span class="sxs-lookup"><span data-stu-id="50d5e-118">Device management exchange connector status</span></span>](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [<span data-ttu-id="50d5e-119">设备管理 Exchange 连接器同步类型</span><span class="sxs-lookup"><span data-stu-id="50d5e-119">Device management exchange connector sync type</span></span>](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [<span data-ttu-id="50d5e-120">设备管理 Exchange 连接器类型</span><span class="sxs-lookup"><span data-stu-id="50d5e-120">Device management exchange connector type</span></span>](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [<span data-ttu-id="50d5e-121">设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="50d5e-121">Device management partner</span></span>](intune-onboarding-devicemanagementpartner.md)
- [<span data-ttu-id="50d5e-122">设备管理合作伙伴应用类型</span><span class="sxs-lookup"><span data-stu-id="50d5e-122">Device management partner app type</span></span>](intune-onboarding-devicemanagementpartnerapptype.md)
- [<span data-ttu-id="50d5e-123">设备管理合作伙伴租户状态</span><span class="sxs-lookup"><span data-stu-id="50d5e-123">Device management partner tenant state</span></span>](intune-onboarding-devicemanagementpartnertenantstate.md)
- [<span data-ttu-id="50d5e-124">支持</span><span class="sxs-lookup"><span data-stu-id="50d5e-124">Enablement</span></span>](intune-onboarding-enablement.md)
- [<span data-ttu-id="50d5e-125">注册配置分配</span><span class="sxs-lookup"><span data-stu-id="50d5e-125">Enrollment configuration assignment</span></span>](intune-onboarding-enrollmentconfigurationassignment.md)
- [<span data-ttu-id="50d5e-126">Intune 品牌</span><span class="sxs-lookup"><span data-stu-id="50d5e-126">Intune brand</span></span>](intune-onboarding-intunebrand.md)
- [<span data-ttu-id="50d5e-127">MDM 颁发机构</span><span class="sxs-lookup"><span data-stu-id="50d5e-127">MDM authority</span></span>](intune-onboarding-mdmauthority.md)
- [<span data-ttu-id="50d5e-128">移动威胁防护连接器</span><span class="sxs-lookup"><span data-stu-id="50d5e-128">Mobile threat defense connector</span></span>](intune-onboarding-mobilethreatdefenseconnector.md)
- [<span data-ttu-id="50d5e-129">移动威胁合作伙伴租户状态</span><span class="sxs-lookup"><span data-stu-id="50d5e-129">Mobile threat partner tenant state</span></span>](intune-onboarding-mobilethreatpartnertenantstate.md)
- [<span data-ttu-id="50d5e-130">本地条件访问设置</span><span class="sxs-lookup"><span data-stu-id="50d5e-130">On-premises conditional access settings</span></span>](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [<span data-ttu-id="50d5e-131">组织</span><span class="sxs-lookup"><span data-stu-id="50d5e-131">Organization</span></span>](intune-onboarding-organization.md)
- [<span data-ttu-id="50d5e-132">RGB 颜色</span><span class="sxs-lookup"><span data-stu-id="50d5e-132">RGB color</span></span>](intune-onboarding-rgbcolor.md)
- [<span data-ttu-id="50d5e-133">VPP 令牌</span><span class="sxs-lookup"><span data-stu-id="50d5e-133">VPP token</span></span>](intune-onboarding-vpptoken.md)
- [<span data-ttu-id="50d5e-134">VPP 令牌状态</span><span class="sxs-lookup"><span data-stu-id="50d5e-134">VPP token state</span></span>](intune-onboarding-vpptokenstate.md)
- [<span data-ttu-id="50d5e-135">VPP 令牌同步状态</span><span class="sxs-lookup"><span data-stu-id="50d5e-135">VPP token sync status</span></span>](intune-onboarding-vpptokensyncstatus.md)
- [<span data-ttu-id="50d5e-136">Windows Hello 企业版 PIN 使用情况</span><span class="sxs-lookup"><span data-stu-id="50d5e-136">Windows Hello for business PIN usage</span></span>](intune-onboarding-windowshelloforbusinesspinusage.md)

