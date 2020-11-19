---
title: 带有 Intune 的板载托管设备-Microsoft Graph API
description: 列出了用于板载 (配置和初始化租户组织的) 设备的 Intune 终结点 (REST) 的 Microsoft Graph API。
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 5788b1d7a13f0be84b0368dfa73e7932f4820d9d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49266548"
---
# <a name="enroll-devices-for-management-in-intune"></a><span data-ttu-id="fb400-103">在 Intune 中注册设备以进行管理</span><span class="sxs-lookup"><span data-stu-id="fb400-103">Enroll devices for management in Intune</span></span>

<span data-ttu-id="fb400-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb400-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb400-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fb400-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb400-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fb400-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb400-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fb400-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb400-108">你可以通过 Microsoft Intune 注册设备（包括 Windows 电脑）以启用移动设备管理 (MDM)。</span><span class="sxs-lookup"><span data-stu-id="fb400-108">You can enroll devices, including Windows PCs, to enable mobile device management (MDM) with Microsoft Intune.</span></span> <span data-ttu-id="fb400-109">本主题介绍在 Intune 管理中注册移动设备的不同方法。</span><span class="sxs-lookup"><span data-stu-id="fb400-109">This topic describes different ways to enroll mobile devices in Intune management.</span></span> <span data-ttu-id="fb400-110">注册设备的方法取决于需要的设备类型、所有权和管理级别。</span><span class="sxs-lookup"><span data-stu-id="fb400-110">The way you enroll your devices depends on the device type, ownership, and the level of management that's needed.</span></span> <span data-ttu-id="fb400-111">“自带设备”(BYOD) 注册可让用户注册其个人手机、平板电脑或电脑。</span><span class="sxs-lookup"><span data-stu-id="fb400-111">"Bring your own device" (BYOD) enrollment lets users enroll their personal phones, tablets, or PCs.</span></span> <span data-ttu-id="fb400-112">企业拥有设备 (COD) 注册允许管理场景，例如远程擦除、共享设备或设备的用户相关性。</span><span class="sxs-lookup"><span data-stu-id="fb400-112">Corporate-owned device (COD) enrollment enables management scenarios like remote wipe, shared devices, or user affinity for a device.</span></span>

<span data-ttu-id="fb400-113">以下 Graph 资源可用于在 Intune 中管理注册：</span><span class="sxs-lookup"><span data-stu-id="fb400-113">The following Graph resources are available to manage enrollment in Intune:</span></span>

