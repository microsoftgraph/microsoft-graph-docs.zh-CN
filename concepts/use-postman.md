---
title: 结合使用 Postman 和 Microsoft Graph API
description: 使用 Microsoft Graph Postman 集合，只需几分钟，即可开始使用 Microsoft Graph API。
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: c7029a68314c0a093e0943bcdad46be27155ca25
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556213"
---
# <a name="use-postman-with-the-microsoft-graph-api"></a>结合使用 Postman 和 Microsoft Graph API

使用 Microsoft Graph Postman 集合，只需几分钟，即可开始使用 Microsoft Graph API。

![Postman 图像](https://github.com/microsoftgraph/microsoftgraph-postman-collections/blob/master/images/postman.png?raw=true)

本文介绍了如何快速掌握 Postman 和 Microsoft Graph。 此外，还可以使用 [Graph 管理器](https://developer.microsoft.com/graph/graph-explorer)直接在 Web 浏览器中浏览 Microsoft Graph API。

## <a name="accessing-the-collection"></a>访问集合
可通过以下两种方法来访问 Postman 中的集合：使用集合或参与集合。 必须先在计算机上运行 [Postman](https://www.getpostman.com/)。

### <a name="consume-the-collection"></a>使用集合
使用集合是开始使用 Microsoft Graph API 的最简单方法。 若要导入 Postman 集合，请执行以下操作：

1. 下载并注册 [Postman](https://www.getpostman.com/)。
2. 依次选择“文件 | 导入”。
3. 选择“从链接导入”。
4. 粘贴以下两个 URL，再选择每个 URL 后面的“导入”。

    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph.postman_collection.json
      
    ```
    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph.postman_environment.json

    ```

现在，应该会在右上角的环境下拉列表中看到“Microsoft Graph 环境”（以眼睛图标为标识）。 现在需要[创建环境](#using-the-collection)。

## <a name="using-the-collection"></a>使用集合
在 Postman 中创建 **Microsoft Graph** 集合和 **Microsoftr Graph 环境** 后，请按照以下步骤操作。

### <a name="set-up-application-api-calls"></a>设置应用程序 API 调用

1. 选择右上角的下拉列表中的“无环境”。
2. 选择“Microsoft Graph 环境”。
3. 依次选择右侧的 **眼睛** 图标和“编辑”。
4. 在 **当前**（而不是 **初始**）变量中，输入你的 Microsoft 标识应用程序：**ClientID**、**ClientSecret** 和 **TenantID**。 
 若要详细了解如何创建应用程序，以及如何让管理员同意仅限应用的流，请参阅[使用 Postman 执行 Microsoft Graph 调用](https://developer.microsoft.com/zh-CN/graph/blogs/30daysmsgraph-day-13-postman-to-make-microsoft-graph-calls/)博客文章。

5. 选择“更新”。 关闭“管理环境”对话框。 在左侧的“**MicrosoftGraph | 应用程序**”集合中，选择“**获取仅限应用的访问令牌**”。 然后，选择右侧的“发送”。
6. 依次展开“应用程序 | 用户”文件夹，再选择“获取用户”。 然后，选择“发送”。

现在，你可以开始使用 Microsoft Graph 集合了。

>**注意：** 若要在集合中运行其他 API，需要同意应用程序拥有必需权限。

### <a name="set-up-on-behalf-of-api-calls"></a>设置代表 API 调用
设置代表 API 调用的最简单方法是，在环境设置中提供 **UserName** 和 **UserPassword**，并使用“代表用户 | 获取用户访问令牌”。 

>**重要提示**：不建议使用生产用户帐户，因为此信息直接存储在 Postman 中。 也不建议使用这种方法在生产中获取访问令牌。 只能用于测试目的。

如果不希望在同步到 Postman 云帐户的环境变量中存储用户名和密码，可使用“获取新访问令牌”功能来获取令牌，而无需离开 Postman。

1. 选择“代表用户 | 使用 Postman 获取访问令牌”。
2. 选择“授权”选项卡。
3. 选择“获取新访问令牌”按钮。
4. 使用真实的租户和应用程序值填写以下框。 请注意，不能在此处使用环境变量；必须使用实际值。 若要查找这些值，可以选择 portal.azure.com 上“应用程序”边栏选项卡中的“终结点”。

    - 回调 URL：https://app.getpostman.com/oauth2/callback
    - 验证 URL：https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/authorize
    - 访问令牌 URL：https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/token
    - 客户端 ID：**CLIENTID**
    - 客户端密码：**CLIENTSECRET**
    - 作用域：https://graph.microsoft.com/.default
    - 状态：**RANDOMSTRING**
 
5. 选择“请求令牌”。 应该会看到 UI 提示，提示你登录和同意权限。
6. 复制访问令牌，打开环境变量，并将它粘贴到“UserAccessToken”字段中。

现在，所有请求都将可以正常运行。


### <a name="contribute-to-the-collection"></a>参与集合
若要贡献你自己的请求，需要为 [Microsoft Graph Postman 集合](https://github.com/microsoftgraph/microsoftgraph-postman-collections) github 存储库创建分支。 

若要详细了解如何执行此操作，请观看以下视频。

> [!VIDEO https://www.youtube-nocookie.com/embed/4tg-OBdv_8o]
