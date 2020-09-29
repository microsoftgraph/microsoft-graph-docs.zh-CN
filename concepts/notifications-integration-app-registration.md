---
title: 管理 Microsoft Graph 通知的应用注册和 API 权限
description: 为接收通过 Microsoft Graph 发送的通知，首先需要在 Microsoft Azure 门户上注册应用程序。
localization_priority: Priority
ms.prod: notifications
author: merzink
ms.openlocfilehash: f975c6aebf9fa8a8dc045c4b60e1c4f21ef84c12
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288362"
---
# <a name="manage-app-registration-and-api-permission-for-microsoft-graph-notifications"></a><span data-ttu-id="d45c6-103">管理 Microsoft Graph 通知的应用注册和 API 权限</span><span class="sxs-lookup"><span data-stu-id="d45c6-103">Manage app registration and API permission for Microsoft Graph notifications</span></span>

<span data-ttu-id="d45c6-104">若要让应用程序服务与 Microsoft Graph 通知集成，你需要通过 Microsoft 标识平台注册应用，以支持 Microsoft 帐户或工作或学校帐户，并删除所需的 API 权限。</span><span class="sxs-lookup"><span data-stu-id="d45c6-104">In order for your application service to integrate with Microsoft Graph notifications, you need to register your app with the Microsoft identity platform to support Microsoft accounts or work or school accounts, and declare the API permissions that are required.</span></span>

## <a name="register-your-app-to-support-microsoft-accounts-or-work-or-school-accounts"></a><span data-ttu-id="d45c6-105">注册应用，以支持 Microsoft 帐户或工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="d45c6-105">Register your app to support Microsoft accounts or work or school accounts</span></span>

