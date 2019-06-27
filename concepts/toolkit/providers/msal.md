---
title: MSAL 提供程序
description: MSAL 提供程序使用 MSAL 来登录用户并获取令牌以用于 Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b66fd9a640c6baa84767e1ab08821b80384a5464
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242965"
---
# <a name="msal-provider"></a>MSAL 提供程序

MSAL 提供程序使用[MSAL](https://github.com/AzureAD/microsoft-authentication-library-for-js)来登录用户并获取令牌以用于 Microsoft Graph。

若要了解详细信息, 请参阅[提供程序](../providers.md)。

## <a name="get-started"></a>入门

您可以初始化 HTML 或 JavaScript 中的 MSAL 提供程序。

### <a name="initialize-in-your-html-page"></a>在 HTML 页面中初始化

若要在 HTML 中初始化 MSAL 提供程序, 最简单的方法是创建新的提供程序。 使用`mgt-msal-provider`组件设置**客户端 id**和其他属性。 这将创建一个将`UserAgentApplication`用于所有身份验证和获取令牌的新实例。

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   authority=""></mgt-msal-provider>
```

>**注意:**`login-type`和`authority`是可选的。

### <a name="initialize-in-javascript"></a>在 JavaScript 中初始化

您可以通过在 JavaScript 中初始化提供程序来提供更多选项。

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

其中 MsalConfig 是:

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  loginType?: LoginType;
  options?: Configuration; // msal js Configuration object
}
```

您必须提供`clientId` (以创建新`UserAgentApplication`的)。

若要了解详细信息, 请参阅[MSAL 文档](https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics)。

## <a name="creating-an-appclient-id"></a>创建应用/客户端 ID

有关如何注册应用并获取客户端 ID 的详细信息, 请参阅[注册应用程序快速入门](https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-register-app)。

>**注意:** MSAL 仅支持 OAuth 的隐式流。 请确保在 Azure 门户中的应用程序中启用隐式流 (默认情况下不启用)。 在 "**身份验证**" 下, 找到 "**隐式授予**" 部分, 然后选择 "**访问令牌**" 和**ID 令牌**的复选框。
