---
title: 管理 Microsoft Graph 通知的应用注册和 API 权限
description: 为接收通过 Microsoft Graph 发送的通知，首先需要在 Microsoft Azure 门户上注册应用程序。
ms.localizationpriority: high
ms.prod: notifications
author: merzink
ms.openlocfilehash: a6bc396a670eb3d96c63a75f6a894be5893c43ce
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59049464"
---
# <a name="manage-app-registration-and-api-permission-for-microsoft-graph-notifications"></a>管理 Microsoft Graph 通知的应用注册和 API 权限

若要让应用程序服务与 Microsoft Graph 通知集成，你需要通过 Microsoft 标识平台注册应用，以支持 Microsoft 帐户或工作或学校帐户，并删除所需的 API 权限。

## <a name="register-your-app-to-support-microsoft-accounts-or-work-or-school-accounts"></a>注册应用，以支持 Microsoft 帐户或工作或学校帐户

在 [Microsoft Azure 门户](https://portal.azure.com/#home)上注册应用程序，以支持 Microsoft 帐户或工作或学校帐户。 如果已在 [Microsoft 应用程序门户](https://apps.dev.microsoft.com/)上注册帐户，则现有应用将在新增和改进的 Azure 门户体验中显示。

有关如何注册应用的信息，请参阅[向 Microsoft 标识平台注册应用程序](auth-register-app-v2.md)。 注册应用时，请确保将应用程序 ID/客户端 ID 置于方便使用的位置。 后续在适用于 Windows、Android 或 iOS 客户端的[合作伙伴中心](https://partner.microsoft.com/)注册应用程序以获取跨设备体验时，需要此 ID。

> [!NOTE]
> 如果没有 Microsoft 帐户并想要使用此类帐户，请转至 [Microsoft 帐户](https://account.microsoft.com/account) 页面。 如果正在编写需要将 Azure AD v1.0 用作工作或学校帐户的身份验证和标识框架的应用，请参阅 [Azure Active Directory 身份验证库](/azure/active-directory/develop/active-directory-authentication-libraries)。 如果你想了解或使用新聚合的 Microsoft 标识平台 (v2.0)，请参阅[比较 Microsoft 标识平台终结点和 Azure AD v1.0 终结点](/azure/active-directory/develop/azure-ad-endpoint-comparison)。


## <a name="app-certificates-and-secrets"></a>应用证书和密码

若要使应用程序在获取身份验证令牌时对自己进行标识和身份验证，你可以转至 Azure 门户中的 **证书和密码**，以上传自己的证书或创建信的客户端密码。
    
![Azure 门户中的应用证书和密码屏幕截图](images/notifications-app-secrets.png)
    
> [!NOTE]
> 如果选择生成新的客户端密码，请确保将其复制并保存到安全的位置。 离开门户后，你将无法再次访问它。

## <a name="api-permissions"></a>API 权限

需要添加其他权限才能使用 Microsoft Graph 通知。 选择“**添加权限**”，在 Microsoft API 下，选择“**Microsoft Graph**”，然后选择“**委派权限**”。
    
![Azure 门户的请求 API 权限页面的屏幕截图](images/notifications-api-permissions.png)
    
添加以下权限：

- User.Read - 允许应用程序登录你的用户

- UserActivity.ReadWrite.CreatedByApp - 允许应用订阅以获取通知检索

![显示 Azure 门户中的通知委派权限的屏幕截图](images/notifications-api-permissions-list.png)

## <a name="next-steps"></a>后续步骤

详细了解[权限和同意](/azure/active-directory/develop/v2-permissions-and-consent)或查看 Microsoft Graph [权限参考](./permissions-reference.md)。

现在，你已注册应用，请访问[合作伙伴中心](https://partner.microsoft.com/)设置应用程序，并定位相应的应用平台（Windows、iOS 或 Android）以获取通过 Microsoft Graph 发送的通知。 有关详细信息，请参阅[载入跨设备体验](notifications-integration-cross-device-experiences-onboarding.md)。 

>[!NOTE]
>如果仅针对 Web 终结点，则可以跳过合作伙伴中心注册并了解如何设置[应用服务](notifications-integrating-app-server.md)以发送通知。
