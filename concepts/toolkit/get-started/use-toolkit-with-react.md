---
title: 将 Microsoft Graph 工具包与响应结合使用
description: 在响应应用程序中开始使用 Microsoft Graph 工具包。
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 8f570caf2be4c123bd9a9a93e45a5508029efdee
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967757"
---
# <a name="use-the-microsoft-graph-toolkit-with-react"></a><span data-ttu-id="13724-103">将 Microsoft Graph 工具包与响应结合使用</span><span class="sxs-lookup"><span data-stu-id="13724-103">Use the Microsoft Graph Toolkit with React</span></span>

<span data-ttu-id="13724-104">Microsoft Graph 工具包是一组 web 组件，可简化与 Microsoft Graph 的连接，并使您可以将精力集中在您的应用程序上。</span><span class="sxs-lookup"><span data-stu-id="13724-104">Microsoft Graph Toolkit is a set of web components that simplify connecting to Microsoft Graph and allow you to focus on your application instead.</span></span> <span data-ttu-id="13724-105">Microsoft Graph 工具包可用作通过 **@microsoft/mgt** npm 程序包分发的一组通用 web 组件。</span><span class="sxs-lookup"><span data-stu-id="13724-105">Microsoft Graph Toolkit is available as a generic set of web components distributed through the **@microsoft/mgt** npm package.</span></span>

<span data-ttu-id="13724-106">如果您正在构建具有反应的应用程序，则可以使用 **@microsoft/mgt-react** 包，它会在响应组件中包装 Microsoft Graph 工具包 web 组件，从而更轻松地传递复杂数据。</span><span class="sxs-lookup"><span data-stu-id="13724-106">If you're building apps with React, you can use the **@microsoft/mgt-react** package, which wraps Microsoft Graph Toolkit web components in React components and makes it easier to pass complex data.</span></span>

<span data-ttu-id="13724-107">本文介绍了使用 Microsoft Graph 工具包创建响应应用程序并将其连接到 Microsoft 365 的分步过程。</span><span class="sxs-lookup"><span data-stu-id="13724-107">This article describes the step-by-step process of using the Microsoft Graph Toolkit to create a React app and connect it to Microsoft 365.</span></span> <span data-ttu-id="13724-108">完成这些步骤后，你将看到一个响应应用，显示 Microsoft 365 中当前登录用户的即将到来的约会。</span><span class="sxs-lookup"><span data-stu-id="13724-108">After completing the steps, you'll have a React app that shows the upcoming appointments of the currently signed in user from Microsoft 365.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13724-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="13724-109">Prerequisites</span></span>

<span data-ttu-id="13724-110">若要按照本文中的步骤操作，你将需要 Microsoft 365 开发环境和一些工具。</span><span class="sxs-lookup"><span data-stu-id="13724-110">To follow the steps in this article, you'll need a Microsoft 365 development environment and a few tools.</span></span> <span data-ttu-id="13724-111">有关详细信息， [请参阅入门](./overview.md)。</span><span class="sxs-lookup"><span data-stu-id="13724-111">For details, see [getting started](./overview.md).</span></span>

## <a name="create-a-react-app"></a><span data-ttu-id="13724-112">创建响应应用程序</span><span class="sxs-lookup"><span data-stu-id="13724-112">Create a React app</span></span>

<span data-ttu-id="13724-113">通过运行以下命令创建新的响应应用程序。</span><span class="sxs-lookup"><span data-stu-id="13724-113">Create a new React app by running the following command.</span></span> <span data-ttu-id="13724-114">这将使用 TypeScript 创建新的响应应用程序，这将帮助您编写更可靠的代码并避免运行时错误。</span><span class="sxs-lookup"><span data-stu-id="13724-114">This will create a new React app using TypeScript, which will help you write more robust code and avoid runtime errors.</span></span>

```cmd
npx create-react-app my-m365-app --template typescript
```

<span data-ttu-id="13724-115">将工作目录更改为新创建的应用程序。</span><span class="sxs-lookup"><span data-stu-id="13724-115">Change the working directory to the newly created app.</span></span>

```cmd
cd my-m365-app
```

