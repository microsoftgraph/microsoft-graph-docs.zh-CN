---
title: 结合使用 Postman 和 Microsoft Graph API
description: Postman 是用于构建和使用 API 的 API 平台。 使用 Microsoft Graph Postman 集合开始使用Microsoft Graph API。
author: jasonjoh
ms.localizationpriority: high
ms.openlocfilehash: ace39134b6a30ce3b8cfe79f539f6d1887a21b02
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2022
ms.locfileid: "66554902"
---
# <a name="use-postman-with-the-microsoft-graph-api"></a>结合使用 Postman 和 Microsoft Graph API

Postman 是用于构建和使用 API 的 API 平台。 Postman 简化了 API 生命周期的每个步骤并简化了协作，使你可以更快地创建更好的 API。

使用 Microsoft Graph Postman 集合，只需几分钟，即可开始使用 Microsoft Graph API。

![Postman 图像](images/postman-screenshot.png)

本文介绍了如何快速掌握 Postman 和 Microsoft Graph。 此外，还可以使用 [Graph 管理器](https://developer.microsoft.com/graph/graph-explorer)直接在 Web 浏览器中浏览 Microsoft Graph API。

若要详细了解如何使用 Postman，请跟随本文中的步骤进行或观看 [Microsoft Graph Postman 工作区入门](https://youtu.be/3RTHY3jScmA)视频。

## <a name="step-1-fork-the-microsoft-graph-postman-collection"></a>步骤 1：分叉 Microsoft Graph Postman 集合

若要使用 Postman 集合，请将其导入到你自己的 Postman 工作区。在 web 浏览器中进行该操作。

1. 转到 [Postman](https://www.postman.com/) 并登录。
1. 转到标签名为 [Microsoft Graph](https://www.postman.com/microsoftgraph/workspace/microsoft-graph/collection/455214-085f7047-1bec-4570-9ed0-3a7253be148c/fork) 的 Postman 集合。
1. 为你自己的分叉填写标签；任何文本皆可。
1. 在“**工作区**”下，请确保在下拉列表中选中“**我的工作区**”。
1. 选择“**分支集合**”。

这会将你重定向至你的工作区中主要 Microsoft Graph Postman 集合的一个分支。

## <a name="step-2-download-the-postman-agent-optional---postman-web-browser-only"></a>步骤 2 - 下载 Postman 代理（可选 - 仅限 Postman Web 浏览器） 

要在 web 浏览器中使用此 Postman 集合，请下载 [Postman 桌面代理](https://www.postman.com/downloads)。 由于 web 浏览器的限制，无法在未下载此代理的情况下在 web 上使用 Postman。

如果你正在使用 Postman for Windows 应用，则不需要此代理。 打开 Postman for Windows 后，你会在工作区中看到这个分支集合。

## <a name="step-3-create-an-azure-ad-application"></a>步骤 3：创建 Azure AD 应用程序

要在自己的开发人员租户中使用此集合，请创建一个 Azure Active Directory (Azure AD) 应用程序，并根据想要调用的请求向其授予合适权限。 如果没有开发者租户，你可以通过 [Microsoft 365 开发人员计划](https://developer.microsoft.com/microsoft-365/dev-program)注册一个。

1. 转到 [portal.azure.com](https://portal.azure.com/) 并使用开发者租户管理员帐户登录。
1. 在 **Azure 服务** 下，选择“**Azure Active Directory**”。
1. 在左侧菜单上，选择 **注册**。
1. 在水平菜单中，单击“**新建注册**”。
1. 将“**应用名称**”设置为“`Postman`”。
1. 从下拉菜单中选择“**Web**”。
1. 将“**重定向 URI**”设置为“`https://oauth.pstmn.io/v1/browser-callback`”。
1. 选择“**注册**”。
1. 在左侧菜单上，选择 **API 权限**。
1. 在水平菜单上，依次选择“**添加权限**”和“**Microsoft Graph**”，然后选择“**委托的权限**”。
1. 键入 `Mail.`，展开“**邮件**”选项，然后选择 `Mail.Read`。
1. 选择“**应用程序权限**”，键入 `User.`，然后选择“**应用程序权限**”。
1. 展开“**用户**”选项，然后选择 `User.Read.All`。
1. 选择 **添加权限**。
1. 在水平菜单上，选择“**授予管理员同意**”，然后选择“**是**”。
1. 在左侧的菜单中，选择“**概述**”。 在这里，可以获取 **应用程序（客户端）ID** 和 **目录（租户）ID**。 步骤 4 中将需要使用这些信息。
1. 在左侧菜单中，选择“**证书和机密**”。
1. 选择“**新建客户端机密**”，输入说明，然后选择“**添加**”。 将鼠标光标悬停在新客户端机密 **值** 上并复制它；步骤 4 中需要用到它。

应用程序现在配置了两个权限。 `Mail.Read` 添加为委托的权限，这是需要登录用户的权限。 应用程序可以代表用户读取邮件。 `User.Read.All` 添加为应用程序权限，这是不需要登录用户的权限。 应用程序可以在 Azure AD 中读取用户。

## <a name="step-4-configure-authentication"></a>步骤 4：配置身份验证

在此步骤中，你将在 Postman 中设置用于检索访问令牌的环境变量。

1. 转到 [分叉](https://www.postman.com/microsoftgraph/workspace/microsoft-graph/environment/455214-efbc69b2-69bd-402e-9e72-850b3a49bb21/fork)。
1. 为分叉添加标签。 此值可以是任何文本。
1. 在“**工作区**”下，请确保在下拉列表中选中“**我的工作区**”。
1. 选择“**分支环境**”。
1. 在 `ClientID` 中，将“**当前值**”设置为步骤 3.16 中的应用程序（客户端）ID 值。
1. 在 `ClientSecret` 中，将“**当前值**”设置为步骤 3.18 中的客户端密码值。
1. 在 `TenantID` 中，将“**当前值**”设置为步骤 3.16 中的目录（租户）ID 值。
1. 在右上角，选择“**保存**”。
1. 关闭" **"选项卡** "。
1. 在右上方的眼睛图标旁边，验证是否已在下拉列表中选择了“**M365 环境**”，而不是“**无环境**”。

## <a name="step-5-get-a-delegated-access-token"></a>步骤 5：获取委派的访问令牌

由于这是你第一次以委派身份验证流的形式运行请求，因此，你需要获取访问令牌。

1. 选择“**委派**”文件夹。
1. 选择“**授权**”选项卡。
1. 在“**配置新令牌**”部分，选择“**配置选项**”选项卡。将所有字段保留为预配置的状态，包括设置为 `Authorization Code` 的“**授权类型**”。
1. 在右侧向下滚动并选择“**获取新的访问令牌**”。
1. 使用你的开发者租户管理员账户登录。
1. 选择“**继续**”，然后选择“**使用令牌**”按钮。

你现在已具有用于委派请求的有效访问令牌。

## <a name="step-6-run-your-first-delegated-request"></a>步骤 6：运行你的第一个委派请求

“**Delegated**”文件夹内是你可以调用的各种 Microsoft Graph 工作负载的请求。

1. 展开“**Delegated**”文件夹，然后展开“**Mail**”文件夹。
1. 双击“**获取我的邮件**”来打开请求。
1. 在右上角，选择“**发送**”。

你已经成功地使用委派身份验证完成了一次 Microsoft Graph 调用。

## <a name="step-7-get-an-application-access-token"></a>步骤 7：获取应用程序访问令牌

由于这是你第一次以应用程序身份验证流的形式运行请求，因此，你需要获取访问令牌。

1. 选择“**应用程序**”文件夹。
1. 选择“**授权**”选项卡。
1. 在“**配置新令牌**”部分，选择“**配置选项**”选项卡。将所有字段保留为预配置的状态，包括设置为 `Client Credentials` 的“**授权类型**”。
1. 在右侧向下滚动并选择“**获取新的访问令牌**”。
1. 选择“**继续**”，然后选择“**使用令牌**”按钮。

你现在已具有用于委派请求的有效访问令牌。

## <a name="step-8-run-your-first-application-request"></a>步骤 8：运行你的第一个应用程序请求

“**Application**”文件夹内是你可以调用的各种 Microsoft Graph 工作负载的请求。

1. 展开“**Application**”文件夹，然后展开“**User**”文件夹。
1. 双击“**获取用户**”来打开请求。
1. 在右上角，选择“**发送**”。

你已经成功地使用应用程序身份验证完成了一次 Microsoft Graph 调用。

你可以按照这些步骤向 Microsoft Graph 发出其他请求。 请记住，你需要向你的 Azure AD 应用程序添加权限来使其他请求正常工作；否则，你将在响应中收到权限被拒的错误。

### <a name="contribute-to-the-collection"></a>参与集合

如果想贡献你自己的请求，你需要 Postman 许可。 你可以对分支集合做出更改，然后将鼠标光标悬浮在集合的顶端节点，然后选择“**创建拉取请求**”。

## <a name="known-issues"></a>已知问题

### <a name="authentication-fails-with-you-cant-get-there-from-here"></a>身份验证失败，并显示“无法从此处到达该处”

组织管理员配置的某些[条件访问策略](/azure/active-directory/conditional-access/overview)可能会阻止来自 Postman 的身份验证流。请联系管理员以了解替代方案。

## <a name="see-also"></a>另请参阅

- [将 Postman 与 Microsoft Graph 连接器 API 一并使用](connecting-external-content-connectors-api-postman.md)
