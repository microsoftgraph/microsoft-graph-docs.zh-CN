---
title: 将 Microsoft Graph Toolkit React
description: 在 React 应用程序中开始使用 Microsoft Graph Toolkit。
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 57e9901c8b7ee1f8a5474f21ff4b09def053e7db
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664133"
---
# <a name="use-the-microsoft-graph-toolkit-with-react"></a><span data-ttu-id="28f46-103">将 Microsoft Graph Toolkit React</span><span class="sxs-lookup"><span data-stu-id="28f46-103">Use the Microsoft Graph Toolkit with React</span></span>

<span data-ttu-id="28f46-104">Microsoft Graph Toolkit是一组 Web 组件，可简化连接到 Microsoft Graph，并允许您专注于应用程序。</span><span class="sxs-lookup"><span data-stu-id="28f46-104">Microsoft Graph Toolkit is a set of web components that simplify connecting to Microsoft Graph and allow you to focus on your application instead.</span></span> <span data-ttu-id="28f46-105">Microsoft Graph Toolkit作为通过 npm 包分发的通用 `@microsoft/mgt` Web 组件集提供。</span><span class="sxs-lookup"><span data-stu-id="28f46-105">Microsoft Graph Toolkit is available as a generic set of web components distributed through the `@microsoft/mgt` npm package.</span></span>

<span data-ttu-id="28f46-106">如果你使用 React 生成应用，可以使用程序包，该程序包[ `@microsoft/mgt-react` ](./mgt-react.md)将 Microsoft Graph Toolkit Web 组件包装在 React 组件中，并更轻松地传递复杂数据。</span><span class="sxs-lookup"><span data-stu-id="28f46-106">If you're building apps with React, you can use the [`@microsoft/mgt-react` package](./mgt-react.md), which wraps Microsoft Graph Toolkit web components in React components and makes it easier to pass complex data.</span></span>

<span data-ttu-id="28f46-107">本文介绍了使用 Microsoft Graph Toolkit创建 React 应用并连接到 Microsoft 365 的分步过程。</span><span class="sxs-lookup"><span data-stu-id="28f46-107">This article describes the step-by-step process of using the Microsoft Graph Toolkit to create a React app and connect it to Microsoft 365.</span></span> <span data-ttu-id="28f46-108">完成这些步骤后，你将拥有一个 React 应用，该应用显示 Microsoft 365 中当前已登录用户的即将进行的约会。</span><span class="sxs-lookup"><span data-stu-id="28f46-108">After completing the steps, you'll have a React app that shows the upcoming appointments of the currently signed in user from Microsoft 365.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28f46-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="28f46-109">Prerequisites</span></span>

<span data-ttu-id="28f46-110">若要按照本文中的步骤操作，你需要 Microsoft 365 开发环境和一些工具。</span><span class="sxs-lookup"><span data-stu-id="28f46-110">To follow the steps in this article, you'll need a Microsoft 365 development environment and a few tools.</span></span> <span data-ttu-id="28f46-111">有关详细信息，请参阅 [入门](./overview.md)。</span><span class="sxs-lookup"><span data-stu-id="28f46-111">For details, see [getting started](./overview.md).</span></span>

## <a name="create-a-react-app"></a><span data-ttu-id="28f46-112">创建 React 应用</span><span class="sxs-lookup"><span data-stu-id="28f46-112">Create a React app</span></span>

<span data-ttu-id="28f46-113">通过运行以下命令创建新的 React 应用。</span><span class="sxs-lookup"><span data-stu-id="28f46-113">Create a new React app by running the following command.</span></span> <span data-ttu-id="28f46-114">这将使用 TypeScript 创建新的 React 应用，这将帮助你编写更可靠的代码并避免运行时错误。</span><span class="sxs-lookup"><span data-stu-id="28f46-114">This will create a new React app using TypeScript, which will help you write more robust code and avoid runtime errors.</span></span>

```cmd
npx create-react-app my-m365-app --template typescript
```

<span data-ttu-id="28f46-115">将工作目录更改为新创建的应用。</span><span class="sxs-lookup"><span data-stu-id="28f46-115">Change the working directory to the newly created app.</span></span>

```cmd
cd my-m365-app
```

<span data-ttu-id="28f46-116">接下来，安装 `mgt-react` npm 包，其中包含 Microsoft Graph Toolkit React 组件。</span><span class="sxs-lookup"><span data-stu-id="28f46-116">Next, install the `mgt-react` npm package, which contains the Microsoft Graph Toolkit React components.</span></span>

