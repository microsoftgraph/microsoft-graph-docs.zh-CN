---
title: 使用 Microsoft Graph API 在 Visual Studio 2017 中调用 Microsoft 365 服务
description: 你可以使用 Visual Studio 中的连接服务配置应用，从而调用 Microsoft Graph API。本文介绍如何获取登录用户的个人资料照片、将其上载至 OneDrive，和发送一封包含指向照片的共享链接的电子邮件。
localization_priority: Priority
ms.prod: reports
author: sarahwxy
ms.openlocfilehash: 95fbe544edff9543d694f5fa024929fd7e241160
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921663"
---
# <a name="call-microsoft-365-services-in-visual-studio-2017-with-the-microsoft-graph-api"></a>使用 Microsoft Graph API 在 Visual Studio 2017 中调用 Microsoft 365 服务

你可以使用 Visual Studio 中的连接服务配置应用，从而调用 Microsoft Graph API。本文介绍如何获取登录用户的个人资料照片、将其上载至 OneDrive，和发送一封包含指向照片的共享链接的电子邮件。

## <a name="get-set-up"></a>开始设置

若要通过 Microsoft Graph 使用 Office 365 连接服务，你需要执行以下操作：

- 如果未下载，请下载 [Visual Studio 2017 Preview](https://www.visualstudio.com/vs/preview/)。如果你使用的是 Visual Studio 的早期版本，你可以将 Visual Studio 2017 Preview 与你的当前版本并排使用。

- 获取 Microsoft 365 订阅。若要获取免费试用版，请加入 [Microsoft 365 开发人员计划](https://developer.microsoft.com/microsoft-365/dev-program)。

## <a name="get-the-starter-project"></a>获取初学者项目

下载 [Microsoft Graph ASP.NET 已连接服务示例](https://github.com/microsoftgraph/aspnet-connect-sample/archive/Office365connectedservice.zip)。此示例包括针对 Microsoft Graph 进行身份验证所需的引用。下载初学者项目后，请解压，然后在 Visual Studio 2017 Preview 中打开示例。

## <a name="add-the-connected-service"></a>添加已连接服务

你现在可以将 Microsoft Graph 服务添加到 Visual Studio 项目中。 

1. 在解决方案资源管理器中，选择“连接的服务”打开“连接的服务”选项卡。 

2. 选择“**使用 Microsoft Graph 访问 Microsoft 365 服务**”提供程序。 按照向导操作。 选择以下权限（你可以在以后更改）：

    - 对于“文件”API，将权限设置为“拥有对文件的完全访问权限”。
    - 对于“邮件”API，将权限设置为“以你的身份发送邮件”。
    - 对于“用户”API，将权限设置为“登录并读取你的个人资料”。

## <a name="call-the-microsoft-graph-api"></a>调用 Microsoft Graph API

初学者示例被配置为发送简单的电子邮件。你可以使用 Microsoft Graph 更新示例，从而发送一封包含指向 OneDrive 中已登录用户的个人资料照片的链接的电子邮件。

1. 转到托管可调用 Microsoft Graph 的代码的“Models\GraphService.cs”。

2. 按以下方法查找对 SDK 的调用并 **取消评论**。这演示了如何调用 Microsoft Graph 以获取个人资料照片、将文件上载至 OneDrive 和获取共享链接。

    ```csharp
        GetCurrentUserPhotoStream(GraphServiceClient graphClient)
    ```
    
    ```csharp
        UploadFileToOneDrive(GraphServiceClient graphClient, byte[] file)
    ```

    ```csharp
        GetSharingLink(GraphServiceClient graphClient, string Id)
    ```
 
> **提示：** 每条评论均以“//Uncomment:”开头
 

## <a name="run-the-sample"></a>运行示例
生成和运行示例 接下来，选择右上角的“登录”链接，然后依次选择“获取电子邮件地址”和“发送电子邮件”

这将发送一封电子邮件，其中包含指向你的个人资料照片的链接。

>**注意：**

>- 如果停止并从 Visual Studio 中重新运行示例，你可能需要明确注销才能使示例运行。
>- 如果你收到异常，指示用户未通过身份验证，则你可能需要重复[添加连接的服务](#add-the-connected-service)步骤。
>- 确保使用与你在向导的 **选择域** 步骤中选择的相同域中的帐户登录。

## <a name="explore-the-code"></a>浏览代码

你现在可以使用 Visual Studio 2017 连接并配置你的服务。初学者示例为你创建基架和引用。  

初学者示例包括以下文件：

- [Startup.Auth.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/App_Start/Startup.Auth.cs) - 对当前用户进行身份验证并初始化该示例的令牌缓存。

- TokenStorage\\[SessionTokenCache.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/TokenStorage/SessionTokenCache.cs) - 存储用户的令牌信息。 可以使用你自己的自定义令牌缓存来替换此信息。 有关详细信息，请参阅[在多租户应用程序中缓存访问令牌](/azure/architecture/multitenant-identity/token-cache)。

- Helpers\\[SampleAuthProvider.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SampleAuthProvider.cs) - 实施本地 IAuthProvider 接口，并获取访问令牌。 

- Helpers\\[SDKHelper.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SDKHelper.cs) - 初始化来自用于与 Microsoft Graph 交互的 [Microsoft Graph .NET 客户端库](https://github.com/microsoftgraph/msgraph-sdk-dotnet)中的 **GraphServiceClient**。

- Controllers\\[HomeController.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Controllers/HomeController.cs) - 包含使用 **GraphServiceClient** 生成和发送对 Microsoft Graph 服务的调用并处理响应的方法。

- Views\\Home\\[Graph.cshtml](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Views/Home/Graph.cshtml) - 包含示例的 UI。 


## <a name="need-help"></a>需要帮助?

如果需要帮助，请在 [Microsoft Q&A](/answers/products/m365#microsoft-graph) 上发布你的问题。 使用 {microsoft-graph-identity} 标记你发布的问题。
