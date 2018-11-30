---
title: 在 Intune 中注册设备以进行管理
description: " (BYOD) 注册允许用户注册其个人电话、 平板电脑或 Pc。 企业拥有设备 (COD) 注册允许管理场景，例如远程擦除、共享设备或设备的用户相关性。"
ms.openlocfilehash: af0a8ac113451c775386ee503026cf04a5641a7d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047645"
---
# <a name="enroll-devices-for-management-in-intune"></a><span data-ttu-id="9afdc-104">在 Intune 中注册设备以进行管理</span><span class="sxs-lookup"><span data-stu-id="9afdc-104">Enroll devices for management in Intune</span></span>

> <span data-ttu-id="9afdc-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9afdc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9afdc-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9afdc-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9afdc-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9afdc-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="9afdc-108">你可以通过 Microsoft Intune 注册设备（包括 Windows 电脑）以启用移动设备管理 (MDM)。</span><span class="sxs-lookup"><span data-stu-id="9afdc-108">You can enroll devices, including Windows PCs, to enable mobile device management (MDM) with Microsoft Intune.</span></span> <span data-ttu-id="9afdc-109">本主题介绍在 Intune 管理中注册移动设备的不同方法。</span><span class="sxs-lookup"><span data-stu-id="9afdc-109">This topic describes different ways to enroll mobile devices in Intune management.</span></span> <span data-ttu-id="9afdc-110">注册设备的方法取决于需要的设备类型、所有权和管理级别。</span><span class="sxs-lookup"><span data-stu-id="9afdc-110">The way you enroll your devices depends on the device type, ownership, and the level of management that's needed.</span></span> <span data-ttu-id="9afdc-111">“自带设备”(BYOD) 注册可让用户注册其个人手机、平板电脑或电脑。</span><span class="sxs-lookup"><span data-stu-id="9afdc-111">"Bring your own device" (BYOD) enrollment lets users enroll their personal phones, tablets, or PCs.</span></span> <span data-ttu-id="9afdc-112">企业拥有设备 (COD) 注册允许管理场景，例如远程擦除、共享设备或设备的用户相关性。</span><span class="sxs-lookup"><span data-stu-id="9afdc-112">Corporate-owned device (COD) enrollment enables management scenarios like remote wipe, shared devices, or user affinity for a device.</span></span>

<span data-ttu-id="9afdc-113">以下 Graph 资源可用于在 Intune 中管理注册：</span><span class="sxs-lookup"><span data-stu-id="9afdc-113">The following Graph resources are available to manage enrollment in Intune:</span></span>

