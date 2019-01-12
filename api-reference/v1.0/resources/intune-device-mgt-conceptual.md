---
title: Microsoft Intune 中的设备管理
description: ''
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3d665b70f812a18f840ce43a029fe0729d454745
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980641"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="47f76-102">Microsoft Intune 中的设备管理</span><span class="sxs-lookup"><span data-stu-id="47f76-102">Device management in Microsoft Intune</span></span>

> <span data-ttu-id="47f76-103">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="47f76-103">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="47f76-104">操作状态</span><span class="sxs-lookup"><span data-stu-id="47f76-104">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="47f76-105">Apple 推送通知证书</span><span class="sxs-lookup"><span data-stu-id="47f76-105">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="47f76-106">审核主角</span><span class="sxs-lookup"><span data-stu-id="47f76-106">Audit actor</span></span>](intune-auditing-auditactor.md)
- [<span data-ttu-id="47f76-107">审核事件</span><span class="sxs-lookup"><span data-stu-id="47f76-107">Audit event</span></span>](intune-auditing-auditevent.md)
- [<span data-ttu-id="47f76-108">审核属性</span><span class="sxs-lookup"><span data-stu-id="47f76-108">Audit property</span></span>](intune-auditing-auditproperty.md)
- [<span data-ttu-id="47f76-109">审核资源</span><span class="sxs-lookup"><span data-stu-id="47f76-109">Audit resource</span></span>](intune-auditing-auditresource.md)
- [<span data-ttu-id="47f76-110">合规性状态</span><span class="sxs-lookup"><span data-stu-id="47f76-110">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="47f76-111">配置管理器客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="47f76-111">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="47f76-112">从共享 Apple 设备删除用户操作结果</span><span class="sxs-lookup"><span data-stu-id="47f76-112">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="47f76-113">检测到的应用</span><span class="sxs-lookup"><span data-stu-id="47f76-113">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="47f76-114">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="47f76-114">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="47f76-115">设备注册失败原因</span><span class="sxs-lookup"><span data-stu-id="47f76-115">Device enrollment failure reason</span></span>](intune-troubleshooting-deviceenrollmentfailurereason.md)
- [<span data-ttu-id="47f76-116">设备注册类型</span><span class="sxs-lookup"><span data-stu-id="47f76-116">Device enrollment type</span></span>](intune-devices-deviceenrollmenttype.md)
- [<span data-ttu-id="47f76-117">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="47f76-117">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="47f76-118">设备地理位置</span><span class="sxs-lookup"><span data-stu-id="47f76-118">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="47f76-119">设备运行状况证明状态</span><span class="sxs-lookup"><span data-stu-id="47f76-119">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="47f76-120">设备管理 exchange 访问状态</span><span class="sxs-lookup"><span data-stu-id="47f76-120">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="47f76-121">设备管理 exchange 访问状态的原因</span><span class="sxs-lookup"><span data-stu-id="47f76-121">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="47f76-122">设备管理订阅状态</span><span class="sxs-lookup"><span data-stu-id="47f76-122">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="47f76-123">设备管理疑难解答事件</span><span class="sxs-lookup"><span data-stu-id="47f76-123">Device management troubleshooting event</span></span>](intune-troubleshooting-devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="47f76-124">设备操作系统摘要</span><span class="sxs-lookup"><span data-stu-id="47f76-124">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="47f76-125">设备注册状态</span><span class="sxs-lookup"><span data-stu-id="47f76-125">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="47f76-126">注册疑难解答事件</span><span class="sxs-lookup"><span data-stu-id="47f76-126">Enrollment troubleshooting event</span></span>](intune-troubleshooting-enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="47f76-127">已本地化的通知邮件</span><span class="sxs-lookup"><span data-stu-id="47f76-127">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="47f76-128">查找设备操作结果</span><span class="sxs-lookup"><span data-stu-id="47f76-128">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="47f76-129">受管理设备</span><span class="sxs-lookup"><span data-stu-id="47f76-129">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="47f76-130">托管设备概述</span><span class="sxs-lookup"><span data-stu-id="47f76-130">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="47f76-131">管理设备所有者类型</span><span class="sxs-lookup"><span data-stu-id="47f76-131">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="47f76-132">托管的设备伙伴报告健康状态</span><span class="sxs-lookup"><span data-stu-id="47f76-132">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="47f76-133">管理代理类型</span><span class="sxs-lookup"><span data-stu-id="47f76-133">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="47f76-134">通知邮件模板</span><span class="sxs-lookup"><span data-stu-id="47f76-134">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="47f76-135">通知模板品牌选项</span><span class="sxs-lookup"><span data-stu-id="47f76-135">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="47f76-136">远程协助的白板状态</span><span class="sxs-lookup"><span data-stu-id="47f76-136">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="47f76-137">远程协助合作伙伴</span><span class="sxs-lookup"><span data-stu-id="47f76-137">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="47f76-138">远程锁定操作结果</span><span class="sxs-lookup"><span data-stu-id="47f76-138">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="47f76-139">重置密码操作结果</span><span class="sxs-lookup"><span data-stu-id="47f76-139">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="47f76-140">更新 Windows 设备帐户操作参数</span><span class="sxs-lookup"><span data-stu-id="47f76-140">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="47f76-141">Windows Defender 扫描操作结果</span><span class="sxs-lookup"><span data-stu-id="47f76-141">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="47f76-142">Windows 设备帐户</span><span class="sxs-lookup"><span data-stu-id="47f76-142">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="47f76-143">Windows 设备 AD 帐户</span><span class="sxs-lookup"><span data-stu-id="47f76-143">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="47f76-144">Windows 设备 Azure AD 帐户</span><span class="sxs-lookup"><span data-stu-id="47f76-144">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)
