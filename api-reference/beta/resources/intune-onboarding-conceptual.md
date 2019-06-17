---
title: 带有 Intune 的板载托管设备-Microsoft Graph API
description: 列出用于为租户组织进行板载 (配置和初始化) 设备的 Intune 终结点 (REST) 的 Microsoft Graph API。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: 08f026a4de95c3720c303f6c324690957d83f076
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34982460"
---
# <a name="enroll-devices-for-management-in-intune"></a><span data-ttu-id="ba639-103">在 Intune 中注册设备以进行管理</span><span class="sxs-lookup"><span data-stu-id="ba639-103">Enroll devices for management in Intune</span></span>

> <span data-ttu-id="ba639-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ba639-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba639-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ba639-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ba639-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ba639-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba639-107">你可以通过 Microsoft Intune 注册设备（包括 Windows 电脑）以启用移动设备管理 (MDM)。</span><span class="sxs-lookup"><span data-stu-id="ba639-107">You can enroll devices, including Windows PCs, to enable mobile device management (MDM) with Microsoft Intune.</span></span> <span data-ttu-id="ba639-108">本主题介绍在 Intune 管理中注册移动设备的不同方法。</span><span class="sxs-lookup"><span data-stu-id="ba639-108">This topic describes different ways to enroll mobile devices in Intune management.</span></span> <span data-ttu-id="ba639-109">注册设备的方法取决于需要的设备类型、所有权和管理级别。</span><span class="sxs-lookup"><span data-stu-id="ba639-109">The way you enroll your devices depends on the device type, ownership, and the level of management that's needed.</span></span> <span data-ttu-id="ba639-110">“自带设备”(BYOD) 注册可让用户注册其个人手机、平板电脑或电脑。</span><span class="sxs-lookup"><span data-stu-id="ba639-110">"Bring your own device" (BYOD) enrollment lets users enroll their personal phones, tablets, or PCs.</span></span> <span data-ttu-id="ba639-111">企业拥有设备 (COD) 注册允许管理场景，例如远程擦除、共享设备或设备的用户相关性。</span><span class="sxs-lookup"><span data-stu-id="ba639-111">Corporate-owned device (COD) enrollment enables management scenarios like remote wipe, shared devices, or user affinity for a device.</span></span>

<span data-ttu-id="ba639-112">以下 Graph 资源可用于在 Intune 中管理注册：</span><span class="sxs-lookup"><span data-stu-id="ba639-112">The following Graph resources are available to manage enrollment in Intune:</span></span>

