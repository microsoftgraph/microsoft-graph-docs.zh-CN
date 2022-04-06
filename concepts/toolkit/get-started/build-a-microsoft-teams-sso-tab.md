---
title: 使用 Microsoft Microsoft Teams生成一个 SSO Graph Toolkit
description: 开始 Microsoft Microsoft Teams生成一个 SSO Graph Toolkit。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 43a7a7b4b1fee3f33b027f170eb66cd04e49157d
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588811"
---
# <a name="build-a-microsoft-teams-sso-tab-with-the-microsoft-graph-toolkit"></a>使用 Microsoft Microsoft Teams生成一个 SSO Graph Toolkit

本主题介绍如何在解决方案Graph Toolkit Microsoft Microsoft Teams Microsoft 解决方案。 本指南适用于在 SSO 应用中具有单一登录 (单页) 并且确实需要后端。 如果要使用交互式登录实现 Teams 选项卡，请参阅生成Microsoft Teams[选项卡](./build-a-microsoft-teams-tab.md)。

构建 SSO 选项卡包括以下步骤： 

1. 添加 Microsoft Graph Toolkit。
1. 创建身份验证弹出窗口页面。
1. 创建应用/客户端 ID
6. 创建后端
7. 初始化 MSAL2 Teams。
8. 添加组件。
9. 测试你的应用。

## <a name="add-the-microsoft-graph-toolkit"></a>添加 Microsoft Graph Toolkit

可以在应用程序中使用 Microsoft Graph Toolkit，方法为直接通过 unpkg (加载程序) 安装 npm 包。 若要使用Toolkit，你还需要 Microsoft Teams [SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk)。

# <a name="unpkg"></a>[unpkg](#tab/unpkg)
若要通过Toolkit使用 Teams SDK，请向代码添加脚本中的引用：

```HTML
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

# <a name="npm"></a>[npm](#tab/npm)
通过 ES6 模块使用工具包可以完全控制捆绑过程，并允许仅捆绑应用程序所需的代码。 若要使用 ES6 模块，请为项目添加 Toolkit 和 Microsoft Teams SDK 的 npm 包：

```cmd
npm install @microsoft/teams-js @microsoft/mgt-element @microsoft/mgt-teams-msal2-provider @microsoft/mgt-components
```

---

## <a name="create-the-auth-popup-page"></a>创建身份验证弹出页

除非你的应用程序事先获得管理员同意，否则你的用户可能需要同意权限。 若要启用此功能，你需要提供一个页面，Teams应用将在弹出窗口中打开该页面，以遵循身份验证流程。 只要页面与应用位于同一域中，就可以将页面路径 (，例如， https://yourdomain.com/tabauth)。 此页面的唯一要求是调用 方法 `TeamsMsal2Provider.handleAuth()` ，但您可以添加任何内容或加载您想要的进度。


下面是处理弹出窗口中的身份验证流的基本页面示例。

# <a name="unpkg"></a>[unpkg](#tab/unpkg)
```HTML
<!DOCTYPE html>
<html>
  <head>
    <script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
    <script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
  </head>

  <body>
    <script>
      mgt.TeamsMsal2Provider.handleAuth();
    </script>
  </body>
</html>
```
# <a name="npm"></a>[npm](#tab/npm)
```JavaScript
import { TeamsMsal2Provider } from '@microsoft/mgt-teams-msal2-provider';

TeamsMsal2Provider.handleAuth();
```

---

## <a name="creating-an-appclient-id"></a>创建应用/客户端 ID
您的选项卡需要作为注册的 Azure AD 运行，才能从应用程序获取Azure AD。 在租户中注册应用程序，并Microsoft Teams代表它获取访问令牌的权限：

1. 打开浏览器并转到Azure Active Directory[中心](https://aad.portal.azure.com)。 使用 Microsoft 帐户 **或工作** (帐户) **个人帐户登录**。

1. 在左窗格中，选择"**Azure Active Directory"，** 然后选择"**应用注册** 下选择 **"管理"**。

1. 选择“新注册”。 在“**注册应用程序**”页上，按如下方式设置值：

    - 将 **"** 名称 `Node.js Teams SSO` (选项的名称或) 。
    - 将“**受支持的帐户类型**”设置为“**任何组织目录中的帐户和个人 Microsoft 帐户**”。
    - 在 **"重定向 URI**"下，将第一个 `Single Page Application` 下拉列表设置为 ，将值设置为在上一步中创建的身份验证页面 URL;例如， `https://myapp.ngrok.io/tabauth`。 

1. 从应用概述页面中，复制 **Application (客户端) ID** 的值，供以后使用。 在创建新提供程序和后端时，将需要此值。

1. 在 **"管理**"下，转到" **证书&密码"**。 选择“新客户端密码”按钮。 在“**说明**”中输入值，并选择“**过期**”下的一个选项，再选择“**添加**”。

