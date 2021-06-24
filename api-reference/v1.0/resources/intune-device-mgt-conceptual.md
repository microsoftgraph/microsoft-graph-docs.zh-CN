---
title: Microsoft Intune 中的设备管理
description: 设备管理资源Microsoft Intune
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 4bd1f7dacae60fd13c1e2911e71ef7308f0b2764
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108927"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="e3ba8-103">Microsoft Intune 中的设备管理</span><span class="sxs-lookup"><span data-stu-id="e3ba8-103">Device management in Microsoft Intune</span></span>

<span data-ttu-id="e3ba8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3ba8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3ba8-105">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户 [正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e3ba8-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="e3ba8-106">操作状态</span><span class="sxs-lookup"><span data-stu-id="e3ba8-106">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="e3ba8-107">Apple 推送通知证书</span><span class="sxs-lookup"><span data-stu-id="e3ba8-107">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="e3ba8-108">审核主角</span><span class="sxs-lookup"><span data-stu-id="e3ba8-108">Audit actor</span></span>](intune-auditing-auditactor.md)
- [<span data-ttu-id="e3ba8-109">审核事件</span><span class="sxs-lookup"><span data-stu-id="e3ba8-109">Audit event</span></span>](intune-auditing-auditevent.md)
- [<span data-ttu-id="e3ba8-110">审核属性</span><span class="sxs-lookup"><span data-stu-id="e3ba8-110">Audit property</span></span>](intune-auditing-auditproperty.md)
- [<span data-ttu-id="e3ba8-111">审核资源</span><span class="sxs-lookup"><span data-stu-id="e3ba8-111">Audit resource</span></span>](intune-auditing-auditresource.md)
- [<span data-ttu-id="e3ba8-112">合规性状态</span><span class="sxs-lookup"><span data-stu-id="e3ba8-112">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="e3ba8-113">配置管理器客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="e3ba8-113">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="e3ba8-114">从共享 Apple 设备删除用户操作结果</span><span class="sxs-lookup"><span data-stu-id="e3ba8-114">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="e3ba8-115">检测到的应用</span><span class="sxs-lookup"><span data-stu-id="e3ba8-115">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="e3ba8-116">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="e3ba8-116">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="e3ba8-117">设备类别</span><span class="sxs-lookup"><span data-stu-id="e3ba8-117">Device category</span></span>](intune-devices-devicecategory.md)
- [<span data-ttu-id="e3ba8-118">设备注册类型</span><span class="sxs-lookup"><span data-stu-id="e3ba8-118">Device enrollment type</span></span>](intune-devices-deviceenrollmenttype.md)
- [<span data-ttu-id="e3ba8-119">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="e3ba8-119">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="e3ba8-120">设备地理位置</span><span class="sxs-lookup"><span data-stu-id="e3ba8-120">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="e3ba8-121">设备运行状况证明状态</span><span class="sxs-lookup"><span data-stu-id="e3ba8-121">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="e3ba8-122">设备管理</span><span class="sxs-lookup"><span data-stu-id="e3ba8-122">Device management</span></span>](intune-auditing-devicemanagement.md)
- [<span data-ttu-id="e3ba8-123">设备管理</span><span class="sxs-lookup"><span data-stu-id="e3ba8-123">Device management</span></span>](intune-auditing-devicemanagement.md)
- [<span data-ttu-id="e3ba8-124">设备管理</span><span class="sxs-lookup"><span data-stu-id="e3ba8-124">Device management</span></span>](intune-auditing-devicemanagement.md)
- [<span data-ttu-id="e3ba8-125">设备管理</span><span class="sxs-lookup"><span data-stu-id="e3ba8-125">Device management</span></span>](intune-auditing-devicemanagement.md)
- [<span data-ttu-id="e3ba8-126">设备管理 Exchange 访问状态</span><span class="sxs-lookup"><span data-stu-id="e3ba8-126">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="e3ba8-127">设备管理 Exchange 访问状态原因</span><span class="sxs-lookup"><span data-stu-id="e3ba8-127">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="e3ba8-128">设备管理订阅状态</span><span class="sxs-lookup"><span data-stu-id="e3ba8-128">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="e3ba8-129">设备操作系统摘要</span><span class="sxs-lookup"><span data-stu-id="e3ba8-129">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="e3ba8-130">设备注册状态</span><span class="sxs-lookup"><span data-stu-id="e3ba8-130">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="e3ba8-131">已本地化的通知邮件</span><span class="sxs-lookup"><span data-stu-id="e3ba8-131">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="e3ba8-132">查找设备操作结果</span><span class="sxs-lookup"><span data-stu-id="e3ba8-132">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="e3ba8-133">托管设备</span><span class="sxs-lookup"><span data-stu-id="e3ba8-133">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="e3ba8-134">托管设备概述</span><span class="sxs-lookup"><span data-stu-id="e3ba8-134">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="e3ba8-135">托管的设备所有者类型</span><span class="sxs-lookup"><span data-stu-id="e3ba8-135">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="e3ba8-136">托管的设备合作伙伴报告的运行状况</span><span class="sxs-lookup"><span data-stu-id="e3ba8-136">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="e3ba8-137">管理代理类型</span><span class="sxs-lookup"><span data-stu-id="e3ba8-137">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="e3ba8-138">通知邮件模板</span><span class="sxs-lookup"><span data-stu-id="e3ba8-138">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="e3ba8-139">通知模板品牌选项</span><span class="sxs-lookup"><span data-stu-id="e3ba8-139">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="e3ba8-140">平台类型</span><span class="sxs-lookup"><span data-stu-id="e3ba8-140">Platform type</span></span>](intune-esim-platformtype.md)
- [<span data-ttu-id="e3ba8-141">远程协助载入状态</span><span class="sxs-lookup"><span data-stu-id="e3ba8-141">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="e3ba8-142">远程协助合作伙伴</span><span class="sxs-lookup"><span data-stu-id="e3ba8-142">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="e3ba8-143">远程锁定操作结果</span><span class="sxs-lookup"><span data-stu-id="e3ba8-143">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="e3ba8-144">重置密码操作结果</span><span class="sxs-lookup"><span data-stu-id="e3ba8-144">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="e3ba8-145">Tuple_2操作type_collection_1执行顺序</span><span class="sxs-lookup"><span data-stu-id="e3ba8-145">Tuple_2 of execution type_ i collection_1 of operation</span></span>](intune-esim-tuple_2ofexecutiontype_icollection_1ofoperation.md)
- [<span data-ttu-id="e3ba8-146">更新 Windows 设备帐户操作参数</span><span class="sxs-lookup"><span data-stu-id="e3ba8-146">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="e3ba8-147">用户</span><span class="sxs-lookup"><span data-stu-id="e3ba8-147">User</span></span>](intune-devices-user.md)
- [<span data-ttu-id="e3ba8-148">Windows Defender 扫描操作结果</span><span class="sxs-lookup"><span data-stu-id="e3ba8-148">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="e3ba8-149">Windows 设备帐户</span><span class="sxs-lookup"><span data-stu-id="e3ba8-149">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="e3ba8-150">Windows 设备 AD 帐户</span><span class="sxs-lookup"><span data-stu-id="e3ba8-150">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="e3ba8-151">Windows 设备 Azure AD 帐户</span><span class="sxs-lookup"><span data-stu-id="e3ba8-151">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)