<span data-ttu-id="13724-116">接下来，安装包含 Microsoft Graph 工具包响应组件 **的 npm 包** 。</span><span class="sxs-lookup"><span data-stu-id="13724-116">Next, install the **mgt-react** npm package, which contains the Microsoft Graph Toolkit React components.</span></span>

```cmd
npm i @microsoft/mgt-react
```

<span data-ttu-id="13724-117">确认您可以运行应用程序。</span><span class="sxs-lookup"><span data-stu-id="13724-117">Confirm that you can run the app.</span></span>

```cmd
HTTPS=true npm start
```

> [!IMPORTANT]
> <span data-ttu-id="13724-118">您的应用程序需要在 HTTPS 上运行，以便能够针对 Microsoft 365 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="13724-118">Your app need to run on HTTPS in order to be able to authenticate against Microsoft 365.</span></span> <span data-ttu-id="13724-119">对于本地测试，使用响应脚本，可以通过将环境变量设置为来将本地 web 服务器配置为在 HTTPS 上运行 `HTTPS` `true` 。</span><span class="sxs-lookup"><span data-stu-id="13724-119">For local testing, with the React scripts, you can configure the local web server to run on HTTPS by setting the `HTTPS` environment variable to `true`.</span></span> <span data-ttu-id="13724-120">您可以每次执行此操作，为 `npm start` 命令加上前缀 `HTTPS=true` (仅在 bash) 或通过在您的计算机上全局设置环境变量。</span><span class="sxs-lookup"><span data-stu-id="13724-120">You can do this either each time, by prefixing the `npm start` command with `HTTPS=true` (works only in bash) or by setting the environment variable globally on your computer.</span></span>

<span data-ttu-id="13724-121">您应该能够通过在浏览器中打开您的应用程序 `https://localhost:3000` 。</span><span class="sxs-lookup"><span data-stu-id="13724-121">You should be able to open your app in the browser via `https://localhost:3000`.</span></span>

[!INCLUDE [AAD with implicit flow app registration](../includes/aad-app-registration-spa.md)]

## <a name="connect-react-app-to-microsoft-365"></a><span data-ttu-id="13724-122">将响应应用连接到 Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="13724-122">Connect React app to Microsoft 365</span></span>

<span data-ttu-id="13724-123">现在，您已将应用程序注册到 Azure Active Directory (Azure AD) ，可以将响应应用程序连接到 Microsoft 365。</span><span class="sxs-lookup"><span data-stu-id="13724-123">Now that you have registered your application with Azure Active Directory (Azure AD), you can connect the React app to Microsoft 365.</span></span> <span data-ttu-id="13724-124">首先，允许用户使用其 Microsoft 帐户登录应用。</span><span class="sxs-lookup"><span data-stu-id="13724-124">First, allow users to sign in to the app using their Microsoft account.</span></span>

### <a name="copy-the-azure-ad-application-registration-id"></a><span data-ttu-id="13724-125">复制 Azure AD 应用程序注册 ID</span><span class="sxs-lookup"><span data-stu-id="13724-125">Copy the Azure AD application registration ID</span></span>

1. <span data-ttu-id="13724-126">在 Azure 门户中，转到应用程序注册。</span><span class="sxs-lookup"><span data-stu-id="13724-126">In the Azure Portal, go to your application registration.</span></span>
1. <span data-ttu-id="13724-127">验证您是否在 " **概述** " 页上。</span><span class="sxs-lookup"><span data-stu-id="13724-127">Verify that you are on the **Overview** page.</span></span>
1. <span data-ttu-id="13724-128">从 " **Essentials** " 部分，将应用程序的值复制 **(客户端) ID** 属性</span><span class="sxs-lookup"><span data-stu-id="13724-128">From the **Essentials** section, copy the value of the **Application (client) ID** property</span></span>

### <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a><span data-ttu-id="13724-129">配置 Microsoft Graph 工具包身份验证提供程序</span><span class="sxs-lookup"><span data-stu-id="13724-129">Configure the Microsoft Graph Toolkit authentication provider</span></span>