<span data-ttu-id="d45c6-106">在 [Microsoft Azure 门户](https://portal.azure.com/#home)上注册应用程序，以支持 Microsoft 帐户或工作或学校帐户。</span><span class="sxs-lookup"><span data-stu-id="d45c6-106">Register your application on the [Microsoft Azure portal](https://portal.azure.com/#home) to support Microsoft accounts or work or school accounts.</span></span> <span data-ttu-id="d45c6-107">如果已在 [Microsoft 应用程序门户](https://apps.dev.microsoft.com/)上注册帐户，则现有应用将在新增和改进的 Azure 门户体验中显示。</span><span class="sxs-lookup"><span data-stu-id="d45c6-107">If you’ve previously registered your application on the [Microsoft Application Portal](https://apps.dev.microsoft.com/), your existing apps will show up in the new and improved Azure portal experience.</span></span>

<span data-ttu-id="d45c6-108">有关如何注册应用的信息，请参阅[向 Microsoft 标识平台注册应用程序](auth-register-app-v2.md)。</span><span class="sxs-lookup"><span data-stu-id="d45c6-108">For information about how to register your apps, see [Register an application with the Microsoft identity platform](auth-register-app-v2.md).</span></span> <span data-ttu-id="d45c6-109">注册应用时，请确保将应用程序 ID/客户端 ID 置于方便使用的位置。</span><span class="sxs-lookup"><span data-stu-id="d45c6-109">When you register your app, be sure to keep the application ID/client ID somewhere handy.</span></span> <span data-ttu-id="d45c6-110">后续在适用于 Windows、Android 或 iOS 客户端的[合作伙伴中心](https://partner.microsoft.com/)注册应用程序以获取跨设备体验时，需要此 ID。</span><span class="sxs-lookup"><span data-stu-id="d45c6-110">You'll need this ID later when you register your application for cross-device experiences in [Partner Center](https://partner.microsoft.com/) for Windows, Android, or iOS clients.</span></span>

> [!NOTE]
> <span data-ttu-id="d45c6-111">如果没有 Microsoft 帐户并想要使用此类帐户，请转至  [Microsoft 帐户](https://account.microsoft.com/account)页面。</span><span class="sxs-lookup"><span data-stu-id="d45c6-111">If you don't already have a Microsoft account and would like to use one, go to the [Microsoft account](https://account.microsoft.com/account) page.</span></span> <span data-ttu-id="d45c6-112">如果正在编写需要将 Azure AD v1.0 用作工作或学校帐户的身份验证和标识框架的应用，请参阅  [Azure Active Directory 身份验证库](/azure/active-directory/develop/active-directory-authentication-libraries)。</span><span class="sxs-lookup"><span data-stu-id="d45c6-112">If you're writing an app that needs to use Azure AD v1.0 as an authentication and identity framework for work or school accounts, see [Azure Active Directory Authentication Libraries](/azure/active-directory/develop/active-directory-authentication-libraries).</span></span> <span data-ttu-id="d45c6-113">如果你想了解或使用新聚合的 Microsoft 标识平台 (v2.0)，请参阅[比较 Microsoft 标识平台终结点和 Azure AD v1.0 终结点](/azure/active-directory/develop/azure-ad-endpoint-comparison)。</span><span class="sxs-lookup"><span data-stu-id="d45c6-113">If you’re interested in learning about or using the new converged Microsoft identity platform (v2.0), see [Comparing the Microsoft identity platform endpoint and Azure AD v1.0 endpoint](/azure/active-directory/develop/azure-ad-endpoint-comparison).</span></span>


## <a name="app-certificates-and-secrets"></a><span data-ttu-id="d45c6-114">应用证书和密码</span><span class="sxs-lookup"><span data-stu-id="d45c6-114">App certificates and secrets</span></span>

<span data-ttu-id="d45c6-115">若要使应用程序在获取身份验证令牌时对自己进行标识和身份验证，你可以转至 Azure 门户中的**证书和密码**，以上传自己的证书或创建信的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="d45c6-115">To enable your application to identify and authenticate itself when obtaining auth tokens, you can either upload your own certificate or create a new client secret by going to **Certificates & secrets** in the Azure portal.</span></span>
    
![Azure 门户中的应用证书和密码屏幕截图](images/notifications-app-secrets.png)
    
> [!NOTE]
> <span data-ttu-id="d45c6-117">如果选择生成新的客户端密码，请确保将其复制并保存到安全的位置。</span><span class="sxs-lookup"><span data-stu-id="d45c6-117">If you opt to generate a new client secret, be sure to copy and keep it in a safe place.</span></span> <span data-ttu-id="d45c6-118">离开门户后，你将无法再次访问它。</span><span class="sxs-lookup"><span data-stu-id="d45c6-118">You won’t be able to access it again after you leave the portal.</span></span>

## <a name="api-permissions"></a><span data-ttu-id="d45c6-119">API 权限</span><span class="sxs-lookup"><span data-stu-id="d45c6-119">API permissions</span></span>

<span data-ttu-id="d45c6-120">需要添加其他权限才能使用 Microsoft Graph 通知。</span><span class="sxs-lookup"><span data-stu-id="d45c6-120">You'll need to add additional permissions in order to use Microsoft Graph notifications.</span></span> <span data-ttu-id="d45c6-121">选择“**添加权限**”，在 Microsoft API 下，选择“**Microsoft Graph**”，然后选择“**委派权限**”。</span><span class="sxs-lookup"><span data-stu-id="d45c6-121">Choose **Add a permission**, and under Microsoft APIs, select **Microsoft Graph**, and then select **Delegated permissions**.</span></span>
    
![Azure 门户的请求 API 权限页面的屏幕截图](images/notifications-api-permissions.png)
    
<span data-ttu-id="d45c6-123">添加以下权限：</span><span class="sxs-lookup"><span data-stu-id="d45c6-123">Add the following permissions:</span></span>

- <span data-ttu-id="d45c6-124">User.Read - 允许应用程序登录你的用户</span><span class="sxs-lookup"><span data-stu-id="d45c6-124">User.Read - allows your application to sign-in your user</span></span>

- <span data-ttu-id="d45c6-125">UserActivity.ReadWrite.CreatedByApp - 允许应用订阅以获取通知检索</span><span class="sxs-lookup"><span data-stu-id="d45c6-125">UserActivity.ReadWrite.CreatedByApp - allows app subscription for notification retrieval</span></span>

![显示 Azure 门户中的通知委派权限的屏幕截图](images/notifications-api-permissions-list.png)

## <a name="next-steps"></a><span data-ttu-id="d45c6-127">后续步骤</span><span class="sxs-lookup"><span data-stu-id="d45c6-127">Next steps</span></span>

<span data-ttu-id="d45c6-128">详细了解[权限和同意](/azure/active-directory/develop/v2-permissions-and-consent)或查看 Microsoft Graph [权限参考](./permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d45c6-128">Learn more about [permissions and consent](/azure/active-directory/develop/v2-permissions-and-consent) or see the Microsoft Graph [permissions reference](./permissions-reference.md).</span></span>

<span data-ttu-id="d45c6-129">现在，你已注册应用，请访问[合作伙伴中心](https://partner.microsoft.com/)设置应用程序，并定位相应的应用平台（Windows、iOS 或 Android）以获取通过 Microsoft Graph 发送的通知。</span><span class="sxs-lookup"><span data-stu-id="d45c6-129">Now that you’ve registered your app, visit [Partner Center](https://partner.microsoft.com/) to set up your application and target your corresponding app platforms (Windows, iOS, or Android) for notifications sent via Microsoft Graph.</span></span> <span data-ttu-id="d45c6-130">有关详细信息，请参阅[载入跨设备体验](notifications-integration-cross-device-experiences-onboarding.md)。</span><span class="sxs-lookup"><span data-stu-id="d45c6-130">For details, see [Onboarding to cross-device experiences](notifications-integration-cross-device-experiences-onboarding.md).</span></span> 

>[!NOTE]
><span data-ttu-id="d45c6-131">如果仅针对 Web 终结点，则可以跳过合作伙伴中心注册并了解如何设置[应用服务](notifications-integrating-app-server.md)以发送通知。</span><span class="sxs-lookup"><span data-stu-id="d45c6-131">If you're only targeting web endpoints, you can skip Partner Center registration and learn how to set up your [app service](notifications-integrating-app-server.md) to send notifications.</span></span>