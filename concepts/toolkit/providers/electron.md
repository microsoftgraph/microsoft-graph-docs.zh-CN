---
title: 提供商
description: Microsoft Graph 的 MSAL 提供程序使用 msal-node 登录用户并获取用于 Microsoft Graph 的令牌。
localization_priority: Normal
author: amrutha95
ms.openlocfilehash: a9e391f96988f8beaf8395e872a6efa08efca8f5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471426"
---
# <a name="electron-provider"></a><span data-ttu-id="4f8a9-103">提供商</span><span class="sxs-lookup"><span data-stu-id="4f8a9-103">Electron provider</span></span>

<span data-ttu-id="4f8a9-104">开发工具提供程序使用 [msal-node](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-node) 登录用户，并获取令牌以在一个更新应用程序中与 Microsoft Graph 一同使用。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-104">The Electron provider uses [msal-node](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-node) to sign in users and acquire tokens to use with Microsoft Graph in an Electron application.</span></span>

<span data-ttu-id="4f8a9-105">若要了解有关身份验证提供程序的信息，请参阅 [提供程序](./providers.md)。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-105">To learn more about authentication providers, see [providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="4f8a9-106">入门</span><span class="sxs-lookup"><span data-stu-id="4f8a9-106">Get started</span></span>
### <a name="install-the-packages"></a><span data-ttu-id="4f8a9-107">安装程序包</span><span class="sxs-lookup"><span data-stu-id="4f8a9-107">Install the packages</span></span>

```bash
npm install @microsoft/mgt-element @microsoft/mgt-electron-provider
```
<span data-ttu-id="4f8a9-108">你需要在呈现器进程中初始化（前端 () ）和在主进程中初始化 (和) 。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-108">You need to initialize ElectronProvider in the renderer process (front end), and ElectronAuthenticator in the main process (back end).</span></span>


### <a name="initializing-electronprovider-in-the-renderer-process-rendererts"></a><span data-ttu-id="4f8a9-109">在呈现器进程中初始化 RendererProvider (renderer.ts) </span><span class="sxs-lookup"><span data-stu-id="4f8a9-109">Initializing ElectronProvider in the renderer process (renderer.ts)</span></span>