<span data-ttu-id="13724-130">接下来，配置 Microsoft Graph 工具包应使用的身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="13724-130">Next, configure the authentication provider that the Microsoft Graph Toolkit should use.</span></span> <span data-ttu-id="13724-131">在这种情况下，您将使用 MSAL，这是构建独立应用程序的一个很棒的默认值。</span><span class="sxs-lookup"><span data-stu-id="13724-131">In this case, you'll use MSAL, which is a good default for building standalone applications.</span></span> <span data-ttu-id="13724-132">如果使用 Microsoft 365 中的任一扩展点（如团队或 SharePoint），则将使用 [其他提供程序](../providers.md)。</span><span class="sxs-lookup"><span data-stu-id="13724-132">If you use any of the extensibility points in Microsoft 365, like Teams or SharePoint, you will use [other providers](../providers.md).</span></span>

1. <span data-ttu-id="13724-133">在代码编辑器中，打开 " **src/索引"。**</span><span class="sxs-lookup"><span data-stu-id="13724-133">In the code editor, open the **src/index.**</span></span> <span data-ttu-id="13724-134">文件，并添加到导入列表中，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="13724-134">file, and to the list of imports, add:</span></span>

    ```tsx
    import { MsalProvider, Providers } from '@microsoft/mgt';
    ```

1. <span data-ttu-id="13724-135">在最后一个 `import` 语句后，使用 MSAL provider 初始化 Microsoft Graph 工具包。</span><span class="sxs-lookup"><span data-stu-id="13724-135">After the last `import` statement, initialize the Microsoft Graph Toolkit with MSAL provider.</span></span>

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'REPLACE_WITH_CLIENTID'
    });
    ```

    <span data-ttu-id="13724-136">将属性的值替换 `clientId` 为 `Application (client) ID` 先前在 Azure 门户中复制的属性的值。</span><span class="sxs-lookup"><span data-stu-id="13724-136">Replace the value of the `clientId` property with the value of the `Application (client) ID` property you copied previously in the Azure Portal.</span></span>

<span data-ttu-id="13724-137">进行这些更改后， **src/index 的 tsx** 文件将如下所示。</span><span class="sxs-lookup"><span data-stu-id="13724-137">With these changes, the **src/index.tsx** file will look like the following.</span></span>

  ```tsx
  import { MsalProvider, Providers } from '@microsoft/mgt';
  import React from 'react';
  import ReactDOM from 'react-dom';
  import App from './App';
  import './index.css';
  import * as serviceWorker from './serviceWorker';
  
  Providers.globalProvider = new MsalProvider({
    clientId: 'REPLACE_WITH_CLIENTID'
  });
  
  ReactDOM.render(
    <React.StrictMode>
      <App />
    </React.StrictMode>,
    document.getElementById('root')
  );
  
  // If you want your app to work offline and load faster, you can change
  // unregister() to register() below. Note this comes with some pitfalls.
  // Learn more about service workers: https://bit.ly/CRA-PWA
  serviceWorker.unregister();
  ```

### <a name="add-the-sign-in-button"></a><span data-ttu-id="13724-138">添加 "登录" 按钮</span><span class="sxs-lookup"><span data-stu-id="13724-138">Add the Sign in button</span></span>

<span data-ttu-id="13724-139">添加 **登录名** Microsoft Graph 工具包响应组件，该组件将显示 " **登录** " 按钮。用户可以使用将其 Microsoft 帐户登录到您的应用程序。</span><span class="sxs-lookup"><span data-stu-id="13724-139">Add the **Login** Microsoft Graph Toolkit React component, which will display the **Sign in** button people can use to sign in with their Microsoft account to your app.</span></span>

1. <span data-ttu-id="13724-140">在代码编辑器中，打开 **src/App/tsx** 文件，并将导入到导入列表：</span><span class="sxs-lookup"><span data-stu-id="13724-140">In the code editor, open the **src/App.tsx** file, and to the list of imports add:</span></span>

    ```tsx
    import { Login } from '@microsoft/mgt-react';
    ```

1. <span data-ttu-id="13724-141">在 `App` 函数中，将子句的内容替换 `return` 为基本结构，包括 Microsoft Graph 工具包登录组件：</span><span class="sxs-lookup"><span data-stu-id="13724-141">In the `App` function, replace the contents of the `return` clause with the basic structure including the Microsoft Graph Toolkit Login component:</span></span>

    ```tsx
    <div className="App">
      <header>
        <Login />
      </header>
    </div>
    ```

<span data-ttu-id="13724-142">在进行这些更改后， **src/App tsx** 文件将如下所示。</span><span class="sxs-lookup"><span data-stu-id="13724-142">With these changes, the **src/App.tsx** file will look like the following.</span></span>
```tsx
import { MsalProvider, Providers } from '@microsoft/mgt';
import { Login } from '@microsoft/mgt-react';
import React from 'react';
import './App.css';