```cmd
npm i @microsoft/mgt-react
```

<span data-ttu-id="28f46-117">同时安装包含 MSAL 身份验证提供程序的 `mgt-msal-provider` `mgt-element` 和 npm 包。</span><span class="sxs-lookup"><span data-stu-id="28f46-117">Install the `mgt-msal-provider` and `mgt-element` npm package as well, which contains the MSAL auth provider.</span></span>

```cmd
npm i @microsoft/mgt-element @microsoft/mgt-msal-provider
```

<span data-ttu-id="28f46-118">确认你可以运行应用。</span><span class="sxs-lookup"><span data-stu-id="28f46-118">Confirm that you can run the app.</span></span>

```cmd
npm start
```

<span data-ttu-id="28f46-119">你应该能够通过在浏览器中打开你的应用 `http://localhost:3000` 。</span><span class="sxs-lookup"><span data-stu-id="28f46-119">You should be able to open your app in the browser via `http://localhost:3000`.</span></span>

[!INCLUDE [AAD with implicit flow app registration](../includes/aad-app-registration-spa.md)]

## <a name="connect-react-app-to-microsoft-365"></a><span data-ttu-id="28f46-120">将 React 应用连接到 Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="28f46-120">Connect React app to Microsoft 365</span></span>

<span data-ttu-id="28f46-121">现在，你已在 Azure AD (Azure Active Directory) ，可以将 React 应用连接到 Microsoft 365。</span><span class="sxs-lookup"><span data-stu-id="28f46-121">Now that you have registered your application with Azure Active Directory (Azure AD), you can connect the React app to Microsoft 365.</span></span> <span data-ttu-id="28f46-122">首先，允许用户使用其 Microsoft 帐户登录应用。</span><span class="sxs-lookup"><span data-stu-id="28f46-122">First, allow users to sign in to the app using their Microsoft account.</span></span>

### <a name="copy-the-azure-ad-application-registration-id"></a><span data-ttu-id="28f46-123">复制 Azure AD 应用程序注册 ID</span><span class="sxs-lookup"><span data-stu-id="28f46-123">Copy the Azure AD application registration ID</span></span>

1. <span data-ttu-id="28f46-124">在 Azure 门户中，转到应用程序注册。</span><span class="sxs-lookup"><span data-stu-id="28f46-124">In the Azure Portal, go to your application registration.</span></span>
1. <span data-ttu-id="28f46-125">验证是否位于"概述 **"页上** 。</span><span class="sxs-lookup"><span data-stu-id="28f46-125">Verify that you are on the **Overview** page.</span></span>
1. <span data-ttu-id="28f46-126">从 **Essentials** 部分，复制 Application (**客户端) ID** 属性的值</span><span class="sxs-lookup"><span data-stu-id="28f46-126">From the **Essentials** section, copy the value of the **Application (client) ID** property</span></span>

### <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a><span data-ttu-id="28f46-127">配置 Microsoft Graph Toolkit身份验证提供程序</span><span class="sxs-lookup"><span data-stu-id="28f46-127">Configure the Microsoft Graph Toolkit authentication provider</span></span>

<span data-ttu-id="28f46-128">接下来，配置 Microsoft Graph Toolkit使用的身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="28f46-128">Next, configure the authentication provider that the Microsoft Graph Toolkit should use.</span></span> <span data-ttu-id="28f46-129">在这种情况下，你将使用 MSAL，这是生成独立应用程序的良好默认值。</span><span class="sxs-lookup"><span data-stu-id="28f46-129">In this case, you'll use MSAL, which is a good default for building standalone applications.</span></span> <span data-ttu-id="28f46-130">如果你使用 Microsoft 365 中的任意扩展点，如 Teams 或 SharePoint，你将使用 [其他提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="28f46-130">If you use any of the extensibility points in Microsoft 365, like Teams or SharePoint, you will use [other providers](../providers/providers.md).</span></span>

1. <span data-ttu-id="28f46-131">在代码编辑器中，打开 **src/index。**</span><span class="sxs-lookup"><span data-stu-id="28f46-131">In the code editor, open the **src/index.**</span></span> <span data-ttu-id="28f46-132">文件，并添加到导入列表中，添加：</span><span class="sxs-lookup"><span data-stu-id="28f46-132">file, and to the list of imports, add:</span></span>

    ```tsx
    import { Providers } from '@microsoft/mgt-element';
    import { MsalProvider } from '@microsoft/mgt-msal-provider';
    ```

