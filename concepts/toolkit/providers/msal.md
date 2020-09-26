---
title: MSAL 提供商
description: MSAL 提供程序使用 MSAL.js 登录用户并获取令牌以用于 Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: c3c921cfa473e2001d2a150096741d2bddf39f10
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288159"
---
# <a name="msal-provider"></a>MSAL 提供商

MSAL 提供程序使用 [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) 登录用户并获取令牌以用于 Microsoft Graph。

若要了解详细信息，请参阅 [提供程序](../providers.md)。

## <a name="get-started"></a>入门

您可以初始化 HTML 或 JavaScript 中的 MSAL 提供程序。

### <a name="initialize-in-your-html-page"></a>在 HTML 页面中初始化

若要在 HTML 中初始化 MSAL 提供程序，最简单的方法是创建新的提供程序。 使用 `mgt-msal-provider` 组件设置 **客户端 id** 和其他属性。 这将创建一个 `UserAgentApplication` 将用于所有身份验证和获取令牌的新实例。

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   redirect-uri="https://my.redirect/uri"
                   authority=""></mgt-msal-provider>
```

| 属性    | 说明                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 客户端 id    | 字符串客户端 ID (请参阅创建应用/客户端 ID) 。 必需。                                                                                                                                                                                                           |
| 登录类型   | `redirect`和 `popup` -默认值之间的枚举为 `redirect` 。 可选。                                                                                                                                                                                   |
| scopes       | 用户必须同意登录时的作用域的逗号分隔字符串。 可选。                                                                                                                                                                                     |
| 监管    | 颁发机构字符串-默认为常用证书颁发机构。 对于单租户应用，请使用租户 ID 或租户名称。 例如， `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` 或 `https://login.microsoftonline.com/[your-tenant-id]` 。 可选。 |
| 重定向-uri | 重定向 URI 字符串-默认情况下，使用当前窗口 URI。 可选。                                                                                                                                                                                            |
| 取决于   | 另一个较高优先级提供程序组件的元素选择器字符串。 可选。                                                                                                                                                                                      |

### <a name="initialize-in-javascript"></a>在 JavaScript 中初始化

您可以通过在 JavaScript 中初始化提供程序来提供更多选项。

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

其中 MsalConfig 是：

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  redirectUri?: string;
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string
  options?: Configuration; // msal js Configuration object
}
```

您必须提供 `clientId` (才能创建新 `UserAgentApplication`) 。

若要详细了解 MSAL.js 以及在初始化 MSAL 库时可使用的其他选项，请参阅 [MSAL 文档](/azure/active-directory/develop/msal-js-initializing-client-applications)。

## <a name="creating-an-appclient-id"></a>创建应用/客户端 ID

有关如何注册应用并获取客户端 ID 的详细信息，请参阅 [注册应用程序快速入门](/azure/active-directory/develop/quickstart-register-app)。

>**注意：** MSAL 仅支持 OAuth 的隐式流。 请务必在 Azure 门户中的应用程序中启用隐式流， (默认情况下不启用它) 。 在 " **身份验证**" 下，找到 " **隐式授予** " 部分，然后选择 " **访问令牌** " 和 **ID 令牌**的复选框。 若要使用公共证书颁发机构，请 **在任何组织目录中设置帐户**。 若要使用特定租户，请在 `authority` 初始化过程中设置。