function App() {
  Providers.globalProvider = new MsalProvider({
    clientId: 'REPLACE_WITH_CLIENTID'
  });

  return (
    <div className="App">
      <header>
        <Login />
      </header>
    </div>
  );
}

export default App;
```

### <a name="test-signing-in-to-your-application"></a><span data-ttu-id="13724-143">测试登录到应用程序</span><span class="sxs-lookup"><span data-stu-id="13724-143">Test signing in to your application</span></span>

<span data-ttu-id="13724-144">你现在应该能够使用 Microsoft 帐户登录到应用程序。</span><span class="sxs-lookup"><span data-stu-id="13724-144">You should now be able to sign in to your application with your Microsoft account.</span></span>

1. <span data-ttu-id="13724-145">返回到正在运行响应应用程序的浏览器。</span><span class="sxs-lookup"><span data-stu-id="13724-145">Go back to the browser where your React app is running.</span></span> <span data-ttu-id="13724-146">现在，你应该会看到 **"登录"** 按钮。</span><span class="sxs-lookup"><span data-stu-id="13724-146">You should now see a **Sign in** button.</span></span>
1. <span data-ttu-id="13724-147">当您单击 " **登录** " 按钮时，系统将提示您使用 Microsoft 帐户登录 (您可以使用与您在其中使用) 的 Azure 门户访问过的帐户相同的帐户。</span><span class="sxs-lookup"><span data-stu-id="13724-147">When you click the **Sign in** button, you will be prompted to sign in with your Microsoft account (you can use the same account as the one you accessed the Azure Portal with).</span></span>
1. <span data-ttu-id="13724-148">由于这是你第一次使用此 Azure AD 应用程序，因此你需要同意它在你的组织中的使用。</span><span class="sxs-lookup"><span data-stu-id="13724-148">Because this is the first time you're using this Azure AD application, you need to consent its use in your organization.</span></span>
1. <span data-ttu-id="13724-149">登录后，你将被重定向到你的响应应用。</span><span class="sxs-lookup"><span data-stu-id="13724-149">After signing in, you will be redirected to your React app.</span></span> <span data-ttu-id="13724-150">请注意，" **登录** " 按钮更改为显示您的用户的名称 ![ 响应显示使用 microsoft Graph 工具包从 Microsoft 365 检索的用户信息的应用程序 ](../images/mgt-react-userinfo.png) 。</span><span class="sxs-lookup"><span data-stu-id="13724-150">Notice that the **Sign in** button changed to show your user's name ![React app showing user info retrieved from Microsoft 365 using Microsoft Graph Toolkit](../images/mgt-react-userinfo.png).</span></span>

## <a name="load-data-from-microsoft-365"></a><span data-ttu-id="13724-151">从 Microsoft 365 加载数据</span><span class="sxs-lookup"><span data-stu-id="13724-151">Load data from Microsoft 365</span></span>

<span data-ttu-id="13724-152">Microsoft Graph 工具包不仅简化了对 Microsoft 365 的身份验证，还简化了其数据的下载。</span><span class="sxs-lookup"><span data-stu-id="13724-152">Microsoft Graph Toolkit not only simplifies authentication to Microsoft 365, but also loading its data.</span></span> <span data-ttu-id="13724-153">在此示例中，您将显示 "已登录人员的日历"。</span><span class="sxs-lookup"><span data-stu-id="13724-153">In this example, you'll show the signed in person's calendar.</span></span>

### <a name="specify-permissions-needed-for-your-application"></a><span data-ttu-id="13724-154">指定应用程序所需的权限</span><span class="sxs-lookup"><span data-stu-id="13724-154">Specify permissions needed for your application</span></span>

<span data-ttu-id="13724-155">在可以从 Microsoft 365 加载数据之前，您需要指定您的应用程序访问用户数据必须授予的权限范围列表。</span><span class="sxs-lookup"><span data-stu-id="13724-155">Before you can load data from Microsoft 365, you need to specify the list of permission scopes your application must be granted to access user's data.</span></span> <span data-ttu-id="13724-156">这些作用域因要显示的信息类型而异。</span><span class="sxs-lookup"><span data-stu-id="13724-156">These scopes differ depending on what kind of information you want to show.</span></span> <span data-ttu-id="13724-157">在这种情况下，你将需要访问人员的日历，以及对同时显示在日历中的人员的信息的基本访问权限。</span><span class="sxs-lookup"><span data-stu-id="13724-157">In this case, you will need access to people's calendar as well as basic access to information about people that is also displayed in the calendar.</span></span> <span data-ttu-id="13724-158">可以在 [Microsoft GRAPH API 文档](/graph/api/overview?toc=.%2Fref%2Ftoc.json&view=graph-rest-1.0)中查找每个 API 所需的范围。</span><span class="sxs-lookup"><span data-stu-id="13724-158">You can find the scopes required by each API in the [Microsoft Graph API documentation](/graph/api/overview?toc=.%2Fref%2Ftoc.json&view=graph-rest-1.0).</span></span>

1. <span data-ttu-id="13724-159">在代码编辑器中，打开 " **src/索引" tsx** 文件，并更新提供程序初始化代码。</span><span class="sxs-lookup"><span data-stu-id="13724-159">In the code editor, open the **src/index.tsx** file, and update the provider initialization code.</span></span>

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'd7cb93c9-9097-4e38-8f06-7c0088ac3318',
      scopes: ['calendars.read', 'user.read', 'openid', 'profile', 'people.read', 'user.readbasic.all']
    });
    ```