1. <span data-ttu-id="28f46-133">最后一 `import` 个语句之后，使用 MSAL Toolkit初始化 Microsoft Graph 应用程序。</span><span class="sxs-lookup"><span data-stu-id="28f46-133">After the last `import` statement, initialize the Microsoft Graph Toolkit with MSAL provider.</span></span>

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'REPLACE_WITH_CLIENTID'
    });
    ```

    <span data-ttu-id="28f46-134">将属性的值替换为之前在 Azure 门户中 `clientId` `Application (client) ID` 复制的属性的值。</span><span class="sxs-lookup"><span data-stu-id="28f46-134">Replace the value of the `clientId` property with the value of the `Application (client) ID` property you copied previously in the Azure Portal.</span></span>

<span data-ttu-id="28f46-135">通过这些更改 **，src/index.tsx** 文件将如下所示。</span><span class="sxs-lookup"><span data-stu-id="28f46-135">With these changes, the **src/index.tsx** file will look like the following.</span></span>

  ```tsx
  import React from 'react';
  import ReactDOM from 'react-dom';
  import App from './App';
  import './index.css';
  import * as serviceWorker from './serviceWorker';

  import { Providers } from '@microsoft/mgt-element';
  import { MsalProvider } from '@microsoft/mgt-msal-provider';
  
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

### <a name="add-the-sign-in-button"></a><span data-ttu-id="28f46-136">添加"登录"按钮</span><span class="sxs-lookup"><span data-stu-id="28f46-136">Add the Sign in button</span></span>

<span data-ttu-id="28f46-137">添加 **登录** Microsoft Graph Toolkit React 组件，该组件将显示用户可使用其 Microsoft 帐户登录应用的登录按钮。</span><span class="sxs-lookup"><span data-stu-id="28f46-137">Add the **Login** Microsoft Graph Toolkit React component, which will display the **Sign in** button people can use to sign in with their Microsoft account to your app.</span></span>

1. <span data-ttu-id="28f46-138">在代码编辑器中，打开 **src/App.tsx** 文件，并添加到导入列表中：</span><span class="sxs-lookup"><span data-stu-id="28f46-138">In the code editor, open the **src/App.tsx** file, and to the list of imports add:</span></span>

    ```tsx
    import { Login } from '@microsoft/mgt-react';
    ```

1. <span data-ttu-id="28f46-139">在函数中，将子句的内容替换为基本结构， `App` `return` 包括 Microsoft Graph Toolkit登录组件：</span><span class="sxs-lookup"><span data-stu-id="28f46-139">In the `App` function, replace the contents of the `return` clause with the basic structure including the Microsoft Graph Toolkit Login component:</span></span>

    ```tsx
    <div className="App">
      <header>
        <Login />
      </header>
    </div>
    ```

