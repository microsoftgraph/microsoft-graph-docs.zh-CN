---
ms.localizationpriority: medium
ms.openlocfilehash: a31594b0add328d1515eeb4965334be724b02a05
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59289521"
---
<!-- markdownlint-disable MD002 MD041 -->

在此练习中，你将创建、运行和批准 Azure 数据工厂管道，以将数据从 Microsoft 365 提取到 Azure 存储 Blob 进行其他处理。

## <a name="create-a-microsoft-azure-active-directory-application-registration"></a>创建Microsoft Azure Active Directory应用程序注册

第一步是创建 Azure AD 应用程序，该应用程序将用作运行数据提取过程的安全主体。

1. 打开浏览器并转到 Azure [门户](https://portal.azure.com/)。

1. 使用具有 Azure 和租户 **全局** 管理员权限Microsoft 365登录。

1. 在边栏导航上，选择 **Azure Active Directory (** Azure AD) 。

1. 在"Azure AD 概述"页上，从菜单 **的** " **管理"部分** 选择"应用注册"。

1. 选择" **新建注册"** 按钮。

    ![显示 Azure 门户中 Azure Active Directory 服务的应用注册的屏幕截图。](images/data-connect-azure-aad-app-reg.png)

1. 使用以下值创建新的 Azure AD 应用程序，然后选择"注册 **"。**

   - **名称**：Microsoft Graph 数据连接数据传输
   - **支持的帐户类型**：仅此组织目录中的帐户。
   - **重定向 URI：** 保留默认值。

    ![显示在 Azure 门户中注册新应用程序注册的步骤的屏幕截图。](images/data-connect-aad-redirect-uri.png)

1. 找到 **应用程序 (客户端) ID，** 然后复制它，因为本教程稍后将需要它。 这称为服务主体 ID。

1. 找到 **" (租户) ID，** 并复制它，因为本教程稍后将对此进行介绍。 这称为租户 ID。

1. 在边栏导航上，选择"管理 **"下的"证书和****密码"。**

1. 选择" **新建客户端密码"按钮**。 将 *"说明*"设置为任意名称，将 **"到期**"设置为下拉列表中的任意值，然后选择"添加 **"。**

    ![显示在 Azure 门户中创建新客户端密码的过程的屏幕截图。](images/data-connect-aad-certs-secrets.png)

    - 创建客户端密码后，请确保将 **"** 值"保存在安全位置，因为稍后将不再可用，并且需要创建新的密码。
    - 这将作为服务主体密钥引用。

1. 在应用程序的边栏导航上， **选择所有者**。

1. 验证您的帐户是否列为应用程序的所有者。 如果未列为所有者，请添加它。

    ![显示用户确认其帐户已设置为 Azure 门户中应用程序注册的所有者的屏幕截图。](images/data-connect-aad-app-owners.png)