### <a name="show-users-data-after-signing-in"></a><span data-ttu-id="13724-160">登录后显示用户数据</span><span class="sxs-lookup"><span data-stu-id="13724-160">Show user's data after signing in</span></span>

<span data-ttu-id="13724-161">接下来，扩展应用程序以显示用户日历中的数据。</span><span class="sxs-lookup"><span data-stu-id="13724-161">Next, extend the application to show data from the user's calendar.</span></span> <span data-ttu-id="13724-162">只有在用户登录后，才能访问此信息。</span><span class="sxs-lookup"><span data-stu-id="13724-162">You can access this information only after the user has signed in.</span></span> <span data-ttu-id="13724-163">若要执行此操作，您需要跟踪用户的登录状态，并在用户使用其 Microsoft 帐户登录后显示日历数据。</span><span class="sxs-lookup"><span data-stu-id="13724-163">To do this, you will need to track the  user's sign in state and show the calendar data after the user has signed in with their Microsoft account.</span></span>

#### <a name="track-users-sign-in-state"></a><span data-ttu-id="13724-164">跟踪用户的登录状态</span><span class="sxs-lookup"><span data-stu-id="13724-164">Track user's sign in state</span></span>

<span data-ttu-id="13724-165">若要在应用程序中跟踪用户的登录状态，您需要结合使用响应 `useState` 和 `useEffect` 挂接与提供程序事件处理程序。</span><span class="sxs-lookup"><span data-stu-id="13724-165">To track the user's sign in state in your application, you will use the React `useState` and `useEffect` hooks in combination with provider event handlers.</span></span>

1. <span data-ttu-id="13724-166">在代码编辑器中，打开 **src/App. tsx** 文件，并扩展现有的响应 `import` 语句。</span><span class="sxs-lookup"><span data-stu-id="13724-166">In the code editor, open the **src/App.tsx** file and extend the existing React `import` statement.</span></span>

    ```tsx
    import React, { useState, useEffect } from 'react';
    ```

