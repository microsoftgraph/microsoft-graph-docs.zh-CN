---
title: 将 Microsoft Graph Toolkit Angular
description: 在 Angular 应用程序中开始使用 Microsoft Graph Toolkit。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: a1c0ebc252545491dc57d8910eb283db6d227ccd
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49664042"
---
# <a name="use-the-microsoft-graph-toolkit-with-angular"></a><span data-ttu-id="f0cbb-103">将 Microsoft Graph Toolkit Angular</span><span class="sxs-lookup"><span data-stu-id="f0cbb-103">Use the Microsoft Graph Toolkit with Angular</span></span>

<span data-ttu-id="f0cbb-104">除了Toolkit JavaScript 和 HTML 之外，Microsoft Graph 组件还非常支持 Angular 等 Web 框架。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-104">Microsoft Graph Toolkit components work great with web frameworks like Angular in addition to vanilla JavaScript and HTML.</span></span> <span data-ttu-id="f0cbb-105">本主题介绍如何将 Microsoft Graph Toolkit Angular。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-105">This topic describes how to use the Microsoft Graph Toolkit with Angular.</span></span> <span data-ttu-id="f0cbb-106">有关介绍如何创建新的 Angular 应用程序和使用 Microsoft Graph Toolkit的分步演练，请参阅将 Microsoft Graph Toolkit [Angular。](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/)</span><span class="sxs-lookup"><span data-stu-id="f0cbb-106">For a step-by-step walkthrough that describes how to create a new Angular application and use the Microsoft Graph Toolkit, see [Using Microsoft Graph Toolkit with Angular](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span></span>

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="f0cbb-107">添加 Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="f0cbb-107">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="f0cbb-108">首先，你需要通过向 in 中添加来启用 Angular 应用程序中 `CUSTOM_ELEMENT_SCHEMA` 的自定义 `@NgModule() decorator` 元素 `app.module.ts` 。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-108">First, you need to enable custom elements in your Angular application by adding the `CUSTOM_ELEMENT_SCHEMA` to the `@NgModule() decorator` in `app.module.ts`.</span></span> <span data-ttu-id="f0cbb-109">以下示例显示了具体的操作方法：</span><span class="sxs-lookup"><span data-stu-id="f0cbb-109">The following example shows how to do this:</span></span>
```ts
import { BrowserModule } from '@angular/platform-browser';
import { NgModule, CUSTOM_ELEMENTS_SCHEMA } from '@angular/core';

import { AppComponent } from './app.component';

@NgModule({
  declarations: [AppComponent],
  imports: [BrowserModule],
  schemas: [CUSTOM_ELEMENTS_SCHEMA],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule {}
```
<span data-ttu-id="f0cbb-110">接下来，通过以下Toolkit npm 程序包，将 Microsoft Graph Toolkit添加到你的项目中：</span><span class="sxs-lookup"><span data-stu-id="f0cbb-110">Next, add the Microsoft Graph Toolkit to your project by installing the npm package with:</span></span>
```bash
npm install @microsoft/mgt
```
## <a name="initialize-a-provider"></a><span data-ttu-id="f0cbb-111">初始化提供程序</span><span class="sxs-lookup"><span data-stu-id="f0cbb-111">Initialize a provider</span></span>

<span data-ttu-id="f0cbb-112">Microsoft Graph Toolkit提供程序为组件启用身份验证并访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-112">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="f0cbb-113">若要了解更多信息，请参阅["使用提供程序"。](../providers/providers.md)</span><span class="sxs-lookup"><span data-stu-id="f0cbb-113">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="f0cbb-114">使用的提供程序取决于将使用解决方案的上下文。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-114">The provider you use depends on the context in which your solution will be used.</span></span>

<span data-ttu-id="f0cbb-115">以下示例显示如何添加 [MSAL 提供程序](../providers/msal.md)，但可以遵循任何提供程序的相同模型。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-115">The following example shows how to add the [MSAL Provider](../providers/msal.md), but you can follow the same model with any of the providers.</span></span> <span data-ttu-id="f0cbb-116">导入提供程序，将其设置为在应用程序初始化时初始化。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-116">Import the provider and set it to initialize when the application initializes.</span></span> <span data-ttu-id="f0cbb-117">替换为 `<YOUR-CLIENT-ID>` 应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-117">Replace `<YOUR-CLIENT-ID>` with the client ID for your application.</span></span>

```ts
import { Component, OnInit } from '@angular/core';
import { Providers, MsalProvider } from '@microsoft/mgt';

@Component({
    selector: 'app-root',
    templateUrl: './app.component.html',
    styleUrls: ['./app.component.css']
})
export class AppComponent implements OnInit {

    ngOnInit()
    {
        Providers.globalProvider = new MsalProvider({
            clientId: '<YOUR-CLIENT-ID>'
        });
    }
}
```
### <a name="create-an-appclient-id"></a><span data-ttu-id="f0cbb-118">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="f0cbb-118">Create an app/client ID</span></span>
<span data-ttu-id="f0cbb-119">若要获取客户端 ID，需要在 Azure AD 中 [注册](../../auth-register-app-v2.md) 应用程序。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-119">In order to get a client ID, you need to [register your application](../../auth-register-app-v2.md) in Azure AD.</span></span> 
><span data-ttu-id="f0cbb-120">**注意**：MSAL 仅支持 OAuth 的隐式流。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-120">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="f0cbb-121">请确保在 Azure 门户中启用应用程序中的隐式流 (默认情况下未启用它) 。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-121">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="f0cbb-122">在 **"身份验证**"下，找到 **隐式授予** 部分并选择 **访问** 令牌和 ID 令牌 **的复选框**。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-122">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span>

## <a name="add-components"></a><span data-ttu-id="f0cbb-123">添加组件</span><span class="sxs-lookup"><span data-stu-id="f0cbb-123">Add components</span></span>

<span data-ttu-id="f0cbb-124">现在，你可以像在 HTML 模板中Toolkit一样使用任何 Microsoft Graph 组件。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-124">Now, you can use any of the Microsoft Graph Toolkit components as you normally would in your HTML templates.</span></span> <span data-ttu-id="f0cbb-125">例如，若要添加 [Person 组件](../components/person.md)，请向模板中添加以下内容：</span><span class="sxs-lookup"><span data-stu-id="f0cbb-125">For example, to add the [Person component](../components/person.md),  add the following to your template:</span></span>

```html
<mgt-person person-query="me" view="twolines"></mgt-person>
```

## <a name="customizing-components-with-angular"></a><span data-ttu-id="f0cbb-126">使用 Angular 自定义组件</span><span class="sxs-lookup"><span data-stu-id="f0cbb-126">Customizing components with Angular</span></span>

<span data-ttu-id="f0cbb-127">所有 Microsoft Graph Toolkit组件都[](../customize-components/templates.md)支持自定义模板，允许您修改组件的内容。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-127">All Microsoft Graph Toolkit components support [custom templates](../customize-components/templates.md), which allow you to modify the content of a component.</span></span> <span data-ttu-id="f0cbb-128">自定义组件的默认语法是使用双括号来引用每个返回项的属性数据，如下所示：</span><span class="sxs-lookup"><span data-stu-id="f0cbb-128">The default syntax for customizing the components is to use double braces to refer to the property data for each of the returned items, as shown:</span></span>

```html
<!-- Double braces are used for data binding in Angular. This will throw an error. -->
<mgt-agenda>
    <template data-type="event">
        <div>{{event.subject}}</div>
    </template>
</mgt-agenda>
```

<span data-ttu-id="f0cbb-129">但是，在 Angular 中，双括号用于数据绑定，如果尝试使用双括号语法，Angular 编译器将引发错误。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-129">In Angular, however, double braces are used for data binding and the Angular compiler will throw an error if you try to use the double brace syntax.</span></span>

<span data-ttu-id="f0cbb-130">可以通过使用 ...将 Toolkit 所使用的默认字符更改为双括号而非双括号，以避免这些错误 `TemplateHelper` 。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-130">You can avoid these errors by changing the default characters used by the Toolkit to something other than double braces by using the `TemplateHelper`.</span></span> <span data-ttu-id="f0cbb-131">最好在顶级应用组件中这样做，以便它全局应用。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-131">It is best to do this in your top-level App component so that it applies globally.</span></span>

<span data-ttu-id="f0cbb-132">导入 `TemplateHelper` 并使用 `.setBindingSyntax()` 方法设置自定义绑定语法。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-132">Import the `TemplateHelper` and use the `.setBindingSyntax()` method to set your custom binding syntax.</span></span>

```ts
import { Component, OnInit } from '@angular/core';
import { Providers, MsalProvider, TemplateHelper } from '@microsoft/mgt';

@Component({
    selector: 'app-root',
    templateUrl: './app.component.html',
    styleUrls: ['./app.component.css']
})
export class AppComponent implements OnInit {

    ngOnInit()
    {
        Providers.globalProvider = new MsalProvider({ clientId: '<YOUR-CLIENT-ID>'})
        TemplateHelper.setBindingSyntax('[[',']]');
    }
}
```
<span data-ttu-id="f0cbb-133">现在，您可以使用自定义绑定语法定义自定义模板。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-133">Now, you can use your custom binding syntax to define custom templates.</span></span>

```html
<mgt-agenda>
    <template data-type="event">
        <div>[[event.subject]]</div>
    </template>
</mgt-agenda>
```

## <a name="next-steps"></a><span data-ttu-id="f0cbb-134">后续步骤</span><span class="sxs-lookup"><span data-stu-id="f0cbb-134">Next steps</span></span>
- <span data-ttu-id="f0cbb-135">请查看此有关生成 Angular 应用的分步 [教程](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/)。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-135">Check out this step-by-step tutorial on [building an Angular app](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span></span>
- <span data-ttu-id="f0cbb-136">尝试在运动场 [中的组件](https://mgt.dev)。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-136">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="f0cbb-137">在 Stack [Overflow](https://aka.ms/mgt-question)上提问。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-137">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="f0cbb-138">在 GitHub 上报告 Bug 或保留 [功能请求](https://aka.ms/mgt)。</span><span class="sxs-lookup"><span data-stu-id="f0cbb-138">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>