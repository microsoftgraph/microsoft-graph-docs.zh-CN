---
title: MSAL 提供程序
description: MSAL 提供程序使用 MSAL.js 登录用户并获取与 Microsoft Graph 一Graph。
ms.localizationpriority: medium
author: nmetulev
ms.openlocfilehash: 5c9c3d8fc416f08b0386335aa518076e256fe0ad
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143550"
---
# <a name="msal-provider"></a>MSAL 提供程序

MSAL 提供程序[使用msal.js](https://github.com/AzureAD/microsoft-authentication-library-for-js)登录用户并获取与 Microsoft Graph 一Graph。

若要了解更多信息，请参阅 [提供程序](./providers.md)。

## <a name="difference-between-msal2-provider-and-msal-provider"></a>MSAL2 提供程序和 MSAL 提供程序的区别
尽管用法相似，但 MSAL 提供程序和 MSAL2 提供程序构建在不同的 OAuth 流上。 MSAL 提供程序基于实现 OAuth2.0 隐式msal.js构建[于](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)Flow。 MSAL2 提供程序基于[msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser)构建，它使用 PKCE 实现 OAuth 2.0 [Flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow)代码。
由于授权代码Flow Web 应用程序的隐式授权Flow，因此我们建议通过 MSAL Provider 使用 MSAL2 提供程序。 有关与隐式授予流相关的安全问题的详细信息，请参阅 [隐式流的缺点](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6)。

所有新应用程序应尽可能使用 MSAL2 提供程序。 有关迁移信息，请参阅[MSAL2 Provider。](./msal2.md)

## <a name="get-started"></a>入门

可以使用 HTML 或 JavaScript 初始化 MSAL 提供程序。

### <a name="initialize-in-your-html-page"></a>在 HTML 页中初始化

使用 HTML 初始化 MSAL 提供程序是创建新提供程序的最简单方法。 使用该 `mgt-msal-provider` 组件设置 **client-id** 和其他属性。 这将创建一 `UserAgentApplication` 个将用于所有身份验证和获取令牌的新实例。

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   redirect-uri="https://my.redirect/uri"
                   authority=""
                   domainHint="mydomain.com"
                   prompt="consent"></mgt-msal-provider>
```

| 属性    | 说明                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| client-id    | 字符串客户端 ID (请参阅创建应用/客户端 ID) 。 必需。                                                                                                                                                                                                           |
| login-type   | 和 之间的 `redirect` `popup` 枚举 - 默认值为 `redirect` 。 可选。                                                                                                                                                                                   |
| scopes       | 用户登录时必须同意的范围的逗号分隔字符串。 可选。                                                                                                                                                                                     |
| authority    | 颁发机构字符串 - 默认为公共颁发机构。 对于单租户应用，请使用租户 ID 或租户名称。 例如， `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` `https://login.microsoftonline.com/[your-tenant-id]` 或 。 可选。 |
| redirect-uri | 重定向 URI 字符串 - 默认情况下，使用当前窗口 URI。 可选。                                                                                                                                                                                            |
| depends-on   | 另一个优先级较高的提供程序组件的元素选择器字符串。 可选。 
| 域提示  | 用于转发登录体验的域位置的查询字符串。 可选。              
| 提示 | 选择登录所需的用户交互类型。 有效选项包括： <ul><li>`login` 强制用户在请求时输入凭据 </li><li>`none` 无交互提示</li> <li>`select_account` 将用户发送到帐户选取器</li><li>`consent` 将用户发送到 OAuth 同意对话框</li></ul> 有关更多提示信息，请参阅本文 [中的MSAL.js](/azure/active-directory/develop/msal-js-prompt-behavior) 行为。 可选。                                                                                                                                                                            |


### <a name="initialize-in-javascript"></a>在 JavaScript 中初始化

可以通过在 JavaScript 中初始化提供程序来提供更多选项。

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

您可以通过两 `MsalProvider` 种方式配置构造函数参数，如以下各节所述。

#### <a name="provide-a-clientid-to-create-a-new-useragentapplication"></a>提供 `clientId` 以创建新 `UserAgentApplication`

此选项在用户负责Graph Toolkit身份验证时有意义。

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  redirectUri?: string;
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string
  options?: Configuration; // msal js Configuration object
  domainHint?: string;
  prompt?: string; // "login", "none", "select_account", "consent"
}
```

#### <a name="pass-an-existing-useragentapplication-in-the-useragentapplication-property"></a>在 属性 `UserAgentApplication` 中传递 `userAgentApplication` 现有的 。

当你的应用使用 MSAL 功能时，除了由 Microsoft 公开的功能和其他 Microsoft Graph Toolkit `MsalProvider` 此功能。 当框架自动实例化 并公开 时，这尤其适用;例如， `UserAgentApplication` 使用 [msal-angular 时](/azure/active-directory/develop/tutorial-v2-angular)。

请务必了解使用此选项时发生冲突的机会。 从本质上说，存在可以更改会话状态的风险，例如，让用户登录或同意其他 `MsalProvider` 范围。 请确保应用和其他框架在状态中流畅地响应这些更改，或考虑改为使用 [自定义提供程序](./custom.md) 。

```ts
interface MsalConfig {
  userAgentApplication: UserAgentApplication;
  scopes?: string[];
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string;
}
```

若要详细了解MSAL.js以及初始化 MSAL 库时可以使用的其他选项，请参阅 [MSAL 文档](/azure/active-directory/develop/msal-js-initializing-client-applications)。

## <a name="creating-an-appclient-id"></a>创建应用/客户端 ID

若要详细了解如何注册应用和获取客户端 ID，请参阅创建Azure Active Directory[应用](../get-started/add-aad-app-registration.md)。