<span data-ttu-id="28f46-140">通过这些更改 **，src/App.tsx** 文件将如下所示。</span><span class="sxs-lookup"><span data-stu-id="28f46-140">With these changes, the **src/App.tsx** file will look like the following.</span></span>
```tsx

import { Login } from '@microsoft/mgt-react';
import React from 'react';
import './App.css';

function App() {
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

### <a name="test-signing-in-to-your-application"></a><span data-ttu-id="28f46-141">测试应用程序登录</span><span class="sxs-lookup"><span data-stu-id="28f46-141">Test signing in to your application</span></span>

<span data-ttu-id="28f46-142">你现在应该能够使用 Microsoft 帐户登录应用程序。</span><span class="sxs-lookup"><span data-stu-id="28f46-142">You should now be able to sign in to your application with your Microsoft account.</span></span>

1. <span data-ttu-id="28f46-143">返回到运行 React 应用的浏览器。</span><span class="sxs-lookup"><span data-stu-id="28f46-143">Go back to the browser where your React app is running.</span></span> <span data-ttu-id="28f46-144">现在应该会看到"登录 **"** 按钮。</span><span class="sxs-lookup"><span data-stu-id="28f46-144">You should now see a **Sign in** button.</span></span>
1. <span data-ttu-id="28f46-145">单击"登录"按钮时，系统将提示你使用 Microsoft 帐户登录 (可以使用与通过) 访问 Azure 门户的帐户相同的帐户。</span><span class="sxs-lookup"><span data-stu-id="28f46-145">When you click the **Sign in** button, you will be prompted to sign in with your Microsoft account (you can use the same account as the one you accessed the Azure Portal with).</span></span>
1. <span data-ttu-id="28f46-146">因为这是你第一次使用此 Azure AD 应用程序，你需要同意在组织中使用它。</span><span class="sxs-lookup"><span data-stu-id="28f46-146">Because this is the first time you're using this Azure AD application, you need to consent its use in your organization.</span></span>
1. <span data-ttu-id="28f46-147">登录后，你将重定向到 React 应用。</span><span class="sxs-lookup"><span data-stu-id="28f46-147">After signing in, you will be redirected to your React app.</span></span> <span data-ttu-id="28f46-148">请注意 **，"登录"** 按钮已更改，显示用户名称 React 应用，该应用显示使用 Microsoft Graph Toolkit ![ 从 Microsoft 365 检索到的用户 ](../images/mgt-react-userinfo.png) Toolkit。</span><span class="sxs-lookup"><span data-stu-id="28f46-148">Notice that the **Sign in** button changed to show your user's name ![React app showing user info retrieved from Microsoft 365 using Microsoft Graph Toolkit](../images/mgt-react-userinfo.png).</span></span>

## <a name="load-data-from-microsoft-365"></a><span data-ttu-id="28f46-149">从 Microsoft 365 加载数据</span><span class="sxs-lookup"><span data-stu-id="28f46-149">Load data from Microsoft 365</span></span>

<span data-ttu-id="28f46-150">Microsoft Graph Toolkit不仅简化了对 Microsoft 365 的身份验证，还加载了数据。</span><span class="sxs-lookup"><span data-stu-id="28f46-150">Microsoft Graph Toolkit not only simplifies authentication to Microsoft 365, but also loading its data.</span></span> <span data-ttu-id="28f46-151">本示例中，将显示登录人的日历。</span><span class="sxs-lookup"><span data-stu-id="28f46-151">In this example, you'll show the signed in person's calendar.</span></span>

### <a name="specify-permissions-needed-for-your-application"></a><span data-ttu-id="28f46-152">指定应用程序所需的权限</span><span class="sxs-lookup"><span data-stu-id="28f46-152">Specify permissions needed for your application</span></span>

<span data-ttu-id="28f46-153">在可以从 Microsoft 365 加载数据之前，需要指定必须授予应用程序的权限范围列表才能访问用户数据。</span><span class="sxs-lookup"><span data-stu-id="28f46-153">Before you can load data from Microsoft 365, you need to specify the list of permission scopes your application must be granted to access user's data.</span></span> <span data-ttu-id="28f46-154">这些范围因要显示的信息类型而不同。</span><span class="sxs-lookup"><span data-stu-id="28f46-154">These scopes differ depending on what kind of information you want to show.</span></span> <span data-ttu-id="28f46-155">在这种情况下，你将需要访问人员日历以及访问日历中也显示的人的信息的基本访问权限。</span><span class="sxs-lookup"><span data-stu-id="28f46-155">In this case, you will need access to people's calendar as well as basic access to information about people that is also displayed in the calendar.</span></span> <span data-ttu-id="28f46-156">可以在 [Microsoft Graph API](/graph/api/overview)文档中找到每个 API 所需的范围。</span><span class="sxs-lookup"><span data-stu-id="28f46-156">You can find the scopes required by each API in the [Microsoft Graph API documentation](/graph/api/overview).</span></span>

1. <span data-ttu-id="28f46-157">在代码编辑器中，打开 **src/index.tsx** 文件，并更新提供程序初始化代码。</span><span class="sxs-lookup"><span data-stu-id="28f46-157">In the code editor, open the **src/index.tsx** file, and update the provider initialization code.</span></span>

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'd7cb93c9-9097-4e38-8f06-7c0088ac3318',
      scopes: ['calendars.read', 'user.read', 'openid', 'profile', 'people.read', 'user.readbasic.all']
    });
    ```

### <a name="show-users-data-after-signing-in"></a><span data-ttu-id="28f46-158">登录后显示用户数据</span><span class="sxs-lookup"><span data-stu-id="28f46-158">Show user's data after signing in</span></span>

