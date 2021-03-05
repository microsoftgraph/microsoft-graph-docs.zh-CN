---
title: Microsoft Intune 中的设备管理
description: Microsoft Intune 中的设备管理资源
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 80c643d4d1c75c27df35a85a576f93838dd03554
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472340"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="d5451-103">Microsoft Intune 中的设备管理</span><span class="sxs-lookup"><span data-stu-id="d5451-103">Device management in Microsoft Intune</span></span>

<span data-ttu-id="d5451-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5451-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5451-105">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户 [正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d5451-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="d5451-106">操作状态</span><span class="sxs-lookup"><span data-stu-id="d5451-106">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="d5451-107">Apple 推送通知证书</span><span class="sxs-lookup"><span data-stu-id="d5451-107">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="d5451-108">合规性状态</span><span class="sxs-lookup"><span data-stu-id="d5451-108">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="d5451-109">配置管理器客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="d5451-109">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="d5451-110">从共享 Apple 设备删除用户操作结果</span><span class="sxs-lookup"><span data-stu-id="d5451-110">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="d5451-111">检测到的应用</span><span class="sxs-lookup"><span data-stu-id="d5451-111">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="d5451-112">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="d5451-112">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="d5451-113">设备注册失败原因</span><span class="sxs-lookup"><span data-stu-id="d5451-113">Device enrollment failure reason</span></span>](intune-troubleshooting-deviceenrollmentfailurereason.md)
- [<span data-ttu-id="d5451-114">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="d5451-114">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="d5451-115">设备地理位置</span><span class="sxs-lookup"><span data-stu-id="d5451-115">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="d5451-116">设备运行状况证明状态</span><span class="sxs-lookup"><span data-stu-id="d5451-116">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="d5451-117">设备管理 Exchange 访问状态</span><span class="sxs-lookup"><span data-stu-id="d5451-117">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="d5451-118">设备管理 Exchange 访问状态原因</span><span class="sxs-lookup"><span data-stu-id="d5451-118">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="d5451-119">设备管理订阅状态</span><span class="sxs-lookup"><span data-stu-id="d5451-119">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="d5451-120">设备管理疑难解答事件</span><span class="sxs-lookup"><span data-stu-id="d5451-120">Device management troubleshooting event</span></span>](intune-troubleshooting-devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="d5451-121">设备操作系统摘要</span><span class="sxs-lookup"><span data-stu-id="d5451-121">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="d5451-122">设备注册状态</span><span class="sxs-lookup"><span data-stu-id="d5451-122">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="d5451-123">注册疑难解答事件</span><span class="sxs-lookup"><span data-stu-id="d5451-123">Enrollment troubleshooting event</span></span>](intune-troubleshooting-enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="d5451-124">已本地化的通知邮件</span><span class="sxs-lookup"><span data-stu-id="d5451-124">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="d5451-125">查找设备操作结果</span><span class="sxs-lookup"><span data-stu-id="d5451-125">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="d5451-126">托管设备</span><span class="sxs-lookup"><span data-stu-id="d5451-126">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="d5451-127">托管设备概述</span><span class="sxs-lookup"><span data-stu-id="d5451-127">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="d5451-128">托管的设备所有者类型</span><span class="sxs-lookup"><span data-stu-id="d5451-128">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="d5451-129">托管的设备合作伙伴报告的运行状况</span><span class="sxs-lookup"><span data-stu-id="d5451-129">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="d5451-130">管理代理类型</span><span class="sxs-lookup"><span data-stu-id="d5451-130">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="d5451-131">通知邮件模板</span><span class="sxs-lookup"><span data-stu-id="d5451-131">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="d5451-132">通知模板品牌选项</span><span class="sxs-lookup"><span data-stu-id="d5451-132">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="d5451-133">远程协助载入状态</span><span class="sxs-lookup"><span data-stu-id="d5451-133">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="d5451-134">远程协助合作伙伴</span><span class="sxs-lookup"><span data-stu-id="d5451-134">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="d5451-135">远程锁定操作结果</span><span class="sxs-lookup"><span data-stu-id="d5451-135">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="d5451-136">重置密码操作结果</span><span class="sxs-lookup"><span data-stu-id="d5451-136">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="d5451-137">更新 Windows 设备帐户操作参数</span><span class="sxs-lookup"><span data-stu-id="d5451-137">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="d5451-138">Windows Defender 扫描操作结果</span><span class="sxs-lookup"><span data-stu-id="d5451-138">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="d5451-139">Windows 设备帐户</span><span class="sxs-lookup"><span data-stu-id="d5451-139">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="d5451-140">Windows 设备 AD 帐户</span><span class="sxs-lookup"><span data-stu-id="d5451-140">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="d5451-141">Windows 设备 Azure AD 帐户</span><span class="sxs-lookup"><span data-stu-id="d5451-141">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)






