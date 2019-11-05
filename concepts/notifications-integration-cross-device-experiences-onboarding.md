---
title: '载入跨设备 Microsoft Graph 通知体验 '
description: 在 Windows 开发人员中心注册应用程序，使应用客户端接收通过 Microsoft Graph 发送的跨设备通知。
localization_priority: Priority
ms.prod: notifications
author: merzink
ms.openlocfilehash: 7cfbbdc61b0e473b7aa1401c8f48a3fd0c828928
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939647"
---
# <a name="onboarding-to-cross-device-experiences-for-microsoft-graph-notifications"></a><span data-ttu-id="27929-103">载入跨设备 Microsoft Graph 通知体验</span><span class="sxs-lookup"><span data-stu-id="27929-103">Onboarding to cross-device experiences for Microsoft Graph notifications</span></span>

>[!NOTE]
><span data-ttu-id="27929-104">如果仅针对 Web 终结点，则可以直接转到设置[应用服务](notifications-integrating-app-server.md)以发送通知。</span><span class="sxs-lookup"><span data-stu-id="27929-104">If you're only targeting web endpoints, you can go directly to setting up your [app service](notifications-integrating-app-server.md) to send notifications.</span></span>

<span data-ttu-id="27929-105">除了[在 Azure 门户上注册应用](notifications-integration-app-registration.md)外，应用程序还需要登记跨设备信息，如跨平台应用程序 ID 和跨平台推送凭据，以授权 Microsoft Graph 通过预每个操作系统（Windows、iOS 和 Android）对应的本机推送通知服务发送通知。</span><span class="sxs-lookup"><span data-stu-id="27929-105">In addition to [app registration on Azure Portal](notifications-integration-app-registration.md), your application needs to register cross-device information such as cross-platform application id and cross-platform push credentials in order to authorizes Microsoft Graph to send notifications via native push notification services that correspond to each operating system: Windows, iOS, and Android.</span></span> <span data-ttu-id="27929-106">这可通过[合作伙伴中心仪表板（先前的 Windows 开发人员中心仪表板）](https://partner.microsoft.com/dashboard/)完成。</span><span class="sxs-lookup"><span data-stu-id="27929-106">This is done through [Partner Center dashboard (formerly Windows Dev Center dashboard)](https://partner.microsoft.com/dashboard/).</span></span> 

> [!NOTE]
> <span data-ttu-id="27929-107">即使不打算构建 Windows UWP 应用程序，你也需要 Windows 开发人员帐户来完成本文中的步骤。</span><span class="sxs-lookup"><span data-stu-id="27929-107">You'll need a Windows developer account to complete the steps in this article, even if you don’t plan to build a Windows UWP application.</span></span> <span data-ttu-id="27929-108">如果没有 Windows 开发人员帐户，请参阅[开立开发人员账户](https://docs.microsoft.com/windows/uwp/publish/opening-a-developer-account)。</span><span class="sxs-lookup"><span data-stu-id="27929-108">If you don’t already have a Windows developer account, see [Opening a developer account](https://docs.microsoft.com/windows/uwp/publish/opening-a-developer-account).</span></span> <span data-ttu-id="27929-109">或者，如果不希望注册为 Windows 开发人员，可通过电子邮件 [gnsengage@microsoft.com](sendto: gnsengage@microsoft.com) 联系我们。</span><span class="sxs-lookup"><span data-stu-id="27929-109">Alternatively, if you prefer not to enroll as a Windows developer, you can reach out to us via email at [gnsengage@microsoft.com](sendto: gnsengage@microsoft.com).</span></span> <span data-ttu-id="27929-110">如果创建 Windows 开发人员帐户且将学校或工作应用程序构建为企业的一部分，则可以将开发人员帐户与用于管理企业提交的相应 Azure AD 帐户关联在一起。</span><span class="sxs-lookup"><span data-stu-id="27929-110">If you’re building a school or work application as part of an enterprise, you can associate your developer account with the appropriate Azure AD account that is used for managing your enterprise submissions.</span></span> <span data-ttu-id="27929-111">有关详细信息，请参阅[关联 Azure Active Directory 与合作伙伴中心帐户](https://docs.microsoft.com/windows/uwp/publish/associate-azure-ad-with-partner-center)。</span><span class="sxs-lookup"><span data-stu-id="27929-111">For details, see [Associate Azure Active Directory with your Partner Center account](https://docs.microsoft.com/windows/uwp/publish/associate-azure-ad-with-partner-center).</span></span>

<span data-ttu-id="27929-112">若要开始使用，请使用 Windows 开发人员帐户登录[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard)：</span><span class="sxs-lookup"><span data-stu-id="27929-112">To get started, sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard) using your Windows developer account (you cannot use an Azure AD account):</span></span>

1.  <span data-ttu-id="27929-113">在左侧菜单上，转至“**跨设备体验**”，选择“**配置新的跨设备应用**”，然后提供应用名称，如下面的屏幕截图所示。</span><span class="sxs-lookup"><span data-stu-id="27929-113">On the left menu, go to **Cross-Device Experiences**, select **Configuring a new cross-device app**, and provide your app name, as shown in the following screenshot.</span></span>

![配置新的跨设备应用注册](images/notifications-crossdevice-new-configure.png)

