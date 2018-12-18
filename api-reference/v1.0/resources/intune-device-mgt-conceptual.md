---
title: Microsoft Intune 中的设备管理
description: ''
author: tfitzmac
ms.openlocfilehash: 3672513defc25d63e18e7432c3883340d31ae264
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341564"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="8c8a6-102">Microsoft Intune 中的设备管理</span><span class="sxs-lookup"><span data-stu-id="8c8a6-102">Device management in Microsoft Intune</span></span>

> <span data-ttu-id="8c8a6-103">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8c8a6-103">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="8c8a6-104">操作状态</span><span class="sxs-lookup"><span data-stu-id="8c8a6-104">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="8c8a6-105">Apple 推送通知证书</span><span class="sxs-lookup"><span data-stu-id="8c8a6-105">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="8c8a6-106">审核主角</span><span class="sxs-lookup"><span data-stu-id="8c8a6-106">Audit actor</span></span>](intune-auditing-auditactor.md)
- [<span data-ttu-id="8c8a6-107">审核事件</span><span class="sxs-lookup"><span data-stu-id="8c8a6-107">Audit event</span></span>](intune-auditing-auditevent.md)
- [<span data-ttu-id="8c8a6-108">审核属性</span><span class="sxs-lookup"><span data-stu-id="8c8a6-108">Audit property</span></span>](intune-auditing-auditproperty.md)
- [<span data-ttu-id="8c8a6-109">审核资源</span><span class="sxs-lookup"><span data-stu-id="8c8a6-109">Audit resource</span></span>](intune-auditing-auditresource.md)
- [<span data-ttu-id="8c8a6-110">合规性状态</span><span class="sxs-lookup"><span data-stu-id="8c8a6-110">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="8c8a6-111">配置管理器客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="8c8a6-111">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="8c8a6-112">从共享 Apple 设备删除用户操作结果</span><span class="sxs-lookup"><span data-stu-id="8c8a6-112">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="8c8a6-113">检测到的应用</span><span class="sxs-lookup"><span data-stu-id="8c8a6-113">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="8c8a6-114">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="8c8a6-114">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="8c8a6-115">设备注册失败原因</span><span class="sxs-lookup"><span data-stu-id="8c8a6-115">Device enrollment failure reason</span></span>](intune-troubleshooting-deviceenrollmentfailurereason.md)
- [<span data-ttu-id="8c8a6-116">设备注册类型</span><span class="sxs-lookup"><span data-stu-id="8c8a6-116">Device enrollment type</span></span>](intune-devices-deviceenrollmenttype.md)
- [<span data-ttu-id="8c8a6-117">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="8c8a6-117">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="8c8a6-118">设备地理位置</span><span class="sxs-lookup"><span data-stu-id="8c8a6-118">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="8c8a6-119">设备运行状况证明状态</span><span class="sxs-lookup"><span data-stu-id="8c8a6-119">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="8c8a6-120">设备管理 exchange 访问状态</span><span class="sxs-lookup"><span data-stu-id="8c8a6-120">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="8c8a6-121">设备管理 exchange 访问状态的原因</span><span class="sxs-lookup"><span data-stu-id="8c8a6-121">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="8c8a6-122">设备管理订阅状态</span><span class="sxs-lookup"><span data-stu-id="8c8a6-122">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="8c8a6-123">设备管理疑难解答事件</span><span class="sxs-lookup"><span data-stu-id="8c8a6-123">Device management troubleshooting event</span></span>](intune-troubleshooting-devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="8c8a6-124">设备操作系统摘要</span><span class="sxs-lookup"><span data-stu-id="8c8a6-124">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="8c8a6-125">设备注册状态</span><span class="sxs-lookup"><span data-stu-id="8c8a6-125">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="8c8a6-126">注册疑难解答事件</span><span class="sxs-lookup"><span data-stu-id="8c8a6-126">Enrollment troubleshooting event</span></span>](intune-troubleshooting-enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="8c8a6-127">已本地化的通知邮件</span><span class="sxs-lookup"><span data-stu-id="8c8a6-127">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="8c8a6-128">查找设备操作结果</span><span class="sxs-lookup"><span data-stu-id="8c8a6-128">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="8c8a6-129">受管理设备</span><span class="sxs-lookup"><span data-stu-id="8c8a6-129">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="8c8a6-130">托管设备概述</span><span class="sxs-lookup"><span data-stu-id="8c8a6-130">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="8c8a6-131">管理设备所有者类型</span><span class="sxs-lookup"><span data-stu-id="8c8a6-131">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="8c8a6-132">托管的设备伙伴报告健康状态</span><span class="sxs-lookup"><span data-stu-id="8c8a6-132">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="8c8a6-133">管理代理类型</span><span class="sxs-lookup"><span data-stu-id="8c8a6-133">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="8c8a6-134">通知邮件模板</span><span class="sxs-lookup"><span data-stu-id="8c8a6-134">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="8c8a6-135">通知模板品牌选项</span><span class="sxs-lookup"><span data-stu-id="8c8a6-135">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="8c8a6-136">远程协助的白板状态</span><span class="sxs-lookup"><span data-stu-id="8c8a6-136">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="8c8a6-137">远程协助合作伙伴</span><span class="sxs-lookup"><span data-stu-id="8c8a6-137">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="8c8a6-138">远程锁定操作结果</span><span class="sxs-lookup"><span data-stu-id="8c8a6-138">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="8c8a6-139">重置密码操作结果</span><span class="sxs-lookup"><span data-stu-id="8c8a6-139">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="8c8a6-140">更新 Windows 设备帐户操作参数</span><span class="sxs-lookup"><span data-stu-id="8c8a6-140">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="8c8a6-141">Windows Defender 扫描操作结果</span><span class="sxs-lookup"><span data-stu-id="8c8a6-141">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="8c8a6-142">Windows 设备帐户</span><span class="sxs-lookup"><span data-stu-id="8c8a6-142">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="8c8a6-143">Windows 设备 AD 帐户</span><span class="sxs-lookup"><span data-stu-id="8c8a6-143">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="8c8a6-144">Windows 设备 Azure AD 帐户</span><span class="sxs-lookup"><span data-stu-id="8c8a6-144">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)
