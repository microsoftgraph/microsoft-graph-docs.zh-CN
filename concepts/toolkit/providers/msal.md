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
# <a name="msal-provider"></a><span data-ttu-id="08926-103">MSAL 提供程序</span><span class="sxs-lookup"><span data-stu-id="08926-103">MSAL provider</span></span>

<span data-ttu-id="08926-104">MSAL 提供程序使用[MSAL](https://github.com/AzureAD/microsoft-authentication-library-for-js)来登录用户并获取令牌以用于 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="08926-104">The MSAL Provider uses [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) to sign in users and acquire tokens to use with the Microsoft Graph.</span></span>

<span data-ttu-id="08926-105">若要了解详细信息, 请参阅[提供程序](../providers.md)。</span><span class="sxs-lookup"><span data-stu-id="08926-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="08926-106">入门</span><span class="sxs-lookup"><span data-stu-id="08926-106">Get started</span></span>

<span data-ttu-id="08926-107">您可以初始化 HTML 或 JavaScript 中的 MSAL 提供程序。</span><span class="sxs-lookup"><span data-stu-id="08926-107">You can initialize the MSAL provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="08926-108">在 HTML 页面中初始化</span><span class="sxs-lookup"><span data-stu-id="08926-108">Initialize in your HTML page</span></span>

<span data-ttu-id="08926-109">若要在 HTML 中初始化 MSAL 提供程序, 最简单的方法是创建新的提供程序。</span><span class="sxs-lookup"><span data-stu-id="08926-109">Initializing the MSAL provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="08926-110">使用`mgt-msal-provider`组件设置**客户端 id**和其他属性。</span><span class="sxs-lookup"><span data-stu-id="08926-110">Use the `mgt-msal-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="08926-111">这将创建一个将`UserAgentApplication`用于所有身份验证和获取令牌的新实例。</span><span class="sxs-lookup"><span data-stu-id="08926-111">This will create a new `UserAgentApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   authority=""></mgt-msal-provider>
```

><span data-ttu-id="08926-112">**注意:**`login-type`和`authority`是可选的。</span><span class="sxs-lookup"><span data-stu-id="08926-112">**Note:** `login-type` and `authority` are optional.</span></span>

### <a name="initialize-in-javascript"></a><span data-ttu-id="08926-113">在 JavaScript 中初始化</span><span class="sxs-lookup"><span data-stu-id="08926-113">Initialize in JavaScript</span></span>

<span data-ttu-id="08926-114">您可以通过在 JavaScript 中初始化提供程序来提供更多选项。</span><span class="sxs-lookup"><span data-stu-id="08926-114">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

<span data-ttu-id="08926-115">其中 MsalConfig 是:</span><span class="sxs-lookup"><span data-stu-id="08926-115">where MsalConfig is:</span></span>

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  loginType?: LoginType;
  options?: Configuration; // msal js Configuration object
}
```

<span data-ttu-id="08926-116">您必须提供`clientId` (以创建新`UserAgentApplication`的)。</span><span class="sxs-lookup"><span data-stu-id="08926-116">You must provide a `clientId` (to create a new `UserAgentApplication`).</span></span>

<span data-ttu-id="08926-117">若要了解详细信息, 请参阅[MSAL 文档](https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics)。</span><span class="sxs-lookup"><span data-stu-id="08926-117">To learn more, see the [MSAL documentation](https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics).</span></span>

## <a name="creating-an-appclient-id"></a><span data-ttu-id="08926-118">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="08926-118">Creating an app/client ID</span></span>

<span data-ttu-id="08926-119">有关如何注册应用并获取客户端 ID 的详细信息, 请参阅[注册应用程序快速入门](https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-register-app)。</span><span class="sxs-lookup"><span data-stu-id="08926-119">For details about how to register an app and get a client ID, see the [Register an app quick start](https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-register-app).</span></span>

><span data-ttu-id="08926-120">**注意:** MSAL 仅支持 OAuth 的隐式流。</span><span class="sxs-lookup"><span data-stu-id="08926-120">**Note:** MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="08926-121">请确保在 Azure 门户中的应用程序中启用隐式流 (默认情况下不启用)。</span><span class="sxs-lookup"><span data-stu-id="08926-121">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="08926-122">在 "**身份验证**" 下, 找到 "**隐式授予**" 部分, 然后选择 "**访问令牌**" 和**ID 令牌**的复选框。</span><span class="sxs-lookup"><span data-stu-id="08926-122">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span>
