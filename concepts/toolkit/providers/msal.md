---
title: MSAL 提供程序
description: MSAL 提供程序使用 MSAL 来登录用户并获取令牌以用于 Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: aa3eecb6bd9f2adae7ff689f30ab69539e1d27f1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955776"
---
# <a name="msal-provider"></a><span data-ttu-id="9fef1-103">MSAL 提供程序</span><span class="sxs-lookup"><span data-stu-id="9fef1-103">MSAL provider</span></span>

<span data-ttu-id="9fef1-104">MSAL 提供程序使用[MSAL](https://github.com/AzureAD/microsoft-authentication-library-for-js)来登录用户并获取令牌以用于 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="9fef1-104">The MSAL Provider uses [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) to sign in users and acquire tokens to use with the Microsoft Graph.</span></span>

<span data-ttu-id="9fef1-105">若要了解详细信息，请参阅[提供程序](../providers.md)。</span><span class="sxs-lookup"><span data-stu-id="9fef1-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="9fef1-106">入门</span><span class="sxs-lookup"><span data-stu-id="9fef1-106">Get started</span></span>

<span data-ttu-id="9fef1-107">您可以初始化 HTML 或 JavaScript 中的 MSAL 提供程序。</span><span class="sxs-lookup"><span data-stu-id="9fef1-107">You can initialize the MSAL provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="9fef1-108">在 HTML 页面中初始化</span><span class="sxs-lookup"><span data-stu-id="9fef1-108">Initialize in your HTML page</span></span>

<span data-ttu-id="9fef1-109">若要在 HTML 中初始化 MSAL 提供程序，最简单的方法是创建新的提供程序。</span><span class="sxs-lookup"><span data-stu-id="9fef1-109">Initializing the MSAL provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="9fef1-110">使用`mgt-msal-provider`组件设置**客户端 id**和其他属性。</span><span class="sxs-lookup"><span data-stu-id="9fef1-110">Use the `mgt-msal-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="9fef1-111">这将创建一个将`UserAgentApplication`用于所有身份验证和获取令牌的新实例。</span><span class="sxs-lookup"><span data-stu-id="9fef1-111">This will create a new `UserAgentApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   authority=""></mgt-msal-provider>
```

| <span data-ttu-id="9fef1-112">属性</span><span class="sxs-lookup"><span data-stu-id="9fef1-112">Attribute</span></span> | <span data-ttu-id="9fef1-113">说明</span><span class="sxs-lookup"><span data-stu-id="9fef1-113">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="9fef1-114">客户端 id</span><span class="sxs-lookup"><span data-stu-id="9fef1-114">client-id</span></span>   | <span data-ttu-id="9fef1-115">字符串客户端 ID （请参阅创建应用/客户端 ID）。</span><span class="sxs-lookup"><span data-stu-id="9fef1-115">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="9fef1-116">必需。</span><span class="sxs-lookup"><span data-stu-id="9fef1-116">Required.</span></span>|
| <span data-ttu-id="9fef1-117">登录类型</span><span class="sxs-lookup"><span data-stu-id="9fef1-117">login-type</span></span>  | <span data-ttu-id="9fef1-118">和`redirect` `popup` -默认值之间的枚举`redirect`为。</span><span class="sxs-lookup"><span data-stu-id="9fef1-118">Enumeration between `redirect` and `popup` - default value is `redirect`.</span></span> <span data-ttu-id="9fef1-119">可选。</span><span class="sxs-lookup"><span data-stu-id="9fef1-119">Optional.</span></span> |
| <span data-ttu-id="9fef1-120">scopes</span><span class="sxs-lookup"><span data-stu-id="9fef1-120">scopes</span></span>  | <span data-ttu-id="9fef1-121">用户必须同意登录时的作用域的逗号分隔字符串。</span><span class="sxs-lookup"><span data-stu-id="9fef1-121">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="9fef1-122">可选。</span><span class="sxs-lookup"><span data-stu-id="9fef1-122">Optional.</span></span>|
| <span data-ttu-id="9fef1-123">监管</span><span class="sxs-lookup"><span data-stu-id="9fef1-123">authority</span></span>  | <span data-ttu-id="9fef1-124">颁发机构字符串-默认为常用证书颁发机构。</span><span class="sxs-lookup"><span data-stu-id="9fef1-124">Authority string - default is the common authority.</span></span> <span data-ttu-id="9fef1-125">可选。</span><span class="sxs-lookup"><span data-stu-id="9fef1-125">Optional.</span></span>|
| <span data-ttu-id="9fef1-126">取决于</span><span class="sxs-lookup"><span data-stu-id="9fef1-126">depends-on</span></span> | <span data-ttu-id="9fef1-127">另一个较高优先级提供程序组件的元素选择器字符串。</span><span class="sxs-lookup"><span data-stu-id="9fef1-127">Element selector string of another higher priority provider component.</span></span> <span data-ttu-id="9fef1-128">可选。</span><span class="sxs-lookup"><span data-stu-id="9fef1-128">Optional.</span></span> |

### <a name="initialize-in-javascript"></a><span data-ttu-id="9fef1-129">在 JavaScript 中初始化</span><span class="sxs-lookup"><span data-stu-id="9fef1-129">Initialize in JavaScript</span></span>

<span data-ttu-id="9fef1-130">您可以通过在 JavaScript 中初始化提供程序来提供更多选项。</span><span class="sxs-lookup"><span data-stu-id="9fef1-130">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

<span data-ttu-id="9fef1-131">其中 MsalConfig 是：</span><span class="sxs-lookup"><span data-stu-id="9fef1-131">where MsalConfig is:</span></span>

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  loginType?: LoginType;
  options?: Configuration; // msal js Configuration object
}
```

<span data-ttu-id="9fef1-132">您必须提供`clientId` （以创建新`UserAgentApplication`的）。</span><span class="sxs-lookup"><span data-stu-id="9fef1-132">You must provide a `clientId` (to create a new `UserAgentApplication`).</span></span>

<span data-ttu-id="9fef1-133">若要了解详细信息，请参阅[MSAL 文档](https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics)。</span><span class="sxs-lookup"><span data-stu-id="9fef1-133">To learn more, see the [MSAL documentation](https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics).</span></span>

## <a name="creating-an-appclient-id"></a><span data-ttu-id="9fef1-134">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="9fef1-134">Creating an app/client ID</span></span>

<span data-ttu-id="9fef1-135">有关如何注册应用并获取客户端 ID 的详细信息，请参阅[注册应用程序快速入门](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app)。</span><span class="sxs-lookup"><span data-stu-id="9fef1-135">For details about how to register an app and get a client ID, see [Register an app quick start](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app).</span></span>

><span data-ttu-id="9fef1-136">**注意：** MSAL 仅支持 OAuth 的隐式流。</span><span class="sxs-lookup"><span data-stu-id="9fef1-136">**Note:** MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="9fef1-137">请确保在 Azure 门户中的应用程序中启用隐式流（默认情况下不启用）。</span><span class="sxs-lookup"><span data-stu-id="9fef1-137">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="9fef1-138">在 "**身份验证**" 下，找到 "**隐式授予**" 部分，然后选择 "**访问令牌**" 和**ID 令牌**的复选框。</span><span class="sxs-lookup"><span data-stu-id="9fef1-138">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span>