<span data-ttu-id="4f8a9-110">在主进程) 中，为请求访问令牌和接收有关组件正常工作所需的已登录状态的信息，而该开发工具负责与 (。</a1></span><span class="sxs-lookup"><span data-stu-id="4f8a9-110">The ElectronProvider is responsible for communicating with ElectronAuthenticator (in the main process) to request access tokens and receive information regarding logged in state that are required for the components to work.</span></span> 

```ts
import {Providers} from '@microsoft/mgt-element';
import {ElectronProvider} from '@microsoft/mgt-electron-provider/dist/Provider';
import '@microsoft/mgt-components';

// initialize the auth provider globally
Providers.globalProvider = new ElectronProvider();
```

### <a name="initializing-electronauthenticator-in-the-main-process-maints"></a><span data-ttu-id="4f8a9-111">在 main.ts (主进程中初始化Authenticator) </span><span class="sxs-lookup"><span data-stu-id="4f8a9-111">Initializing ElectronAuthenticator in the main process (main.ts)</span></span>

<span data-ttu-id="4f8a9-112">一名用户负责设置 MSAL 身份验证的配置变量、获取访问令牌以及与一名用户通信。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-112">The ElectronAuthenticator is responsible for setting up the configuration variables for MSAL authentication, acquiring access tokens, and communicating with ElectronProvider.</span></span>
<span data-ttu-id="4f8a9-113">在主进程中初始化Authenticator，并设置配置变量，如客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-113">Initialize the ElectronAuthenticator in the main process and set up the configuration variables such as client-id.</span></span>

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
 
| <span data-ttu-id="4f8a9-114">属性</span><span class="sxs-lookup"><span data-stu-id="4f8a9-114">Attribute</span></span>    | <span data-ttu-id="4f8a9-115">说明</span><span class="sxs-lookup"><span data-stu-id="4f8a9-115">Description</span></span>                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4f8a9-116">clientId</span><span class="sxs-lookup"><span data-stu-id="4f8a9-116">clientId</span></span>    | <span data-ttu-id="4f8a9-117">字符串客户端 ID (请参阅创建应用/客户端 ID) 。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-117">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="4f8a9-118">必填。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-118">Required.</span></span>                                                                                                                                                                                                           |                                                                                                                                                                               |
| <span data-ttu-id="4f8a9-119">scopes</span><span class="sxs-lookup"><span data-stu-id="4f8a9-119">scopes</span></span>       | <span data-ttu-id="4f8a9-120">用户必须同意登录的范围的逗号分隔字符串。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-120">Comma-separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="4f8a9-121">推荐。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-121">Recommended.</span></span>                                                                                                                                                                                     |
| <span data-ttu-id="4f8a9-122">authority</span><span class="sxs-lookup"><span data-stu-id="4f8a9-122">authority</span></span>    | <span data-ttu-id="4f8a9-123">颁发机构字符串 - 默认为公共颁发机构。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-123">Authority string - default is the common authority.</span></span> <span data-ttu-id="4f8a9-124">对于单租户应用，请使用租户 ID 或租户名称。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-124">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="4f8a9-125">例如， `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` 或 `https://login.microsoftonline.com/[your-tenant-id]` 。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-125">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="4f8a9-126">可选。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-126">Optional.</span></span> |                                                                                                                                                                                          |
| <span data-ttu-id="4f8a9-127">mainWindow</span><span class="sxs-lookup"><span data-stu-id="4f8a9-127">mainWindow</span></span>  | <span data-ttu-id="4f8a9-128">需要身份验证的主 BrowserWindow 实例。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-128">Instance of the main BrowserWindow that requires authentication.</span></span>|
| <span data-ttu-id="4f8a9-129">cachePlugin</span><span class="sxs-lookup"><span data-stu-id="4f8a9-129">cachePlugin</span></span> | <span data-ttu-id="4f8a9-130">要用于永久存储令牌的缓存插件。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-130">Cache plugin you would like to use for persistent storage of tokens.</span></span> <span data-ttu-id="4f8a9-131">请参阅 [节点的 Microsoft 身份验证扩展](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/extensions/msal-node-extensions)。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-131">See [Microsoft Authentication Extensions for Node](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/extensions/msal-node-extensions).</span></span> <span data-ttu-id="4f8a9-132">可选。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-132">Optional.</span></span> | 

><span data-ttu-id="4f8a9-133">**注意：** 目前，提供程序不支持增量支持。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-133">**Note:** Currently, the provider does not support incremental support.</span></span> <span data-ttu-id="4f8a9-134">作为最佳实践，请务必同意组件需要的所有作用域。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-134">As a best practice, be sure to consent to all the scopes that the components require.</span></span>
    
## <a name="create-an-appclient-id"></a><span data-ttu-id="4f8a9-135">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="4f8a9-135">Create an app/client ID</span></span>

### <a name="add-new-application-registration-in-azure-active-directory-to-get-a-client-id"></a><span data-ttu-id="4f8a9-136">在 Azure Active Directory 中添加新应用程序注册，获取客户端 ID</span><span class="sxs-lookup"><span data-stu-id="4f8a9-136">Add new application registration in Azure Active Directory to get a client ID</span></span>

<span data-ttu-id="4f8a9-137">若要在 Azure Active Directory 中创建应用程序，请添加新的应用程序注册，然后配置应用名称和重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-137">To create an application in Azure Active Directory, add a new application registration, and then configure an app name and redirect URI.</span></span>

<span data-ttu-id="4f8a9-138">若要在 Azure Active Directory 中创建应用，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="4f8a9-138">To create the app in Azure Active Directory:</span></span>

1. <span data-ttu-id="4f8a9-139">转到 [Azure 门户](https://portal.azure.com)。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-139">Go to the [Azure portal](https://portal.azure.com).</span></span>
1. <span data-ttu-id="4f8a9-140">从菜单中，选择 **Azure Active Directory**。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-140">From the menu, select **Azure Active Directory**.</span></span>
1. <span data-ttu-id="4f8a9-141">从 Azure Active Directory 菜单中，选择 **应用注册**。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-141">From the Azure Active Directory menu, select **App registrations**.</span></span>
1. <span data-ttu-id="4f8a9-142">从顶部菜单中，选择 **"新建注册"** 按钮。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-142">From the top menu, select the **New registration** button.</span></span>
1. <span data-ttu-id="4f8a9-143">输入应用的名称;例如 `My Electron-App` ，。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-143">Enter the name for your app; for example, `My Electron-App`.</span></span>
1. <span data-ttu-id="4f8a9-144">对于受支持的帐户类型 [](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)类型，选择任何组织目录中的帐户 (任何 Azure AD 目录 - 多租户) 和个人 Microsoft 帐户 (例如 **Skype、Xbox) 。**</span><span class="sxs-lookup"><span data-stu-id="4f8a9-144">For the type of [supported account types](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app), select **Accounts in any organizational directory (Any Azure AD directory - Multitenant) and personal Microsoft accounts (e.g. Skype, Xbox)**.</span></span>
1. <span data-ttu-id="4f8a9-145">在"重定向 **URI"** 字段中的下拉列表中，选择 **"** 公共客户端/本机 (移动&桌面) ，在 URL 字段中输入 `msal://redirect` 。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-145">In the **Redirect URI** field, in the dropdown, select **Public client/native (mobile & desktop)**, and in the URL field, enter `msal://redirect`.</span></span>
1. <span data-ttu-id="4f8a9-146">通过选择"注册"按钮 **确认** 更改。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-146">Confirm changes by selecting the **Register** button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4f8a9-147">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4f8a9-147">Next steps</span></span>

* <span data-ttu-id="4f8a9-148">查看生成电子应用 [分步教程](../get-started/build-an-electron-app.md)。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-148">Check out the step-by-step tutorial for [building an electron app](../get-started/build-an-electron-app.md).</span></span>
* <span data-ttu-id="4f8a9-149">请看一下显示如何使用"一体器"提供程序的示例 ["一](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/samples/electron-app) 体"。</span><span class="sxs-lookup"><span data-stu-id="4f8a9-149">Take a look at a [sample Electron application](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/samples/electron-app) that shows how to use the Electron provider.</span></span>
