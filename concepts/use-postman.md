---
title: 结合使用 Postman 和 Microsoft Graph API
description: 使用 Microsoft Graph Postman 集合，只需几分钟，即可开始使用 Microsoft Graph API。
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: 04668cd76a7d8ca298e2ad16483be902c59983c5
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469043"
---
# <a name="use-postman-with-the-microsoft-graph-api"></a>结合使用 Postman 和 Microsoft Graph API
使用 Microsoft Graph Postman 集合，只需几分钟，即可开始使用 Microsoft Graph API。

![Postman 图像](https://github.com/microsoftgraph/microsoftgraph-postman-collections/blob/master/images/postman.png?raw=true)

本文介绍了如何快速掌握 Postman 和 Microsoft Graph。 此外，还可以使用 [Graph 管理器](https://developer.microsoft.com/graph/graph-explorer)直接在 Web 浏览器中浏览 Microsoft Graph API。

有关如何操作的详细信息，请跟随此文章中的步骤或观看 [Microsoft Graph Postman 工作区入门](https://youtu.be/3RTHY3jScmA)视频。


## <a name="step-1---forking-the-microsoft-graph-postman-collection"></a>第一步 - 创建 Microsoft Graph Postman 集合分支
要使用 Postman 集合，请创建其分支到你的 Postman 工作区。 在 web 浏览器中进行该操作。

1. 转到 [Postman](https://www.postman.com/) 并登录。
2. 转到标签名为 [Microsoft Graph](https://www.postman.com/microsoftgraph/workspace/microsoft-graph/collection/455214-085f7047-1bec-4570-9ed0-3a7253be148c/fork) 的 Postman 集合。
3. 为你的分支填充标签。 此值可以是任何文本。
4. 在工作区下，请确保在下拉列表中选中 **我的工作区**。 
5. 单击 **分支集合**。

随后会重定向至你的工作区中主要 Microsoft Graph Postman 集合的一个分支。

## <a name="step-2---optional---postman-web-browser-only-download-the-postman-agent"></a>第二步 - （可选 - 仅针对 Postman web 浏览器）下载 Postman 代理。
要在 web 浏览器中使用此 Postman 集合，请下载 [Postman 桌面代理](https://www.postman.com/downloads)。 由于 web 浏览器的限制，无法在未下载此代理的情况下在 web 上使用 Postman。 

如果你正在使用 Postman for Windows 应用，则不需要此代理。 打开 Postman for Windows 后，你会在工作区中看到这个分支集合。

## <a name="step-3---create-an-azure-ad-application"></a>第三步 - 创建 Azure AD 应用程序
要在你的开发者租户中使用此集合，请创建一个 Azure AD 应用程序并根据想要调用的请求给予其合适的权限。 如果没有开发者租户，你可以通过 [Microsoft 365 开发人员计划](https://developer.microsoft.com/zh-CN/microsoft-365/dev-program)注册一个。

1. 转到 [portal.azure.com](https://portal.azure.com/) 并使用开发者租户管理员帐户登录。
2. 单击 “**Azure Services**” 下的 “**Azure Active Directory**”。
3. 在左侧菜单中，单击“**应用注册**”。
4. 在水平菜单中，单击“**新建注册**”。
5. 将“**应用名称**”设置为“`Postman`”。
6. 将“**重定向 URI**”设置为“`https://oauth.pstmn.io/v1/browser-callback`”。
7. 单击“**注册**”。
8. 在左侧菜单中，单击 “**API 权限**”。
9. 在水平菜单中，单击“**添加权限**”，选择 “**Microsoft Graph**”，然后选择“**委派权限**”。
10. 键入“`Mail.`”，展开“**邮件**”选项，然后检查 **Mail.Read**.
11. 单击“**应用权限**”然后键入“`User.`”，随后检查“**应用权限**”。
12. 展开“**用户**”选项并检查 **User.Read.All**。
13. 单击“**添加权限**”。
14. 在水平菜单中，单击“**授予管理员许可**”，并单击“**确定**”。
15. 在左侧菜单中，单击“**概述**”。 你可以从这里获取“**应用程序（客户端）ID**” 和“**目录（客户端）ID**”。 这些会在第四步中用到。
16. 单击左侧菜单中的“**证书和机密**”。 
17. 单击“**新建客户端机密**”，并输入简短说明，然后单击“**添加**”。 将鼠标光标悬浮在新的客户端机密 **值** 上并复制。 第四步中会用到它。

Azure AD 应用程序现已具有代表用户提出调用 Mail.Read 请求的权限并成为 User.Read.All 的一个应用。

## <a name="step-4---configuring-authentication-in-postman"></a>步骤 4 - 在 Postman 中配置身份验证
转到"邮政编码"，并确保已选择步骤 1 中创建的工作区。 设置一些环境变量来检索访问令牌。

1. 单击右上角“**无环境**”下拉菜单旁边的眼睛图标。
2. 单击弹出窗口右上角的“**添加**”。
3. 将“**新环境**”更改为“**M365 环境**”。
4. 创建名为`ClientID`的变量并将“**当前值**”设置为步骤 3.15 中的应用程序（客户端）ID 值。
5. 创建名为`ClientSecret`的变量并将“**当前值**”设置为步骤 3.17 中的客户端机密值。
6. 创建名为`TenantID`的变量并将“**当前值**”设置为步骤 3.15 中的目录（租户）ID 值。
7. 选择“**保存**”/“**更新**”。 
8. 关闭“**管理环境**”对话框。 
9. 仔细检查是否在下拉菜单中选中了 “**M365 环境**” 而不是 “**无环境**”。

## <a name="step-5---get-a-delegated-access-token"></a>第五步 - 获取委派的访问令牌
由于这是你第一次通过委派身份验证流程运行请求，你需要获取访问令牌。

1. 将鼠标光标悬浮在“**代表用户**”文件夹上，单击省略号，然后选择“**编辑**”
2. 单击“**授权**”选项卡。
3. 在右侧下滑并单击“**获取新的访问令牌**”。
4. 登录你的开发者租户管理员账户。
5. 单击“**继续**”，然后单击“**使用令牌**”按钮。
6. 在该对话框的右下角，单击“**更新**”。

你现在已具有用于委派请求的有效访问令牌。

## <a name="step-6---run-your-first-delegated-request"></a>第六步 - 运行你的第一个委派请求
“**代表用户**”文件夹中是你可以调用的各种 Microsoft Graph 工作负载请求。

1. 展开 “**代表用户**”文件夹，然后展开“**邮件**”文件夹。
2. 双击“**获取我的邮件**”来打开请求。
3. 在右上角，单击“**发送**”。

你已经成功地使用委派身份验证完成了一次 Microsoft Graph 调用。

## <a name="step-7---get-an-application-access-token"></a>第七步 - 获取应用程序访问令牌
由于这是你第一次通过应用程序身份验证流程运行请求，你需要获取访问令牌。

1. 将鼠标光标悬浮在“**应用程序**”文件夹上，单击省略号，然后选择“**编辑**”。
2. 单击“**授权**”选项卡。
3. 在右侧下滑并单击“**获取新的访问令牌**”。
5. 单击“**继续**”，然后单击“**使用令牌**”按钮。
6. 在该对话框的右下角，单击“**更新**”。

你现在已具有用于委派请求的有效访问令牌。

## <a name="step-8---run-your-first-application-request"></a>第八步 - 运行你的第一个应用程序请求
“**应用程序**”文件夹中是你可以调用的各种 Microsoft Graph 工作负载请求。

1. 展开“**应用程序**”文件夹，然后展开“**用户**”文件夹。
2. 双击“**获取用户**”来打开请求。
3. 在右上角，单击“**发送**”。

你已经成功地使用应用程序身份验证完成了一次 Microsoft Graph 调用。

你可以按照这些步骤向 Microsoft Graph 发出其他请求。 请记住，你需要向你的 Azure AD 应用程序添加权限来使其他请求正常运行；否则，你将在响应中收到权限被拒的错误。

### <a name="contribute-to-the-collection"></a>参与集合
若要贡献你自己的请求，需要 Postman 许可。 你可以对分支集合做出更改，然后将鼠标光标悬浮在集合的顶端节点，然后选择“**创建拉取请求**”。

## <a name="see-also"></a>另请参阅

有关如何操作的详细信息，请观看 [Microsoft Graph Postman 工作区入门](https://youtu.be/3RTHY3jScmA)视频。