- [<span data-ttu-id="ba639-113">证书连接器设置</span><span class="sxs-lookup"><span data-stu-id="ba639-113">Certificate connector setting</span></span>](intune-onboarding-certificateconnectorsetting.md)
- [<span data-ttu-id="ba639-114">设备和应用管理数据</span><span class="sxs-lookup"><span data-stu-id="ba639-114">Device and app management data</span></span>](intune-onboarding-deviceandappmanagementdata.md)
- [<span data-ttu-id="ba639-115">设备注册配置</span><span class="sxs-lookup"><span data-stu-id="ba639-115">Device enrollment configuration</span></span>](intune-onboarding-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="ba639-116">设备注册限制配置</span><span class="sxs-lookup"><span data-stu-id="ba639-116">Device enrollment limit configuration</span></span>](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [<span data-ttu-id="ba639-117">设备注册平台限制</span><span class="sxs-lookup"><span data-stu-id="ba639-117">Device enrollment platform restriction</span></span>](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [<span data-ttu-id="ba639-118">设备注册平台限制配置</span><span class="sxs-lookup"><span data-stu-id="ba639-118">Device enrollment platform restrictions configuration</span></span>](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [<span data-ttu-id="ba639-119">设备注册 Windows Hello 企业版配置</span><span class="sxs-lookup"><span data-stu-id="ba639-119">Device enrollment Windows Hello for business configuration</span></span>](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [<span data-ttu-id="ba639-120">设备管理 Exchange 访问级别</span><span class="sxs-lookup"><span data-stu-id="ba639-120">Device management exchange access level</span></span>](intune-onboarding-devicemanagementexchangeaccesslevel.md)
- [<span data-ttu-id="ba639-121">设备管理 Exchange 访问规则</span><span class="sxs-lookup"><span data-stu-id="ba639-121">Device management exchange access rule</span></span>](intune-onboarding-devicemanagementexchangeaccessrule.md)
- [<span data-ttu-id="ba639-122">设备管理 Exchange 访问规则类型</span><span class="sxs-lookup"><span data-stu-id="ba639-122">Device management exchange access rule type</span></span>](intune-onboarding-devicemanagementexchangeaccessruletype.md)
- [<span data-ttu-id="ba639-123">设备管理 Exchange 连接器</span><span class="sxs-lookup"><span data-stu-id="ba639-123">Device management exchange connector</span></span>](intune-onboarding-devicemanagementexchangeconnector.md)
- [<span data-ttu-id="ba639-124">设备管理 Exchange 连接器状态</span><span class="sxs-lookup"><span data-stu-id="ba639-124">Device management exchange connector status</span></span>](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [<span data-ttu-id="ba639-125">设备管理 Exchange 连接器同步类型</span><span class="sxs-lookup"><span data-stu-id="ba639-125">Device management exchange connector sync type</span></span>](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [<span data-ttu-id="ba639-126">设备管理 Exchange 连接器类型</span><span class="sxs-lookup"><span data-stu-id="ba639-126">Device management exchange connector type</span></span>](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [<span data-ttu-id="ba639-127">设备管理 Exchange 设备类</span><span class="sxs-lookup"><span data-stu-id="ba639-127">Device management exchange device class</span></span>](intune-onboarding-devicemanagementexchangedeviceclass.md)
- [<span data-ttu-id="ba639-128">设备管理 Exchange 本地策略</span><span class="sxs-lookup"><span data-stu-id="ba639-128">Device management exchange on-premises policy</span></span>](intune-onboarding-devicemanagementexchangeonpremisespolicy.md)
- [<span data-ttu-id="ba639-129">设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="ba639-129">Device management partner</span></span>](intune-onboarding-devicemanagementpartner.md)
- [<span data-ttu-id="ba639-130">设备管理合作伙伴应用类型</span><span class="sxs-lookup"><span data-stu-id="ba639-130">Device management partner app type</span></span>](intune-onboarding-devicemanagementpartnerapptype.md)
- [<span data-ttu-id="ba639-131">设备管理合作伙伴租户状态</span><span class="sxs-lookup"><span data-stu-id="ba639-131">Device management partner tenant state</span></span>](intune-onboarding-devicemanagementpartnertenantstate.md)
- [<span data-ttu-id="ba639-132">注册配置分配</span><span class="sxs-lookup"><span data-stu-id="ba639-132">Enrollment configuration assignment</span></span>](intune-onboarding-enrollmentconfigurationassignment.md)
- [<span data-ttu-id="ba639-133">Intune 品牌</span><span class="sxs-lookup"><span data-stu-id="ba639-133">Intune brand</span></span>](intune-onboarding-intunebrand.md)
- [<span data-ttu-id="ba639-134">MDM 颁发机构</span><span class="sxs-lookup"><span data-stu-id="ba639-134">MDM authority</span></span>](intune-onboarding-mdmauthority.md)
- [<span data-ttu-id="ba639-135">适用于企业的 Microsoft Store 门户选定内容的选项</span><span class="sxs-lookup"><span data-stu-id="ba639-135">Microsoft store for business portal selection options</span></span>](intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)
- [<span data-ttu-id="ba639-136">移动威胁防护连接器</span><span class="sxs-lookup"><span data-stu-id="ba639-136">Mobile threat defense connector</span></span>](intune-onboarding-mobilethreatdefenseconnector.md)
- [<span data-ttu-id="ba639-137">移动威胁合作伙伴租户状态</span><span class="sxs-lookup"><span data-stu-id="ba639-137">Mobile threat partner tenant state</span></span>](intune-onboarding-mobilethreatpartnertenantstate.md)
- [<span data-ttu-id="ba639-138">本地条件访问设置</span><span class="sxs-lookup"><span data-stu-id="ba639-138">On-premises conditional access settings</span></span>](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [<span data-ttu-id="ba639-139">组织</span><span class="sxs-lookup"><span data-stu-id="ba639-139">Organization</span></span>](intune-onboarding-organization.md)
- [<span data-ttu-id="ba639-140">侧加载密钥</span><span class="sxs-lookup"><span data-stu-id="ba639-140">Side loading key</span></span>](intune-onboarding-sideloadingkey.md)
- [<span data-ttu-id="ba639-141">VPP 令牌</span><span class="sxs-lookup"><span data-stu-id="ba639-141">VPP token</span></span>](intune-onboarding-vpptoken.md)
- [<span data-ttu-id="ba639-142">VPP 令牌操作结果</span><span class="sxs-lookup"><span data-stu-id="ba639-142">VPP token action result</span></span>](intune-onboarding-vpptokenactionresult.md)
- [<span data-ttu-id="ba639-143">VPP 令牌许可证摘要</span><span class="sxs-lookup"><span data-stu-id="ba639-143">VPP token license summary</span></span>](intune-onboarding-vpptokenlicensesummary.md)
- [<span data-ttu-id="ba639-144">VPP 令牌撤销许可证操作结果</span><span class="sxs-lookup"><span data-stu-id="ba639-144">VPP token revoke licenses action result</span></span>](intune-onboarding-vpptokenrevokelicensesactionresult.md)
- [<span data-ttu-id="ba639-145">VPP 令牌状态</span><span class="sxs-lookup"><span data-stu-id="ba639-145">VPP token state</span></span>](intune-onboarding-vpptokenstate.md)
- [<span data-ttu-id="ba639-146">VPP 令牌同步状态</span><span class="sxs-lookup"><span data-stu-id="ba639-146">VPP token sync status</span></span>](intune-onboarding-vpptokensyncstatus.md)
- [<span data-ttu-id="ba639-147">Windows 10 注册完成页配置</span><span class="sxs-lookup"><span data-stu-id="ba639-147">Windows 10 enrollment completion page configuration</span></span>](intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)
- [<span data-ttu-id="ba639-148">Windows Hello 企业版 PIN 使用情况</span><span class="sxs-lookup"><span data-stu-id="ba639-148">Windows Hello for business PIN usage</span></span>](intune-onboarding-windowshelloforbusinesspinusage.md)
