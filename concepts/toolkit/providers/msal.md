---
title: MSAL 提供商
description: MSAL 提供程序MSAL.js登录用户并获取与 Microsoft Graph 一同使用的令牌
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 738e8ebcd24b3e7e528bdf0a1676dd54103ee2ea
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883023"
---
# <a name="msal-provider"></a>MSAL 提供商

MSAL [ 提供程序MSAL.js登录 ](https://github.com/AzureAD/microsoft-authentication-library-for-js) 用户并获取与 Microsoft Graph 一同使用的令牌。

若要了解更多信息，请参阅 [提供程序](./providers.md)。

## <a name="get-started"></a>入门

可以使用 HTML 或 JavaScript 初始化 MSAL 提供程序。

### <a name="initialize-in-your-html-page"></a>在 HTML 页中初始化

以 HTML 格式初始化 MSAL 提供程序是创建新提供程序的最简单方法。 使用该 `mgt-msal-provider` 组件设置 **客户端 ID** 和其他属性。 这将创建一 `UserAgentApplication` 个新实例，该实例将用于所有身份验证和获取令牌。

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   redirect-uri="https://my.redirect/uri"
                   authority=""></mgt-msal-provider>
```

| 属性    | 说明                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| client-id    | 字符串客户端 ID (请参阅创建应用/客户端 ID) 。 必需。                                                                                                                                                                                                           |
| login-type   | 与 - `redirect` `popup` 默认值之间的枚举为 `redirect` 。 可选。                                                                                                                                                                                   |
| scopes       | 用户登录时必须同意的范围的逗号分隔字符串。 可选。                                                                                                                                                                                     |
| authority    | 颁发机构字符串 - 默认为公用颁发机构。 对于单租户应用，请使用租户 ID 或租户名称。 例如， `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` 或 `https://login.microsoftonline.com/[your-tenant-id]` 。 可选。 |
| redirect-uri | 重定向 URI 字符串 - 默认情况下，使用当前窗口 URI。 可选。                                                                                                                                                                                            |
| depends-on   | 另一个优先级较高的提供程序组件的元素选择器字符串。 可选。                                                                                                                                                                                      |

### <a name="initialize-in-javascript"></a>在 JavaScript 中初始化

可以通过在 JavaScript 中初始化提供程序提供更多选项。

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

可以通过两 `MsalProvider` 种方式配置构造函数参数，如以下各节所述。

#### <a name="provide-a-clientid-to-create-a-new-useragentapplication"></a>提供 `clientId` 用于创建新 `UserAgentApplication`

当 Graph Toolkit负责应用程序中的所有身份验证时，此选项有意义。

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

#### <a name="pass-an-existing-useragentapplication-in-the-useragentapplication-property"></a>传递属性 `UserAgentApplication` 中的 `userAgentApplication` 现有属性。

当你的应用使用 MSAL 功能超过由 Microsoft Graph 和其他 Microsoft Graph 功能公开的功能 `MsalProvider` 时，Toolkit此功能。 当框架自动实例化并公开 a 时，这尤其适用;例如，使用 `UserAgentApplication` [msal-angular 时](/azure/active-directory/develop/tutorial-v2-angular)。

请务必了解使用此选项时发生冲突的机会。 从本质上说，存在更改会话状态的风险，例如，让用户登录或同意其他 `MsalProvider` 范围。 请确保你的应用和其他框架在状态中流畅地响应这些更改，或考虑改为使用 [自定义提供程序](./custom.md) 。

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

若要详细了解如何注册应用和获取客户端 ID，请参阅"创建[Azure Active Directory 应用"。](../get-started/add-aad-app-registration.md)