2.  <span data-ttu-id="27929-115">选择应用具有状态且可以接收通知的所有受支持平台。</span><span class="sxs-lookup"><span data-stu-id="27929-115">Select all supported platforms where your app will have a presence and be enabled to receive notifications.</span></span> <span data-ttu-id="27929-116">可以从受支持平台（包括 Windows、Android 和 iOS）中进行选择，如图所示。</span><span class="sxs-lookup"><span data-stu-id="27929-116">You can select from supported platforms that include Windows, Android, and iOS, as shown.</span></span> 

![设置受支持的平台类型](images/notifications-crossdevice-supported-platforms.png)

3.  <span data-ttu-id="27929-118">为应用具有状态的每个平台提供应用 ID，如图所示。</span><span class="sxs-lookup"><span data-stu-id="27929-118">Provide app IDs for each of the platforms where your app has a presence, as shown.</span></span>

 ![提供平台特定的应用 ID](images/notifications-crossdevice-platform-appids.png)

> [!NOTE] 
> <span data-ttu-id="27929-120">可以为每个平台添加不同 ID（最多十个） – 这是为了以防同一应用的多个版本或者不同应用希望接收由应用服务器发送的针对相同用户的相同通知。</span><span class="sxs-lookup"><span data-stu-id="27929-120">You can add different IDs (up to ten) per platform – this is in case you have multiple versions of the same app, or even different apps, that want to be able to receive the same notification sent by your app server and targeted to the same user.</span></span>

4.  <span data-ttu-id="27929-121">从 Microsoft 帐户和/或 Azure AD 应用注册提供或选择应用 ID。</span><span class="sxs-lookup"><span data-stu-id="27929-121">Provide or select the app ID from Microsoft account and/or Azure AD app registration.</span></span> <span data-ttu-id="27929-122">此客户端 ID 对应于 Microsoft 帐户或在 Azure 门户中注册时获取的 Azure AD 应用注册。</span><span class="sxs-lookup"><span data-stu-id="27929-122">This client ID corresponds to the Microsoft account or Azure AD app registration that you obtained when you register in the Azure Portal.</span></span>

![为 MSA 和 AAD 提供 Azure 应用注册客户端 ID](images/notifications-crossdevice-azureportal-clientid.png)

5.  <span data-ttu-id="27929-124">Microsoft Graph 通知使用所有主要平台上的各个本机通知平台向应用客户端终结点（也就是 WNS - Windows UWP、FCM - Android 和 APNS - iOS）发送通知。</span><span class="sxs-lookup"><span data-stu-id="27929-124">Microsoft Graph notifications use each of the native notification platforms on all major platforms to send notifications to the app client endpoints, namely, WNS (for Windows UWP), FCM (for Android), and APNS (for iOS).</span></span> <span data-ttu-id="27929-125">提供这些通知平台的凭据，使 Microsoft Graph 通知在你发布针对用户的通知时传递应用服务器通知，如图所示。</span><span class="sxs-lookup"><span data-stu-id="27929-125">Provide your credentials for these notification platforms to enable Microsoft Graph notifications to deliver notifications for your app server when you publish user-targeted notifications, as shown.</span></span>

 ![提供跨设备推送凭据](images/notifications-crossdevice-push-cred.png)

> [!NOTE]
> <span data-ttu-id="27929-127">对于 Windows UWP 应用，启用 WNS 推送通知是使用 Microsoft Graph 通知的前提条件。</span><span class="sxs-lookup"><span data-stu-id="27929-127">For Windows UWP apps, enabling WNS push notification is a prerequisite to using Microsoft Graph notifications.</span></span> <span data-ttu-id="27929-128">有关详细信息，请查阅 [WNS 概述](https://docs.microsoft.com/windows/uwp/design/shell/tiles-and-notifications/windows-push-notification-services--wns--overview)。</span><span class="sxs-lookup"><span data-stu-id="27929-128">For details, see [WNS overview](https://docs.microsoft.com/windows/uwp/design/shell/tiles-and-notifications/windows-push-notification-services--wns--overview).</span></span> <span data-ttu-id="27929-129">载入后，可以通过合作伙伴中心向连接设备平台提供推送凭据。</span><span class="sxs-lookup"><span data-stu-id="27929-129">After you onboard, you can provide push credentials via Partner Center to the Connected Device Platform.</span></span>

6.  <span data-ttu-id="27929-130">验证跨设备应用域，这将用作验证流程以证明你的应用程序拥有此域的所有权。</span><span class="sxs-lookup"><span data-stu-id="27929-130">Verify your cross-device app domain, which serves as a verification process to prove that your application has ownership of this domain.</span></span> <span data-ttu-id="27929-131">这就好比所注册的应用的跨设备应用标识，如图所示。</span><span class="sxs-lookup"><span data-stu-id="27929-131">This acts like a cross-device app identity for the application or applications you registered, as shown.</span></span>
    
    ![验证域](images/notifications-crossdevice-domain-verify.png)

<span data-ttu-id="27929-133">搞定！</span><span class="sxs-lookup"><span data-stu-id="27929-133">That’s it!</span></span> <span data-ttu-id="27929-134">你现在已注册应用程序以接收通知。</span><span class="sxs-lookup"><span data-stu-id="27929-134">You've now registered your applications to receive notifications.</span></span> <span data-ttu-id="27929-135">接下来，了解如何设置[应用服务](notifications-integrating-app-server.md)并开始发送通知。</span><span class="sxs-lookup"><span data-stu-id="27929-135">Next, learn how to set up your [app service](notifications-integrating-app-server.md) and start sending notifications.</span></span>