<span data-ttu-id="28f46-159">接下来，扩展应用程序以显示用户日历数据。</span><span class="sxs-lookup"><span data-stu-id="28f46-159">Next, extend the application to show data from the user's calendar.</span></span> <span data-ttu-id="28f46-160">只有在用户登录后，才能访问此信息。</span><span class="sxs-lookup"><span data-stu-id="28f46-160">You can access this information only after the user has signed in.</span></span> <span data-ttu-id="28f46-161">为此，你需要跟踪用户的登录状态，在用户使用其 Microsoft 帐户登录后显示日历数据。</span><span class="sxs-lookup"><span data-stu-id="28f46-161">To do this, you will need to track the  user's sign in state and show the calendar data after the user has signed in with their Microsoft account.</span></span>

#### <a name="track-users-sign-in-state"></a><span data-ttu-id="28f46-162">跟踪用户的登录状态</span><span class="sxs-lookup"><span data-stu-id="28f46-162">Track user's sign in state</span></span>

<span data-ttu-id="28f46-163">若要跟踪应用程序中的用户登录状态，你将 React 和挂钩与提供程序 `useState` `useEffect` 事件处理程序结合使用。</span><span class="sxs-lookup"><span data-stu-id="28f46-163">To track the user's sign in state in your application, you will use the React `useState` and `useEffect` hooks in combination with provider event handlers.</span></span>

1. <span data-ttu-id="28f46-164">在代码编辑器中，打开 **src/App.tsx** 文件并扩展现有的 React `import` 语句。</span><span class="sxs-lookup"><span data-stu-id="28f46-164">In the code editor, open the **src/App.tsx** file and extend the existing React `import` statement.</span></span>

    ```tsx
    import React, { useState, useEffect } from 'react';
    ```

1. <span data-ttu-id="28f46-165">通过添加到 `Provider` `ProviderState` 导入 `mgt-element` 来导入和类型。</span><span class="sxs-lookup"><span data-stu-id="28f46-165">Import the `Provider` and `ProviderState` types from `mgt-element`, by adding to imports.</span></span>

    ```tsx
    import { Providers, ProviderState } from '@microsoft/mgt-element';
    ```

1. <span data-ttu-id="28f46-166">添加一个名为的自定义函数，该函数可在应用程序中跟踪 `useIsSignedIn` 用户的登录状态。</span><span class="sxs-lookup"><span data-stu-id="28f46-166">Add a custom function named `useIsSignedIn` that enables tracking the user's sign in state in your application.</span></span>

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

<span data-ttu-id="28f46-167">此函数执行两项操作。</span><span class="sxs-lookup"><span data-stu-id="28f46-167">This function does two things.</span></span> <span data-ttu-id="28f46-168">首先，使用 React `useState` 挂钩，它可以在组件内启用跟踪状态。</span><span class="sxs-lookup"><span data-stu-id="28f46-168">First, using the React `useState` hook, it enables tracking state inside your component.</span></span> <span data-ttu-id="28f46-169">只要状态发生更改，React 就会重新呈现你的组件。</span><span class="sxs-lookup"><span data-stu-id="28f46-169">Whenever the state changes, React will re-render your component.</span></span> <span data-ttu-id="28f46-170">其次，使用 React 挂钩，它通过跟踪 Microsoft Graph Toolkit提供程序中的更改并在必要时更新组件来扩展 `useEffect` 组件的生命周期。</span><span class="sxs-lookup"><span data-stu-id="28f46-170">Second, using the React `useEffect` hook, it extends the component's lifecycle by tracking changes in the Microsoft Graph Toolkit provider and updating the component if necessary.</span></span>

#### <a name="load-users-calendar-if-user-is-signed-in"></a><span data-ttu-id="28f46-171">如果用户已登录，则加载用户的日历</span><span class="sxs-lookup"><span data-stu-id="28f46-171">Load user's calendar if user is signed in</span></span>

<span data-ttu-id="28f46-172">现在，在应用程序中跟踪用户的登录状态，可以在用户登录后显示其日历。</span><span class="sxs-lookup"><span data-stu-id="28f46-172">Now that you track the user's sign in state in your application, you can show their calendar after they signed in.</span></span>

