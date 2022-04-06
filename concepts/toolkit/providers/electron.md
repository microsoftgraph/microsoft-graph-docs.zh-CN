---
title: 电子提供程序
description: 适用于 Insmicrosoft 的 MSAL 提供程序使用 msal-node 登录用户并获取与 Microsoft Graph 一Graph。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 34bc60842c9bd22ca79d9a36ce0aa31ef1168f7f
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589287"
---
# <a name="electron-provider"></a>电子提供程序

开发工具提供程序使用 [msal 节点](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-node)登录用户并获取令牌，以便与 Microsoft Graph应用程序一同使用。

若要了解有关身份验证提供程序的信息，请参阅 [提供程序](./providers.md)。

## <a name="get-started"></a>入门
### <a name="install-the-packages"></a>安装程序包

```bash
npm install @microsoft/mgt-element @microsoft/mgt-electron-provider
```
你需要在呈现器进程中初始化 (前端) ，在前端) 主进程中初始化 (Authenticator) 。


### <a name="initializing-electronprovider-in-the-renderer-process-rendererts"></a>在呈现器进程中 (Renderer.ts) 

在主进程) 中，将使用一个功能控制程序 (与一个操作者通信，以请求访问令牌，并接收组件正常工作所需的有关登录状态的信息。 

```ts
import {Providers} from '@microsoft/mgt-element';
import {ElectronProvider} from '@microsoft/mgt-electron-provider/dist/Provider';
import '@microsoft/mgt-components';

// initialize the auth provider globally
Providers.globalProvider = new ElectronProvider();
```

### <a name="initializing-electronauthenticator-in-the-main-process-maints"></a>在 main.ts (主进程中初始化一) 

为 MSAL 身份验证设置配置变量、获取访问令牌以及与一起与一起通信时，一直由一位用户负责使用一个配置变量。
在主进程中初始化一个为一个，然后设置 Client-id 等配置变量。

```ts
import { ElectronAuthenticator, MsalElectronConfig } from '@microsoft/mgt-electron-provider/dist/Authenticator'; 

let config: MsalElectronConfig = {
  clientId: '<your_client_id>',
  authority: '<your_authority_url>', //optional
  mainWindow: mainWindow, 
  scopes: ['user.read'] //We recommend pre-consenting all the required scopes on the Azure portal
};

ElectronAuthenticator.initialize(config);
```
 
| 属性   | 说明                                                                                                                                                                                                                                                           |
| ----------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| clientId    | 字符串客户端 ID (创建应用/客户端 ID) 。 必需项。                                                                                                                                                                                                           |
| scopes      | 用户必须同意登录的范围的逗号分隔字符串。 推荐。                                                                                                                                                                                  |
| authority   | 颁发机构字符串 - 默认为公共颁发机构。 对于单租户应用，请使用租户 ID 或租户名称。 例如，`https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` 或 `https://login.microsoftonline.com/[your-tenant-id]`。 可选。 |
| mainWindow  | 需要身份验证的主 BrowserWindow 的实例。                                                                                                                                                                                                      |
| cachePlugin | 要用于永久存储令牌的缓存插件。 请参阅 [Microsoft Authentication Extensions for Node](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/extensions/msal-node-extensions)。 可选。                       |

>**注意：** 目前，提供程序不支持增量支持。 作为最佳实践，请确保同意组件需要的所有范围。
    
## <a name="create-an-appclient-id"></a>创建应用/客户端 ID

### <a name="add-new-application-registration-in-azure-active-directory-to-get-a-client-id"></a>在客户端中添加新Azure Active Directory以获取客户端 ID

若要在应用程序中创建Azure Active Directory，请添加新的应用程序注册，然后配置应用名称和重定向 URI。

若要在应用中创建Azure Active Directory：

1. 转到“[Azure 门户](https://portal.azure.com)”。
1. 从菜单中，选择"Azure Active Directory **"**。
1. 从"Azure Active Directory"菜单中，选择"应用注册 **"**。
1. 从顶部菜单中，选择"新建 **注册"** 按钮。
1. 输入应用的名称;例如， `My Electron-App`。
1. 对于受支持的帐户类型 [](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)类型，选择任何组织目录中的帐户 (任何 Azure AD 目录 - 多租户 **) 和个人 Microsoft 帐户 (例如 Skype、Xbox)**。
1. In the **Redirect URI** field， in the dropdown， select **Public client/native (mobile & desktop)**， and in the URL field， enter `msal://redirect`.
1. 通过选择"注册" **按钮确认** 更改。

## <a name="next-steps"></a>后续步骤

* 查看有关生成一个电子应用 [分步教程](../get-started/build-an-electron-app.md)。
* 请看一个 [显示如何使用"](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/samples/electron-app) 开发工具"提供程序的示例"一些"开发应用程序"。
