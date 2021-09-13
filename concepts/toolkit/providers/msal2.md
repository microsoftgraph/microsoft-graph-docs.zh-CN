---
title: MSAL2 提供程序
description: MSAL 2 提供程序使用 msal-browser 登录用户并获取令牌以与 Microsoft Graph
ms.localizationpriority: medium
author: amrutha95
ms.openlocfilehash: 80178f379d0f6d9101cec794bc1d0d36ccb640d7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143480"
---
# <a name="msal2-provider"></a>MSAL2 提供程序

MSAL2 提供程序使用[msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser)登录用户并获取与 Microsoft Graph 一Graph。

若要了解更多信息，请参阅 [提供程序](./providers.md)。

## <a name="difference-between-msal2-provider-and-msal-provider"></a>MSAL2 提供程序和 MSAL 提供程序的区别
尽管用法相似，但 MSAL 提供程序和 MSAL2 提供程序构建在不同的 OAuth 流上。 MSAL 提供程序基于实现 OAuth2.0 隐式msal.js构建[于](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)Flow。 MSAL2 提供程序基于[msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser)构建，它使用 PKCE 实现 OAuth 2.0 授权[Flow](/azure/active-directory/develop/v2-oauth2-auth-code-flow)代码。
由于授权代码Flow Web 应用程序的隐式授权Flow，因此我们建议使用 Msal2Provider 而不是 MsalProvider。 有关与隐式授予流相关的安全问题的详细信息，请参阅 [隐式流的缺点](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6)。

所有新应用程序应尽可能使用 MSAL2 提供程序。 

## <a name="get-started"></a>入门

可以使用 HTML 或 JavaScript 初始化 MSAL2 提供程序。

### <a name="initialize-in-your-html-page"></a>在 HTML 页中初始化

使用 HTML 初始化 MSAL2 提供程序是创建新提供程序的最简单方法。 使用该 `mgt-msal2-provider` 组件设置 **client-id** 和其他属性。 这将创建一 `PublicClientApplication` 个将用于所有身份验证和获取令牌的新实例。

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
| client-id    | 字符串客户端 ID (请参阅创建应用/客户端 ID) 。 必填。                                                                                                                                                                                                           |
| login-type   | 和 之间的 `redirect` `popup` 枚举 - 默认值为 `redirect` 。 可选。                                                                                                                                                                                   |
| scopes       | 用户登录时必须同意的范围的逗号分隔字符串。 可选。                                                                                                                                                                                     |
| authority    | 颁发机构字符串 - 默认为公共颁发机构。 对于单租户应用，请使用租户 ID 或租户名称。 例如， `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` `https://login.microsoftonline.com/[your-tenant-id]` 或 。 可选。 |
| redirect-uri | 重定向 URI 字符串 - 默认情况下，使用当前窗口 URI。 可选。                                                                                                                                                                                            |
| 提示       | 用于登录的提示类型，介于 ```SELECT_ACCOUNT``` 和 ```CONSENT``` ```LOGIN``` 之间。 默认值为 ```SELECT_ACCOUNT```。 可选。

### <a name="initialize-in-javascript"></a>在 JavaScript 中初始化

可以通过在 JavaScript 中初始化提供程序来提供更多选项。

```ts
    import {Providers} from '@microsoft/mgt-element';
    import {Msal2Provider, Msal2Config, Msal2PublicClientApplicationConfig} from '@microsoft/mgt-msal2-provider';

    // initialize the auth provider globally
    Providers.globalProvider = new Msal2Provider(config: Msal2Config | Msal2PublicClientApplicationConfig);
```

您可以通过两 `Msal2Provider` 种方式配置构造函数参数，如以下各节所述。

#### <a name="provide-a-clientid-to-create-a-new-publicclientapplication"></a>提供 `clientId` 以创建新 `PublicClientApplication`

当 Microsoft Graph Toolkit负责应用程序中的所有身份验证时，此选项有意义。

```ts
interface Msal2Config {
  clientId: string;
  scopes?: string[];
  authority?: string;
  redirectUri?: string;
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  prompt?: PromptType; // PromptType.CONSENT, PromptType.LOGIN or PromptType.SELECT_ACCOUNT
  sid?: string; // Session ID
  loginHint?: string;
  domainHint?: string;
  options?: Configuration // msal-browser Configuration object
}
```

#### <a name="pass-an-existing-publicclientapplication-in-the-publicclientapplication-property"></a>在 属性 `PublicClientApplication` 中传递 `publicClientApplication` 现有的 。

当你的应用使用 MSAL 功能时，除了由 Microsoft 公开的功能和其他 Microsoft Graph Toolkit `Msal2Provider` 此功能。 当框架自动实例化 并公开 时，这尤其适用;例如， `PublicClientApplication` 使用 [msal-angular 时](/azure/active-directory/develop/tutorial-v2-angular)。 有关进一步指导，请参阅 `angular-app` Microsoft Graph Toolkit[中的示例](https://github.com/microsoftgraph/microsoft-graph-toolkit)。

请务必了解使用此选项时发生冲突的机会。 从本质上说，存在可以更改会话状态的风险;例如，让用户登录或同意其他 `Msal2Provider` 范围。 请确保应用和其他框架在状态中流畅地响应这些更改，或考虑改为使用 [自定义提供程序](./custom.md) 。

```ts
interface Msal2PublicClientApplicationConfig {
  publicClientApplication: PublicClientApplication;
  scopes?: string[];
  authority?: string;
  redirectUri?: string;
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  prompt?: PromptType; // PromptType.CONSENT, PromptType.LOGIN or PromptType.SELECT_ACCOUNT
  sid?: string; // Session ID
  loginHint?: string;
  domainHint?: string;
  options?: Configuration // msal-browser Configuration object
}
```

## <a name="creating-an-appclient-id"></a>创建应用/客户端 ID

若要详细了解如何注册应用和获取客户端 ID，请参阅创建Azure Active Directory[应用](../get-started/add-aad-app-registration.md)。

## <a name="migrating-from-msal-provider-to-msal2-provider"></a>从 MSAL 提供程序迁移到 MSAL2 提供程序
若要将使用 MSAL 提供程序的应用程序迁移到 MSAL2 提供程序：
1. 转到 Azure 门户，位于 https://portal.azure.com 。
1. 从菜单中，选择 **"Azure Active Directory"。**
1. 从"Azure Active Directory"菜单中，选择 **"应用注册"。**
1. 选择当前使用的应用的应用注册。 
1. 转到左侧 **菜单** 上的"身份验证"。
1. 在 **"平台配置"** 下，单击 **"添加平台"，** 然后选择 **"单页应用程序"。**
1. 删除当前在 **Web** 下注册的所有重定向 URI，并改为将它们添加到 **单页应用程序 下**。
1. 在代码中，将 替换为 `MSALProvider` `MSAL2Provider` 。

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