- [<span data-ttu-id="9afdc-114">证书连接器设置</span><span class="sxs-lookup"><span data-stu-id="9afdc-114">Certificate connector setting</span></span>](intune-onboarding-certificateconnectorsetting.md)
- [<span data-ttu-id="9afdc-115">管理的设备和应用程序数据</span><span class="sxs-lookup"><span data-stu-id="9afdc-115">Device and app management data</span></span>](intune-onboarding-deviceandappmanagementdata.md)
- [<span data-ttu-id="9afdc-116">设备注册配置</span><span class="sxs-lookup"><span data-stu-id="9afdc-116">Device enrollment configuration</span></span>](intune-onboarding-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="9afdc-117">设备注册限制配置</span><span class="sxs-lookup"><span data-stu-id="9afdc-117">Device enrollment limit configuration</span></span>](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [<span data-ttu-id="9afdc-118">设备注册平台限制</span><span class="sxs-lookup"><span data-stu-id="9afdc-118">Device enrollment platform restriction</span></span>](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [<span data-ttu-id="9afdc-119">设备注册平台限制配置</span><span class="sxs-lookup"><span data-stu-id="9afdc-119">Device enrollment platform restrictions configuration</span></span>](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [<span data-ttu-id="9afdc-120">设备注册 Windows Hello 企业版配置</span><span class="sxs-lookup"><span data-stu-id="9afdc-120">Device enrollment Windows Hello for business configuration</span></span>](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [<span data-ttu-id="9afdc-121">设备管理 exchange 访问级别</span><span class="sxs-lookup"><span data-stu-id="9afdc-121">Device management exchange access level</span></span>](intune-onboarding-devicemanagementexchangeaccesslevel.md)
- [<span data-ttu-id="9afdc-122">设备管理 exchange 访问规则</span><span class="sxs-lookup"><span data-stu-id="9afdc-122">Device management exchange access rule</span></span>](intune-onboarding-devicemanagementexchangeaccessrule.md)
- [<span data-ttu-id="9afdc-123">设备管理 exchange 访问规则类型</span><span class="sxs-lookup"><span data-stu-id="9afdc-123">Device management exchange access rule type</span></span>](intune-onboarding-devicemanagementexchangeaccessruletype.md)
- [<span data-ttu-id="9afdc-124">设备管理 Exchange 连接器</span><span class="sxs-lookup"><span data-stu-id="9afdc-124">Device management exchange connector</span></span>](intune-onboarding-devicemanagementexchangeconnector.md)
- [<span data-ttu-id="9afdc-125">设备管理 exchange 连接器状态</span><span class="sxs-lookup"><span data-stu-id="9afdc-125">Device management exchange connector status</span></span>](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [<span data-ttu-id="9afdc-126">设备管理 exchange 连接器同步类型</span><span class="sxs-lookup"><span data-stu-id="9afdc-126">Device management exchange connector sync type</span></span>](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [<span data-ttu-id="9afdc-127">设备管理 exchange 连接器类型</span><span class="sxs-lookup"><span data-stu-id="9afdc-127">Device management exchange connector type</span></span>](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [<span data-ttu-id="9afdc-128">设备管理 exchange 设备类</span><span class="sxs-lookup"><span data-stu-id="9afdc-128">Device management exchange device class</span></span>](intune-onboarding-devicemanagementexchangedeviceclass.md)
- [<span data-ttu-id="9afdc-129">设备管理 exchange 内部部署策略</span><span class="sxs-lookup"><span data-stu-id="9afdc-129">Device management exchange on-premises policy</span></span>](intune-onboarding-devicemanagementexchangeonpremisespolicy.md)
- [<span data-ttu-id="9afdc-130">设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="9afdc-130">Device management partner</span></span>](intune-onboarding-devicemanagementpartner.md)
- [<span data-ttu-id="9afdc-131">设备管理合作伙伴应用程序类型</span><span class="sxs-lookup"><span data-stu-id="9afdc-131">Device management partner app type</span></span>](intune-onboarding-devicemanagementpartnerapptype.md)
- [<span data-ttu-id="9afdc-132">设备管理合作伙伴租户状态</span><span class="sxs-lookup"><span data-stu-id="9afdc-132">Device management partner tenant state</span></span>](intune-onboarding-devicemanagementpartnertenantstate.md)
- [<span data-ttu-id="9afdc-133">注册配置分配</span><span class="sxs-lookup"><span data-stu-id="9afdc-133">Enrollment configuration assignment</span></span>](intune-onboarding-enrollmentconfigurationassignment.md)
- [<span data-ttu-id="9afdc-134">Intune 品牌</span><span class="sxs-lookup"><span data-stu-id="9afdc-134">Intune brand</span></span>](intune-onboarding-intunebrand.md)
- [<span data-ttu-id="9afdc-135">MDM 证书颁发机构</span><span class="sxs-lookup"><span data-stu-id="9afdc-135">MDM authority</span></span>](intune-onboarding-mdmauthority.md)
- [<span data-ttu-id="9afdc-136">Microsoft 存储业务门户选择选项</span><span class="sxs-lookup"><span data-stu-id="9afdc-136">Microsoft store for business portal selection options</span></span>](intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)
- [<span data-ttu-id="9afdc-137">移动威胁防护连接器</span><span class="sxs-lookup"><span data-stu-id="9afdc-137">Mobile threat defense connector</span></span>](intune-onboarding-mobilethreatdefenseconnector.md)
- [<span data-ttu-id="9afdc-138">移动威胁合作伙伴租户状态</span><span class="sxs-lookup"><span data-stu-id="9afdc-138">Mobile threat partner tenant state</span></span>](intune-onboarding-mobilethreatpartnertenantstate.md)
- [<span data-ttu-id="9afdc-139">本地条件访问设置</span><span class="sxs-lookup"><span data-stu-id="9afdc-139">On-premises conditional access settings</span></span>](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [<span data-ttu-id="9afdc-140">组织</span><span class="sxs-lookup"><span data-stu-id="9afdc-140">Organization</span></span>](intune-onboarding-organization.md)
- [<span data-ttu-id="9afdc-141">端加载项</span><span class="sxs-lookup"><span data-stu-id="9afdc-141">Side loading key</span></span>](intune-onboarding-sideloadingkey.md)
- [<span data-ttu-id="9afdc-142">VPP 令牌</span><span class="sxs-lookup"><span data-stu-id="9afdc-142">VPP token</span></span>](intune-onboarding-vpptoken.md)
- [<span data-ttu-id="9afdc-143">VPP 令牌操作结果</span><span class="sxs-lookup"><span data-stu-id="9afdc-143">VPP token action result</span></span>](intune-onboarding-vpptokenactionresult.md)
- [<span data-ttu-id="9afdc-144">VPP 令牌许可证摘要</span><span class="sxs-lookup"><span data-stu-id="9afdc-144">VPP token license summary</span></span>](intune-onboarding-vpptokenlicensesummary.md)
- [<span data-ttu-id="9afdc-145">VPP 令牌 revoke 许可证操作结果</span><span class="sxs-lookup"><span data-stu-id="9afdc-145">VPP token revoke licenses action result</span></span>](intune-onboarding-vpptokenrevokelicensesactionresult.md)
- [<span data-ttu-id="9afdc-146">VPP 令牌状态</span><span class="sxs-lookup"><span data-stu-id="9afdc-146">VPP token state</span></span>](intune-onboarding-vpptokenstate.md)
- [<span data-ttu-id="9afdc-147">VPP 令牌的同步状态</span><span class="sxs-lookup"><span data-stu-id="9afdc-147">VPP token sync status</span></span>](intune-onboarding-vpptokensyncstatus.md)
- [<span data-ttu-id="9afdc-148">Windows 10 注册完成页上配置</span><span class="sxs-lookup"><span data-stu-id="9afdc-148">Windows 10 enrollment completion page configuration</span></span>](intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)
- [<span data-ttu-id="9afdc-149">Windows Hello 业务 PIN 用法</span><span class="sxs-lookup"><span data-stu-id="9afdc-149">Windows Hello for business PIN usage</span></span>](intune-onboarding-windowshelloforbusinesspinusage.md)
