# <a name="get-started-with-microsoft-graph-in-a-java-app"></a>在 Java 应用中开始使用 Microsoft Graph

本文使用 [console-java-connect-sample](https://github.com/microsoftgraph/console-java-connect-sample) 来逐步完成通过 Microsoft Graph 从 Java 控制台应用程序发送邮件。 本文介绍了需要添加到 Java 应用的代码，以便可以使用 Microsoft Graph API。 该应用通过使用 [适用于 Java 的 Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-java) 来访问 Microsoft Graph。

## <a name="choose-an-authentication-library"></a>选择身份验证库

Microsoft Graph 采用了 OAuth 2.0 和 Open ID Connect 标准，它允许你从多个可用的开源 OAuth 2 Java 库中进行选择。 Azure AD 团队建议使用 [ScribeJava](https://github.com/scribejava/scribejava)，它是 Java 的一个简单 OAuth2 库。

此示例实现了授权代码授予流，这对于客户端授权方案、用户以及启用了 OAuth 2 的终结点来说是恰当的选择。 在生产服务器间 Java 应用程序中，使用的是客户端凭据授权流。 **ScribeJava** 处理这两个授权流。 为了使本示例容易进行注册、身份验证和运行，我们演示了最简单的流程。

在应用可以在 Microsoft Graph 上执行调用之前，应用必须从 Azure Active Directory (Azure AD) 获得一个访问令牌。 每次调用 Microsoft Graph 时，此令牌必须出现在 HTTP 身份验证标头中。 在你实施 [IAuthenticationProvider](https://github.com/microsoftgraph/msgraph-sdk-java/blob/dev/src/main/java/com/microsoft/graph/authentication/IAuthenticationProvider.java) 时，**Microsoft Graph SDK** 负责插入标头和添加每个调用令牌。 **ScribeJava** 处理身份验证和获取访问令牌。 应用通过 **IAuthenticationProvider** 界面向 Microsoft Graph SDK 提供访问令牌。

## <a name="install-and-run-the-sample"></a>安装并运行示例

若要安装和配置示例应用，请按照 GitHub 上 **console-java-connect-sample** 存储库中的 [README](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md) 文档中的说明操作。 可以通过此命令克隆示例并逐步完成你最喜爱的 Java IDE 中的代码来克隆存储库：

```
git@github.com:microsoftgraph/console-java-connect-sample.git
```

在[注册 Console Java Connect 应用](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md#register-your-app)时，向示例分配委派作用域（权限）。 确保作用域如中下图所示：

![Java 连接控制台示例权限](../concepts/images/console-java-connnect-sample-permissions.JPG)

在注册应用程序并为从应用程序注册获取的**应用程序 ID** [配置示例](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md#configure-your-app)后，可以生成并运行示例。

## <a name="console-java-connect-code"></a>Console-Java-Connect 代码 

在查看示例逻辑流之前，请花几分钟时间了解一下[示例项目的结构](#sample-project-structure)。 如果已准备就绪，则可以逐步完成示例中的逻辑：


   
### <a name="walk-through-the-code"></a>演练代码
我们将先概括性地查看示例代码，然后再深入了解有关创建电子邮件和发送邮件的详细信息。

#### <a name="the-user-experience"></a>用户体验

本节将介绍启动应用程序的逻辑，然后向你展示用户在运行示例时看到的示例输出。

[PublicClient](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/PublicClient.java) **主**静态方法创建一个 **PublicClient** 实例，然后启动登录和身份验证过程。  

[AuthenticationManager](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/AuthenticationManager) 提供了用于将用户连接到 Microsoft Graph 的单一实例。 **AuthenticationManager** 以字符串属性形式公开**访问令牌**。 当对用户进行身份验证并授予示例权限来访问请求的 Microsoft Graph 资源时，将由 **Azure AD** 返回访问令牌。 

**PublicClient.startSendMail** 方法执行以下步骤：

- 创建 [GraphSendMail](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphSendMail.java) 类的新实例。 
- 调用 **GraphSendMail.getMeUser()**，以返回当前用户的 **Azure AD** 配置文件，以便示例控制台对象可个性化设置向用户显示的提示。 
- 控制台会显示：

   `Hello, Laura Steele. Would you like to send an email to yourself or someone else?`

   `Enter the address to which you'd like to send a message. If you enter nothing, the message will go to your address`

- 调用 **GraphSendMail.sendMail** 方法，这将接受用户输入。 如果提供电子邮件地址，**sendMail** 会将邮件发送到此地址。 否则，邮件会被发送给当前用户。 

- 提示用户发送另一封电子邮件或退出控制台应用。

   `Email sent!`

   `Want to send another message? Type 'y' for yes and any other key to exit.`

#### <a name="the-send-mail-logic"></a>发送邮件逻辑

邮件发送逻辑将执行以下步骤：



1. **获取个人资料图片**：<br/> 调用 **GraphServiceController.getUserProfilePicture()**，以获取表示已登录到示例的 **Azure AD** 用户的个人资料图片的字节数组。

   **API 调用**

```java
            photoStream = mGraphServiceClient
                    .me()
                    .photo()
                    .content()
                    .buildRequest()
                    .get();

```
2. **将图片上传到 OneDrive**：
<br/>调用 **GraphServiceController.uploadPictureToOneDrive(bytes)**，以在用户的 OneDrive 根文件夹中发布个人资料图片。 将返回 Microsoft Graph SDK **DriveItem** 对象。 

   **API 调用**
```java
            driveItem = mGraphServiceClient
                    .me()
                    .drive()
                    .root()
                    .itemWithPath("me2.png")
                    .content()
                    .buildRequest()
                    .put(picture);

```
3. **使 OneDrive 共享该图片链接**：<br/>调用 **GraphServiceController.getPermissionSharingLink**，以创建新的共享链接。 将返回 Microsoft Graph SDK **Permission** 对象。

   **API 调用**
```java
            permission = mGraphServiceClient
                    .me()
                    .drive()
                    .items(id)
                    .createLink("view", "organization")
                    .buildRequest()
                    .post();

```
4. 使用上一步中共享链接的 **webUrl** **替换 HTML 模板定位标记的内容**。 
> **注意：** 应用程序发送的邮件正文源自作为静态字符串存储在 [Constants.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Constants.java) 中的 HTML 模板。 发送时，邮件正文包含一个公共共享超链接，指向示例上传到用户的 OneDrive 根文件夹的图片。 
5. **创建草稿邮件**： <br/>调用 **GraphServiceController.createDraftMail**，传递收件人电子邮件地址、主题文本和更新的 HTML 模板。 将创建草稿邮件并发布到用户的草稿邮件文件夹。

   **API 调用**
```java
            message = mGraphServiceClient
                    .me()
                    .messages()
                    .buildRequest()
                    .post(message);

```
6. **将图片附加到草稿邮件**： <br/>调用 **GraphServiceController.addPictureToDraftMessage**，以获取草稿邮件，并将图片作为对象附件添加到邮件。

   **API 调用**
```java
            FileAttachment fileAttachment = new FileAttachment();
            fileAttachment.oDataType = "#microsoft.graph.fileAttachment";
            fileAttachment.contentBytes = attachementBytes;
            fileAttachment.name = "me.png";
            fileAttachment.size = attachementBytes.length;
            fileAttachment.isInline = false;
            fileAttachment.id = "my profile picture";

            attachment = mGraphServiceClient
                    .me()
                    .messages(messageId)
                    .attachments()
                    .buildRequest()
                    .post(fileAttachment);

```
7. **发送草稿邮件**：<br/>调用 **GraphServiceController.sendDraftMessage**，以便向预期用户发送已更新的草稿邮件。

   **API 调用**
```java
            mGraphServiceClient
                    .me()
                    .mailFolders("Drafts")
                    .messages(messageId)
                    .send()
                    .buildRequest()
                    .post();

```



### <a name="sample-project-structure"></a>示例项目结构

### <a name="connect-package"></a>连接包
此包包含 OAuth2 身份验证流逻辑和将要更新的配置。

- [AuthenticationManager.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/AuthenticationManager.java)：此类导入用于授权代码授予流的 **ScribeJava** 对象。
- [Constants.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Constants.java)：保留提供应用注册相关值的公共静态字符串和应用程序发送的电子邮件的模板。
- [Debug.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Debug.java)：公共调试级别标志。 设置其值以更改示例应用的日志记录行为。
- [DebugLogger.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/DebugLogger.java)：根据调试级别设置将信息写入控制台的日志记录实用工具。
- [IConnectCallback](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/IConnectCallback.java)：定义回调方法，如果你调用 **ScribeJava.getAccessToken** 方法的异步重载，将会使用它。
- [SendMailException](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/SendMailException.java)：从**异常**中派生的类，并封装 Microsoft Graph 特定的异常信息。 **GraphSendMail** 包中的类可引发此类异常。

### <a name="msgraph-package"></a>msgraph 包

此包包含在 Microsoft Graph 上进行调用的所有逻辑。

- [GraphSendMail](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphSendMail.java)：链接在一起调用 **GraphServiceController**（Microsoft Graph API 示例帮助程序类），以创建和发送包含图片附件的电子邮件。
- [GraphServiceClientManager.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphServiceClientManager.java)：实例化 Microsoft Graph SDK [GraphServiceClient](https://github.com/microsoftgraph/msgraph-sdk-java/blob/dev/src/main/java/com/microsoft/graph/requests/extensions/GraphServiceClient.java)，并将访问令牌添加到 Microsoft Graph 终结点上的所有出站 API 调用。

- [GraphServiceController.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphServiceController.java)：使用 Microsoft Graph SDK 以完成对 **GraphServiceClient** 的所有调用。 调用包括：

   - **createDraftMail**：创建草稿电子邮件并将其保存在草稿邮件文件夹中。
   - **sendNewMessageAsync**：创建和发送电子邮件。
   - **addPictureToDraftMessage**：根据邮件 ID 发布草稿邮件中的文件附件
   - **addAttachmentToDraftAsync**：将附件添加到草稿邮件。
   - **sendDraftMessage**：从草稿文件夹发送邮件。
   - **getDraftMessage**：从用户邮件集中根据邮件 ID 获取邮件。
   - **getUser**：获取通过 Microsoft Graph API 终结点进行身份验证的本地用户。
   - **getUserProfilePicture**：从 Microsoft Graph 获取已登录用户的个人资料图片。
   - **uploadPictureToOneDrive**：将图片以字节数组形式上传到用户的 OneDrive 根文件夹。
   - **getPermissionSharingLink**：请求 OneDrive 创建指向存储在 OneDrive 中的图片的公用共享链接。

## <a name="other-microsoft-graph-samples"></a>其他 Microsoft Graph 示例

若要查看某个特定示例，请通过[提交问题](https://github.com/microsoftgraph/console-java-connect-sample/issues)告诉我们。 我们非常期待收到大家就希望在 Java 中生成的任何 Microsoft Graph 方案提供的反馈！

Microsoft Graph API 的功能非常强大，统一了可用于与各种 Microsoft 数据进行交互的 API。 请查看[开发人员文档](https://developer.microsoft.com/zh-CN/graph/docs/concepts/overview)或 [Graph 浏览器](https://developer.microsoft.com/zh-CN/graph/graph-explorer)，了解还可以使用 Microsoft Graph 做什么。