1. <span data-ttu-id="13724-167">`Provider` `ProviderState` 通过添加到导入，从 Microsoft Graph 工具包导入和类型。</span><span class="sxs-lookup"><span data-stu-id="13724-167">Import the `Provider` and `ProviderState` types from Microsoft Graph Toolkit, by adding to imports.</span></span>

    ```tsx
    import { Providers, ProviderState } from '@microsoft/mgt';
    ```

1. <span data-ttu-id="13724-168">添加一个名为的自定义函数 `useIsSignedIn` ，该函数可在应用程序中跟踪用户的登录状态。</span><span class="sxs-lookup"><span data-stu-id="13724-168">Add a custom function named `useIsSignedIn` that enables tracking the user's sign in state in your application.</span></span>

    ```tsx
    function useIsSignedIn(): [boolean] {
      const [isSignedIn, setIsSignedIn] = useState(false);
    
      useEffect(() => {
        const updateState = () => {
          const provider = Providers.globalProvider;
          setIsSignedIn(provider && provider.state === ProviderState.SignedIn);
        };
    
        Providers.onProviderUpdated(updateState);
        updateState();
    
        return () => {
          Providers.removeProviderUpdatedListener(updateState);
        }
      }, []);
    
      return [isSignedIn];
    }
    ```

<span data-ttu-id="13724-169">此函数执行两项操作。</span><span class="sxs-lookup"><span data-stu-id="13724-169">This function does two things.</span></span> <span data-ttu-id="13724-170">首先，使用响应 `useState` 挂钩，启用组件内的跟踪状态。</span><span class="sxs-lookup"><span data-stu-id="13724-170">First, using the React `useState` hook, it enables tracking state inside your component.</span></span> <span data-ttu-id="13724-171">每当状态更改时，响应将重新呈现你的组件。</span><span class="sxs-lookup"><span data-stu-id="13724-171">Whenever the state changes, React will re-render your component.</span></span> <span data-ttu-id="13724-172">其次，通过响应 `useEffect` 挂钩，它通过跟踪 Microsoft Graph 工具包提供程序中的更改并更新组件（如有必要）来扩展组件的生命周期。</span><span class="sxs-lookup"><span data-stu-id="13724-172">Second, using the React `useEffect` hook, it extends the component's lifecycle by tracking changes in the Microsoft Graph Toolkit provider and updating the component if necessary.</span></span>

#### <a name="load-users-calendar-if-user-is-signed-in"></a><span data-ttu-id="13724-173">如果用户已登录，则加载用户的日历</span><span class="sxs-lookup"><span data-stu-id="13724-173">Load user's calendar if user is signed in</span></span>

<span data-ttu-id="13724-174">现在，您在应用程序中跟踪用户的登录状态，您可以在登录后显示其日历。</span><span class="sxs-lookup"><span data-stu-id="13724-174">Now that you track the user's sign in state in your application, you can show their calendar after they signed in.</span></span>

1. <span data-ttu-id="13724-175">在代码编辑器中，打开 **src/app.config** 文件，并在 **应用程序** 函数中添加：</span><span class="sxs-lookup"><span data-stu-id="13724-175">In the code editor, open the **src/App.tsx** file, and inside the **App** function, add:</span></span>

    ```tsx
    const [isSignedIn] = useIsSignedIn();
    ```

    <span data-ttu-id="13724-176">这将定义一个布尔 `isSignedIn` 常量，可使用该常量来确定用户当前是否登录到您的应用程序。</span><span class="sxs-lookup"><span data-stu-id="13724-176">This defines a Boolean `isSignedIn` constant, which you can use to determine whether the user is currently signed in to your application.</span></span>

1. <span data-ttu-id="13724-177">`return`使用附加 `div` 的和 Microsoft Graph 工具包的 "议程" 组件扩展子句的内容。</span><span class="sxs-lookup"><span data-stu-id="13724-177">Extend the contents of the `return` clause with an additional `div` and the Microsoft Graph Toolkit Agenda component.</span></span>

    ```tsx
    <div>
      {isSignedIn &&
        <Agenda />}
    </div>
    ```

<span data-ttu-id="13724-178">使用这些更改时， **src/App tsx** 文件应如下所示：</span><span class="sxs-lookup"><span data-stu-id="13724-178">With these changes, the **src/App.tsx** file should look like the following.</span></span>