1. 离开此页前，先复制客户端密码值。 对于后端服务，你将需要它。

    >[!IMPORTANT]
    >此客户端密码不会再次显示，所以请务必现在就复制它。

1. 在 **"管理**"下，转到 **"API 权限"**。 选择 **"添加权限** > **Microsoft Graph** > **委派权限"**，然后添加以下权限：`email``profile``offline_access``openid`、、。 `User.Read` 选择 **添加权限**。

1.  (可选) 如果要预先同意任何其他范围，可以添加更多权限。 如果你使用不同的组件或计划使用其他 Microsoft Graph API，可能需要其他权限。 有关所需权限的详细信息，请参阅 [每个组件](../overview.md) 的文档。

    - 若要以管理员角色预先同意，请选择" **授予管理员同意"**，然后选择"是 **"**。

1.  在 **"管理**"下，转到 **"公开 API"**。 在页面顶部，选择"设置"旁边的`Application ID URI`**"设置"**。 这将生成一个 API，格式为： `api://{AppID}`。 更新它以添加子域;例如， `api://myapp.ngrok.io/{appID}`。

1. 在同一页上，选择 **"添加范围"**。 按如下所示填写字段，然后选择" **添加范围"**：

    - 范围名称： `access_as_user`
    - Who同意？：**管理员和用户**
    - 管理员同意显示名称： `Teams can access the user’s profile`
    - 管理员同意说明： `Allows Teams to call the app’s web APIs as the current user`
    - 用户同意显示名称： `Teams can access the user profile and make requests on the user's behalf`
    - 用户同意说明： `Enable Teams to call this app’s APIs with the same rights as the user.`
    - 状态： **已启用**
    
    你的 API URL 应如下所示： `api://myapp.ngrok.io/{appID}/access_as_user`。 

1. 接下来，添加两个客户端应用程序。 这适用于Teams/移动客户端和 Web 客户端。 在" **授权客户端应用程序"** 部分，选择 **"添加客户端应用程序"**。 填写客户端 ID 并选择你创建的范围。 然后选择" **添加应用程序"**。 对以下 ID 执行下列操作：
    
    - 5e3ce6c0-2b1f-4285-8d4b-75ee78787346
    - 1fec8e78-bce4-4aaf-ab1b-5451cc387264

## <a name="create-the-backend"></a>创建后端

后端可以是允许使用令牌交换 Microsoft Teams 身份验证令牌的任何后端，该令牌可用于通过Graph流调用 Microsoft [身份验证令牌。](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) 

有关参考，请参阅 Teams [SSO 节点示例](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/samples/teams-sso-node)。

下面是节点 express 服务器的参考实现：

```TypeScript
import dotenv from 'dotenv';
import express from 'express';
import path from 'path';
import * as msal from '@azure/msal-node';
import { NextFunction, Request, Response } from 'express';
import jwt, { JwtHeader, SigningKeyCallback } from 'jsonwebtoken';
import jwksClient from 'jwks-rsa';
import jwt_decode from 'jwt-decode';

// Load .env file
dotenv.config();

/**
 * Validates a JWT
 * @param {Request} req - The incoming request
 * @param {Response} res - The outgoing response
 * @returns {Promise<string | null>} - Returns the token if valid, returns null if invalid
 */
function validateJwt(req: Request, res: Response, next: NextFunction): void {
  const authHeader = req.headers.authorization!;
  const ssoToken = authHeader.split(' ')[1];
  if (ssoToken) {
    const validationOptions = {
      audience: process.env.CLIENT_ID,
    };
    jwt.verify(ssoToken, getSigningKey, validationOptions, (err, payload) => {
      if (err) {
        return res.sendStatus(403);
      }
      next();
    });
  } else {
    res.sendStatus(401);
  }
}

/**
 * Parses the JWT header and retrieves the appropriate public key
 * @param {JwtHeader} header - The JWT header
 * @param {SigningKeyCallback} callback - Callback function
 */
function getSigningKey(header: JwtHeader, callback: SigningKeyCallback): void {
  const client = jwksClient({
    jwksUri: 'https://login.microsoftonline.com/common/discovery/keys'
  });
  client.getSigningKey(header.kid!, (err, key) => {
    if (err) {
      callback(err, undefined);
    } else {
      callback(null, key.getPublicKey());
    }
  });
}

/**
 * Gets an access token for the user using the on-behalf-of flow
 * @param authHeader - The Authorization header value containing a JWT bearer token
 * @returns {Promise<string | null>} - Returns the access token if successful, null if not
 */
async function getAccessTokenOnBehalfOf(req: Request, res: Response): Promise<void> {
  // The token has already been validated, just grab it
  const authHeader = req.headers.authorization!;
  const ssoToken = authHeader.split(' ')[1];

  // Create an MSAL client
  const msalClient = new msal.ConfidentialClientApplication({
    auth: {
      clientId: req.body.clientid,
      clientSecret: process.env.APP_SECRET
    }
  });

  try {
    const result = await msalClient.acquireTokenOnBehalfOf({
      authority: `https://login.microsoftonline.com/${jwt_decode<any>(ssoToken).tid}`,
      oboAssertion: ssoToken,
      scopes: req.body.scopes,
      skipCache: true
    });
    res.json({ access_token: result?.accessToken });
  } catch (error) {
    if (error.errorCode === 'invalid_grant' || error.errorCode === 'interaction_required') {
      // This is expected if it's the user's first time running the app ( user must consent ) or the admin requires MFA
      res.status(403).json({ error: 'consent_required' }); // This error triggers the consent flow in the client.
    } else {
      // Unknown error
      res.status(500).json({ error: error.message });
    }
  }
}