- [<span data-ttu-id="fb400-114">证书连接器设置</span><span class="sxs-lookup"><span data-stu-id="fb400-114">Certificate connector setting</span></span>](intune-onboarding-certificateconnectorsetting.md)
- [<span data-ttu-id="fb400-115">合规性管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="fb400-115">Compliance management partner</span></span>](intune-onboarding-compliancemanagementpartner.md)
- [<span data-ttu-id="fb400-116">合规性管理合作伙伴分配</span><span class="sxs-lookup"><span data-stu-id="fb400-116">Compliance management partner assignment</span></span>](intune-onboarding-compliancemanagementpartnerassignment.md)
- [<span data-ttu-id="fb400-117">设备和应用管理数据</span><span class="sxs-lookup"><span data-stu-id="fb400-117">Device and app management data</span></span>](intune-onboarding-deviceandappmanagementdata.md)
- [<span data-ttu-id="fb400-118">设备 comanagement 证书颁发机构配置</span><span class="sxs-lookup"><span data-stu-id="fb400-118">Device comanagement authority configuration</span></span>](intune-onboarding-devicecomanagementauthorityconfiguration.md)
- [<span data-ttu-id="fb400-119">设备注册限制配置</span><span class="sxs-lookup"><span data-stu-id="fb400-119">Device enrollment limit configuration</span></span>](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [<span data-ttu-id="fb400-120">设备注册平台限制</span><span class="sxs-lookup"><span data-stu-id="fb400-120">Device enrollment platform restriction</span></span>](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [<span data-ttu-id="fb400-121">设备注册平台限制配置</span><span class="sxs-lookup"><span data-stu-id="fb400-121">Device enrollment platform restrictions configuration</span></span>](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [<span data-ttu-id="fb400-122">设备注册 Windows Hello 企业版配置</span><span class="sxs-lookup"><span data-stu-id="fb400-122">Device enrollment Windows Hello for business configuration</span></span>](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [<span data-ttu-id="fb400-123">设备管理 Exchange 访问级别</span><span class="sxs-lookup"><span data-stu-id="fb400-123">Device management exchange access level</span></span>](intune-onboarding-devicemanagementexchangeaccesslevel.md)
- [<span data-ttu-id="fb400-124">设备管理 Exchange 访问规则</span><span class="sxs-lookup"><span data-stu-id="fb400-124">Device management exchange access rule</span></span>](intune-onboarding-devicemanagementexchangeaccessrule.md)
- [<span data-ttu-id="fb400-125">设备管理 Exchange 访问规则类型</span><span class="sxs-lookup"><span data-stu-id="fb400-125">Device management exchange access rule type</span></span>](intune-onboarding-devicemanagementexchangeaccessruletype.md)
- [<span data-ttu-id="fb400-126">设备管理 Exchange 连接器</span><span class="sxs-lookup"><span data-stu-id="fb400-126">Device management exchange connector</span></span>](intune-onboarding-devicemanagementexchangeconnector.md)
- [<span data-ttu-id="fb400-127">设备管理 Exchange 连接器状态</span><span class="sxs-lookup"><span data-stu-id="fb400-127">Device management exchange connector status</span></span>](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [<span data-ttu-id="fb400-128">设备管理 Exchange 连接器同步类型</span><span class="sxs-lookup"><span data-stu-id="fb400-128">Device management exchange connector sync type</span></span>](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [<span data-ttu-id="fb400-129">设备管理 Exchange 连接器类型</span><span class="sxs-lookup"><span data-stu-id="fb400-129">Device management exchange connector type</span></span>](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [<span data-ttu-id="fb400-130">设备管理 Exchange 设备类</span><span class="sxs-lookup"><span data-stu-id="fb400-130">Device management exchange device class</span></span>](intune-onboarding-devicemanagementexchangedeviceclass.md)
- [<span data-ttu-id="fb400-131">设备管理 Exchange 本地策略</span><span class="sxs-lookup"><span data-stu-id="fb400-131">Device management exchange on-premises policy</span></span>](intune-onboarding-devicemanagementexchangeonpremisespolicy.md)
- [<span data-ttu-id="fb400-132">设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="fb400-132">Device management partner</span></span>](intune-onboarding-devicemanagementpartner.md)
- [<span data-ttu-id="fb400-133">设备管理合作伙伴应用类型</span><span class="sxs-lookup"><span data-stu-id="fb400-133">Device management partner app type</span></span>](intune-onboarding-devicemanagementpartnerapptype.md)
- [<span data-ttu-id="fb400-134">设备管理合作伙伴分配</span><span class="sxs-lookup"><span data-stu-id="fb400-134">Device management partner assignment</span></span>](intune-onboarding-devicemanagementpartnerassignment.md)
- [<span data-ttu-id="fb400-135">设备管理合作伙伴租户状态</span><span class="sxs-lookup"><span data-stu-id="fb400-135">Device management partner tenant state</span></span>](intune-onboarding-devicemanagementpartnertenantstate.md)
- [<span data-ttu-id="fb400-136">注册配置分配</span><span class="sxs-lookup"><span data-stu-id="fb400-136">Enrollment configuration assignment</span></span>](intune-onboarding-enrollmentconfigurationassignment.md)
- [<span data-ttu-id="fb400-137">Intune 品牌</span><span class="sxs-lookup"><span data-stu-id="fb400-137">Intune brand</span></span>](intune-onboarding-intunebrand.md)
- [<span data-ttu-id="fb400-138">MDM 颁发机构</span><span class="sxs-lookup"><span data-stu-id="fb400-138">MDM authority</span></span>](intune-onboarding-mdmauthority.md)
- [<span data-ttu-id="fb400-139">适用于企业的 Microsoft Store 门户选定内容的选项</span><span class="sxs-lookup"><span data-stu-id="fb400-139">Microsoft store for business portal selection options</span></span>](intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)
- [<span data-ttu-id="fb400-140">移动威胁防护连接器</span><span class="sxs-lookup"><span data-stu-id="fb400-140">Mobile threat defense connector</span></span>](intune-onboarding-mobilethreatdefenseconnector.md)
- [<span data-ttu-id="fb400-141">移动威胁合作伙伴租户状态</span><span class="sxs-lookup"><span data-stu-id="fb400-141">Mobile threat partner tenant state</span></span>](intune-onboarding-mobilethreatpartnertenantstate.md)
- [<span data-ttu-id="fb400-142">本地条件访问设置</span><span class="sxs-lookup"><span data-stu-id="fb400-142">On-premises conditional access settings</span></span>](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [<span data-ttu-id="fb400-143">组织</span><span class="sxs-lookup"><span data-stu-id="fb400-143">Organization</span></span>](intune-onboarding-organization.md)
- [<span data-ttu-id="fb400-144">侧加载密钥</span><span class="sxs-lookup"><span data-stu-id="fb400-144">Side loading key</span></span>](intune-onboarding-sideloadingkey.md)
- [<span data-ttu-id="fb400-145">VPP 令牌</span><span class="sxs-lookup"><span data-stu-id="fb400-145">VPP token</span></span>](intune-onboarding-vpptoken.md)
- [<span data-ttu-id="fb400-146">VPP 令牌操作结果</span><span class="sxs-lookup"><span data-stu-id="fb400-146">VPP token action result</span></span>](intune-onboarding-vpptokenactionresult.md)
- [<span data-ttu-id="fb400-147">VPP 令牌许可证摘要</span><span class="sxs-lookup"><span data-stu-id="fb400-147">VPP token license summary</span></span>](intune-onboarding-vpptokenlicensesummary.md)
- [<span data-ttu-id="fb400-148">VPP 令牌撤销许可证操作结果</span><span class="sxs-lookup"><span data-stu-id="fb400-148">VPP token revoke licenses action result</span></span>](intune-onboarding-vpptokenrevokelicensesactionresult.md)
- [<span data-ttu-id="fb400-149">VPP 令牌状态</span><span class="sxs-lookup"><span data-stu-id="fb400-149">VPP token state</span></span>](intune-onboarding-vpptokenstate.md)
- [<span data-ttu-id="fb400-150">VPP 令牌同步状态</span><span class="sxs-lookup"><span data-stu-id="fb400-150">VPP token sync status</span></span>](intune-onboarding-vpptokensyncstatus.md)
- [<span data-ttu-id="fb400-151">Windows 10 注册完成页配置</span><span class="sxs-lookup"><span data-stu-id="fb400-151">Windows 10 enrollment completion page configuration</span></span>](intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)
- [<span data-ttu-id="fb400-152">Windows Hello 企业版 PIN 使用情况</span><span class="sxs-lookup"><span data-stu-id="fb400-152">Windows Hello for business PIN usage</span></span>](intune-onboarding-windowshelloforbusinesspinusage.md)