1. <span data-ttu-id="28f46-173">在代码编辑器中，打开 **src/App.tsx** 文件，在 **App** 函数内添加：</span><span class="sxs-lookup"><span data-stu-id="28f46-173">In the code editor, open the **src/App.tsx** file, and inside the **App** function, add:</span></span>

    ```tsx
    const [isSignedIn] = useIsSignedIn();
    ```

    <span data-ttu-id="28f46-174">这将定义一个布尔常量，该常量可用于确定用户当前 `isSignedIn` 是否已登录到您的应用程序。</span><span class="sxs-lookup"><span data-stu-id="28f46-174">This defines a Boolean `isSignedIn` constant, which you can use to determine whether the user is currently signed in to your application.</span></span>

1. <span data-ttu-id="28f46-175">使用附加组件 `return` 和 Microsoft Graph Toolkit `div` 扩展子句的内容。</span><span class="sxs-lookup"><span data-stu-id="28f46-175">Extend the contents of the `return` clause with an additional `div` and the Microsoft Graph Toolkit Agenda component.</span></span>

    ```tsx
    <div>
      {isSignedIn &&
        <Agenda />}
    </div>
    ```

<span data-ttu-id="28f46-176">借助这些更改 **，src/App.tsx** 文件应如下所示。</span><span class="sxs-lookup"><span data-stu-id="28f46-176">With these changes, the **src/App.tsx** file should look like the following.</span></span>

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

### <a name="test-showing-users-calendar-after-they-signed-in"></a><span data-ttu-id="28f46-177">测试显示用户登录后的日历</span><span class="sxs-lookup"><span data-stu-id="28f46-177">Test showing user's calendar after they signed in</span></span>

<span data-ttu-id="28f46-178">借助这些更改，使用 Microsoft 帐户登录应用程序后，应该会看到日历。</span><span class="sxs-lookup"><span data-stu-id="28f46-178">With these changes, after signing in to your application with your Microsoft account, you should see your calendar.</span></span>

1. <span data-ttu-id="28f46-179">To see the changes， close the browser and open it again， and go to `http://localhost:3000` .</span><span class="sxs-lookup"><span data-stu-id="28f46-179">To see the changes, close the browser and open it again, and go to `http://localhost:3000`.</span></span> <span data-ttu-id="28f46-180">你这样做是因为你更改了属性的值，这将影响从 `scopes` Azure AD 请求的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="28f46-180">You do this because you changed the value of the `scopes` property, which affects the access token that you request from Azure AD.</span></span>
1. <span data-ttu-id="28f46-181">选择 **"登录"** 按钮，然后使用 Microsoft 帐户登录。</span><span class="sxs-lookup"><span data-stu-id="28f46-181">Choose the **Sign In** button and sign in using your Microsoft account.</span></span> <span data-ttu-id="28f46-182">请注意同意提示中请求的权限列表的新增内容。</span><span class="sxs-lookup"><span data-stu-id="28f46-182">Notice the additions to the list of permissions requested in the consent prompt.</span></span> <span data-ttu-id="28f46-183">这是因为属性中包含了其他 `scope` 权限。</span><span class="sxs-lookup"><span data-stu-id="28f46-183">This is because you included additional permissions in the `scope` property.</span></span>
1. <span data-ttu-id="28f46-184">同意使用应用程序后，应看到有关当前用户及其日历的信息。</span><span class="sxs-lookup"><span data-stu-id="28f46-184">After consenting to the use of the application, you should see information about the current user and their calendar.</span></span>

![已完成的应用](../images/mgt-finished-app.png)

## <a name="next-steps"></a><span data-ttu-id="28f46-186">后续步骤</span><span class="sxs-lookup"><span data-stu-id="28f46-186">Next steps</span></span>

- <span data-ttu-id="28f46-187">查看[Microsoft Graph Toolkit。](../overview.md)</span><span class="sxs-lookup"><span data-stu-id="28f46-187">See [what's in the Microsoft Graph Toolkit](../overview.md).</span></span>
- <span data-ttu-id="28f46-188">尝试在运动场 [中的组件](https://mgt.dev)。</span><span class="sxs-lookup"><span data-stu-id="28f46-188">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="28f46-189">在 Stack [Overflow](https://aka.ms/mgt-question)上提问。</span><span class="sxs-lookup"><span data-stu-id="28f46-189">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="28f46-190">在 GitHub 上报告 Bug 或保留 [功能请求](https://aka.ms/mgt)。</span><span class="sxs-lookup"><span data-stu-id="28f46-190">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
