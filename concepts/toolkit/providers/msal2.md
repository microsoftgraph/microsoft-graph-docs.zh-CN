---
title: MSAL 2 提供商
description: MSAL 2 提供程序使用 msal-browser 登录用户并获取令牌以用于 Microsoft Graph
localization_priority: Normal
author: amrutha95
ms.openlocfilehash: f856c900b0b8aace7a1c2248d2921b39fe0a2c44c6fc9e05c35003c0d0c53d50
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54204905"
---
# <a name="msal-2--provider"></a>MSAL 2 提供程序

MSAL 2 提供程序使用[msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser)登录用户并获取与 Microsoft Graph 一Graph。
若要了解更多信息，请参阅 [提供程序](./providers.md)。

## <a name="get-started"></a>入门

可以使用 HTML 或 JavaScript 初始化 MSAL 2.0 提供程序。

### <a name="initialize-in-your-html-page"></a>在 HTML 页中初始化

使用 HTML 初始化 MSAL 2 提供程序是创建新提供程序的最简单方法。 使用该 `mgt-msal2-provider` 组件设置 **client-id** 和其他属性。 这将创建一 `PublicClientApplication` 个将用于所有身份验证和获取令牌的新实例。

```html
    <mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"
                        login-type="redirect/popup" 
                        scopes="user.read,people.read" 
                        redirect-uri="https://my.redirect/uri" 
                        authority=""> 
    </mgt-msal2-provider> 
```

| 属性    | 说明                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| client-id    | 字符串客户端 ID (创建应用/客户端 ID) 。 必填。                                                                                                                                                                                                           |
| login-type   | 和 之间的 `redirect` `popup` 枚举 - 默认值为 `redirect` 。 可选。                                                                                                                                                                                   |
| scopes       | 用户登录时必须同意的范围的逗号分隔字符串。 可选。                                                                                                                                                                                     |
| authority    | 颁发机构字符串 - 默认为公共颁发机构。 对于单租户应用，请使用租户 ID 或租户名称。 例如， `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` `https://login.microsoftonline.com/[your-tenant-id]` 或 。 可选。 |
| redirect-uri | 重定向 URI 字符串 - 默认情况下，使用当前窗口 URI。 可选。                                                                                                                                                                                            |
| 提示       | 用于登录的提示类型，介于 ```SELECT_ACCOUNT``` 和 ```CONSENT``` 之间 ```LOGIN``` 。 默认值为“```SELECT_ACCOUNT```”。 可选。

### <a name="initialize-in-javascript"></a>在 JavaScript 中初始化

可以通过在 JavaScript 中初始化提供程序来提供更多选项。

```ts
    import {Providers, LoginType} from '@microsoft/mgt-element';
    import {Msal2Provider, PromptType} from '@microsoft/mgt-msal2-provider';

    // initialize the auth provider globally
    Providers.globalProvider = new Msal2Provider({
      clientId: 'REPLACE_WITH_CLIENTID',
      scopes?: string[],
      authority?: string,
      redirectUri?: string,
      loginType?: LoginType, // LoginType.Popup or LoginType.Redirect (redirect is default)
      prompt?: PromptType, // PromptType.CONSENT, PromptType.LOGIN or PromptType.SELECT_ACCOUNT
      sid?: string, // Session ID
      loginHint?: string,
      domainHint?: string,
      options?: Configuration // msal js Configuration object
    });
```

## <a name="creating-an-appclient-id"></a>创建应用/客户端 ID

若要详细了解如何注册应用和获取客户端 ID，请参阅创建Azure Active Directory[应用](../get-started/add-aad-app-registration.md)。

## <a name="difference-between-msal2provider-and-msalprovider"></a>Msal2Provider 和 MsalProvider 的区别
尽管用法非常相似，但 MsalProvider 和 Msal2Provider 是在不同的 OAuth 流上构建的。 MsalProvider 基于实现 OAuth2.0 [](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)隐式MSAL.js构建于 Flow。 Msal2Provider 基于[msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser)构建，它使用 PKCE 实现 OAuth 2.0 授权[Flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow)代码。
授权代码Flow Web 应用程序的隐式授权Flow，因此我们建议使用 MSAL2Provider 而不是 MSALProvider。 有关与隐式授予流相关的安全问题的详细信息，请参阅 [隐式流的缺点](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6)。

## <a name="migrating-from-msal-provider-to-msal-2-provider"></a>从 MSAL 提供程序迁移到 MSAL 2 提供程序
若要将使用 MSAL 提供程序的应用程序迁移到 MSAL 2 提供程序：
1. 转到 Azure 门户，位于 https://portal.azure.com 。
1. 从菜单中，选择 **"Azure Active Directory"。**
1. 从"Azure Active Directory"菜单中，选择 **"应用注册"。**
1. 选择当前使用的应用的应用注册。 
1. 转到左侧 **菜单** 上的"身份验证"。
1. 在 **"平台配置"** 下，单击 **"添加平台"，** 然后选择 **"单页应用程序"。**
1. 删除当前在 **Web** 下注册的所有重定向 URI，并改为将它们添加到 **单页应用程序 下**。
1. 在你的代码中，将 MSALProvider 替换为 MSAL2Provider。

    如果要在 JS/TS 代码中初始化提供程序，请按照以下步骤操作：
    
    将 的 import 语句 ```mgt-msal-provider``` 替换为 
    ```ts 
    import {Msal2Provider, PromptType} from '@microsoft/mgt-msal2-provider';
    ```

    将 MsalProvider 的初始化替换为
    ```ts
    Providers.globalProvider = new Msal2Provider({ 
      clientId: 'REPLACE_WITH_CLIENTID'
      ...
    })
    ```
    如果以 HTML 格式初始化提供程序，请替换 
    ```html
    <mgt-msal-provider client-id="" ... ></mgt-msal-provider>
    ``` 
    with 
    ```html
    <mgt-msal2-provider  client-id="" ... ></mgt-msal2-provider>
     ```
    有关详细信息，请参阅[HTML 页面中的 Initialize。](#initialize-in-your-html-page)