////////////////////////
// create and run server
////////////////////////

const app = express();
const PORT = process.env.port || process.env.PORT || 8000;

// Support JSON payloads
app.use(express.json());
app.use(express.static(path.join(__dirname, 'client')));

// An example for using POST and with token validation using middleware
app.post('/api/token', validateJwt, async (req, res) => {
  await getAccessTokenOnBehalfOf(req, res);
});

app.listen(PORT, () => {
  console.log(`⚡️[server]: Server is running at http://localhost:${PORT}`);
});
```

## <a name="initialize-the-teams-msal2-provider"></a>初始化 MSAL2 Teams

Microsoft Graph Toolkit提供程序启用身份验证并访问 Microsoft Graph。 若要了解详细信息，请参阅[使用提供程序](../providers/providers.md)。 [MSAL2 Teams处理](../providers/teams-msal2.md)需要通过 Teams SDK 实现以对用户进行身份验证的所有逻辑和交互。

对于 SSO 模式，请确保提供 `sso-url` / `ssoUrl` 并指向后端 API。

# <a name="html"></a>[HTML](#tab/HTML)

`mgt-teams-msal2-provider`在 HTML 中添加 。

```HTML
<mgt-teams-msal2-provider 
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/tabauth"
  scopes="User.Read,Mail.ReadBasic"
  sso-url="http://localhost:8000/api/token"
  http-method="POST"
  ></mgt-teams-msal2-provider>
```

将 `<YOUR_CLIENT_ID>` 替换为应用程序的客户端 ID `auth-popup-url` `sso-url` ，将 替换为身份验证页面的完整路径或相对路径，将 替换为后端服务的完整路径或相对路径。

# <a name="javascript"></a>[JavaScript](#tab/JavaScript)

若要在 JavaScript 代码中初始化提供程序，请导入 `TeamsMsal2Provider` 并设置 `globalProvider`。

```TypeScript
import {Providers} from '@microsoft/mgt-element';
import {TeamsMsal2Provider, HttpMethod} from '@microsoft/mgt-teams-msal2-provider';
import * as MicrosoftTeams from "@microsoft/teams-js";

TeamsMsal2Provider.microsoftTeamsLib = MicrosoftTeams;

Providers.globalProvider = new TeamsMsal2Provider({
  clientId: `<YOUR_CLIENT_ID>`,
  authPopupUrl: '/tabauth',
  scopes: ['User.Read','Mail.ReadBasic'],
  ssoUrl: 'http://localhost:8000/api/token',
  httpMethod: HttpMethod.POST
});
```
将 `<YOUR_CLIENT_ID>` 替换为应用程序的客户端 ID `authPopupUrl` `ssoUrl` ，将 替换为身份验证页面的完整路径或相对路径，将 替换为后端服务的完整路径或相对路径。

---

## <a name="add-components"></a>添加组件

现在，你已准备好添加任何 Microsoft Graph Toolkit组件。 

您可以像平常一样向 HTML 添加组件。 例如，若要添加组件 `Person` ，请向 HTML 中添加以下代码。

```HTML
<mgt-person person-query="me"></mgt-person>
```

如果你使用的是 React，我们建议改为React库中的组件`mgt-react`。 若要了解更多信息，请参阅[将 Microsoft Graph Toolkit与 React](./use-toolkit-with-react.md)。

## <a name="test-the-sample"></a>测试示例
有关完整实现，请参阅 Teams [SSO 节点示例](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/samples/teams-sso-node)。

如果所有内容都配置正确 `Person` ，你将看到呈现的组件无需登录。
>[!IMPORTANT]
>如果尚未预先同意，可能需要通过提示同意。

## <a name="next-steps"></a>后续步骤
- 在[样本](https://mgt.dev)中试用组件。
- 在 [Microsoft 问答中&问题](/answers/topics/microsoft-graph-toolkit.html)。
- 在 [GitHub](https://aka.ms/mgt) 上报告 bug 或提出功能请求。