```tsx
import { Providers, ProviderState } from '@microsoft/mgt';
import { Agenda, Login } from '@microsoft/mgt-react';
import React, { useState, useEffect } from 'react';
import './App.css';

function useIsSignedIn(): [boolean] {
  const [isSignedIn, setIsSignedIn] = useState(false);

  useEffect(() => {
    const updateState = () => {
      const provider = Providers.globalProvider;
      setIsSignedIn(provider && provider.state === ProviderState.SignedIn);
    };

    Providers.onProviderUpdated(updateState);
    updateState();

    return () => {
      Providers.removeProviderUpdatedListener(updateState);
    }
  }, []);

  return [isSignedIn];
}

function App() {
  const [isSignedIn] = useIsSignedIn();

  return (
    <div className="App">
      <header>
        <Login />
      </header>
      <div>
        {isSignedIn &&
          <Agenda />}
      </div>
    </div>
  );
}

export default App;
```

### <a name="test-showing-users-calendar-after-they-signed-in"></a><span data-ttu-id="13724-179">在用户登录后显示用户日历的测试</span><span class="sxs-lookup"><span data-stu-id="13724-179">Test showing user's calendar after they signed in</span></span>

<span data-ttu-id="13724-180">使用这些更改，在使用 Microsoft 帐户登录应用程序后，您应该会看到您的日历。</span><span class="sxs-lookup"><span data-stu-id="13724-180">With these changes, after signing in to your application with your Microsoft account, you should see your calendar.</span></span>

1. <span data-ttu-id="13724-181">若要查看所做的更改，请关闭浏览器并重新打开它，然后转到 `https://localhost:3000` 。</span><span class="sxs-lookup"><span data-stu-id="13724-181">To see the changes, close the browser and open it again, and go to `https://localhost:3000`.</span></span> <span data-ttu-id="13724-182">执行此操作的原因是您更改了属性的值 `scopes` ，这将影响您从 AZURE AD 请求的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="13724-182">You do this because you changed the value of the `scopes` property, which affects the access token that you request from Azure AD.</span></span>
1. <span data-ttu-id="13724-183">选择 " **登录** " 按钮，并使用你的 Microsoft 帐户登录。</span><span class="sxs-lookup"><span data-stu-id="13724-183">Choose the **Sign In** button and sign in using your Microsoft account.</span></span> <span data-ttu-id="13724-184">请注意，在同意提示中所请求的权限列表中添加的内容。</span><span class="sxs-lookup"><span data-stu-id="13724-184">Notice the additions to the list of permissions requested in the consent prompt.</span></span> <span data-ttu-id="13724-185">这是因为您在该属性中包含了其他权限 `scope` 。</span><span class="sxs-lookup"><span data-stu-id="13724-185">This is because you included additional permissions in the `scope` property.</span></span>
1. <span data-ttu-id="13724-186">在同意使用应用程序后，您应看到有关当前用户及其日历的信息。</span><span class="sxs-lookup"><span data-stu-id="13724-186">After consenting to the use of the application, you should see information about the current user and their calendar.</span></span>

![已完成应用](../images/mgt-finished-app.png)

## <a name="next-steps"></a><span data-ttu-id="13724-188">后续步骤</span><span class="sxs-lookup"><span data-stu-id="13724-188">Next steps</span></span>

- <span data-ttu-id="13724-189">请参阅 [Microsoft Graph 工具包中的内容](../overview.md)。</span><span class="sxs-lookup"><span data-stu-id="13724-189">See [what's in the Microsoft Graph Toolkit](../overview.md).</span></span>
- <span data-ttu-id="13724-190">尝试 [样本](https://mgt.dev)中的组件。</span><span class="sxs-lookup"><span data-stu-id="13724-190">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="13724-191">在 [堆栈溢出](https://aka.ms/mgt-question)时提出问题。</span><span class="sxs-lookup"><span data-stu-id="13724-191">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="13724-192">在 [GitHub](https://aka.ms/mgt)上报告错误或保留功能请求。</span><span class="sxs-lookup"><span data-stu-id="13724-192">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
