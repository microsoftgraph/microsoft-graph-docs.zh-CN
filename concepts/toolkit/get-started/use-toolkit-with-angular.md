---
title: 使用具有角度的 Microsoft Graph 工具包
description: 开始在角度应用程序中使用 Microsoft Graph 工具包。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: be84107314a9696486b377f09dc399d6e15c44cf
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288502"
---
# <a name="use-the-microsoft-graph-toolkit-with-angular"></a><span data-ttu-id="4a69b-103">使用具有角度的 Microsoft Graph 工具包</span><span class="sxs-lookup"><span data-stu-id="4a69b-103">Use the Microsoft Graph Toolkit with Angular</span></span>

<span data-ttu-id="4a69b-104">除了 vanilla JavaScript 和 HTML 之外，Microsoft Graph 工具包组件也适用于 web 框架等 web 框架。</span><span class="sxs-lookup"><span data-stu-id="4a69b-104">Microsoft Graph Toolkit components work great with web frameworks like Angular in addition to vanilla JavaScript and HTML.</span></span> <span data-ttu-id="4a69b-105">本主题介绍如何使用具有角度的 Microsoft Graph 工具包。</span><span class="sxs-lookup"><span data-stu-id="4a69b-105">This topic describes how to use the Microsoft Graph Toolkit with Angular.</span></span> <span data-ttu-id="4a69b-106">有关介绍如何创建新的角度应用程序和使用 Microsoft Graph 工具包的分步演练，请参阅 [使用具有角度的 Microsoft Graph 工具包](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/)。</span><span class="sxs-lookup"><span data-stu-id="4a69b-106">For a step-by-step walkthrough that describes how to create a new Angular application and use the Microsoft Graph Toolkit, see [Using Microsoft Graph Toolkit with Angular](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span></span>

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="4a69b-107">添加 Microsoft Graph 工具包</span><span class="sxs-lookup"><span data-stu-id="4a69b-107">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="4a69b-108">首先，您需要通过将添加到中的来启用角度应用程序中的自定义元素 `CUSTOM_ELEMENT_SCHEMA` `@NgModule() decorator` `app.module.ts` 。</span><span class="sxs-lookup"><span data-stu-id="4a69b-108">First, you need to enable custom elements in your Angular application by adding the `CUSTOM_ELEMENT_SCHEMA` to the `@NgModule() decorator` in `app.module.ts`.</span></span> <span data-ttu-id="4a69b-109">以下示例显示了具体的操作方法：</span><span class="sxs-lookup"><span data-stu-id="4a69b-109">The following example shows how to do this:</span></span>
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
<span data-ttu-id="4a69b-110">接下来，通过以下方式安装 npm 程序包以将 Microsoft Graph 工具包添加到项目中：</span><span class="sxs-lookup"><span data-stu-id="4a69b-110">Next, add the Microsoft Graph Toolkit to your project by installing the npm package with:</span></span>
```bash
npm install @microsoft/mgt
```
## <a name="initialize-a-provider"></a><span data-ttu-id="4a69b-111">初始化提供程序</span><span class="sxs-lookup"><span data-stu-id="4a69b-111">Initialize a provider</span></span>

<span data-ttu-id="4a69b-112">Microsoft Graph 工具包提供程序启用对组件的 Microsoft Graph 的身份验证和访问。</span><span class="sxs-lookup"><span data-stu-id="4a69b-112">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="4a69b-113">若要了解详细信息，请参阅 [使用提供程序](../providers.md)。</span><span class="sxs-lookup"><span data-stu-id="4a69b-113">To learn more, see [Using the providers](../providers.md).</span></span> <span data-ttu-id="4a69b-114">您使用的提供程序取决于将在其中使用解决方案的上下文。</span><span class="sxs-lookup"><span data-stu-id="4a69b-114">The provider you use depends on the context in which your solution will be used.</span></span>

<span data-ttu-id="4a69b-115">下面的示例展示了如何添加 [MSAL 提供程序](../providers/msal.md)，但您可以使用与任何提供程序相同的模型。</span><span class="sxs-lookup"><span data-stu-id="4a69b-115">The following example shows how to add the [MSAL Provider](../providers/msal.md), but you can follow the same model with any of the providers.</span></span> <span data-ttu-id="4a69b-116">导入提供程序并将其设置为在应用程序初始化时初始化。</span><span class="sxs-lookup"><span data-stu-id="4a69b-116">Import the provider and set it to initialize when the application initializes.</span></span> <span data-ttu-id="4a69b-117">将替换为 `<YOUR-CLIENT-ID>` 应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="4a69b-117">Replace `<YOUR-CLIENT-ID>` with the client ID for your application.</span></span>

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
### <a name="create-an-appclient-id"></a><span data-ttu-id="4a69b-118">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="4a69b-118">Create an app/client ID</span></span>
<span data-ttu-id="4a69b-119">为了获取客户端 ID，需要在 Azure AD 中 [注册应用程序](../../auth-register-app-v2.md) 。</span><span class="sxs-lookup"><span data-stu-id="4a69b-119">In order to get a client ID, you need to [register your application](../../auth-register-app-v2.md) in Azure AD.</span></span> 
><span data-ttu-id="4a69b-120">**注意**： MSAL 仅支持 OAuth 的隐式流。</span><span class="sxs-lookup"><span data-stu-id="4a69b-120">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="4a69b-121">请务必在 Azure 门户中的应用程序中启用隐式流， (默认情况下不启用它) 。</span><span class="sxs-lookup"><span data-stu-id="4a69b-121">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="4a69b-122">在 " **身份验证**" 下，找到 " **隐式授予** " 部分，然后选择 " **访问令牌** " 和 **ID 令牌**的复选框。</span><span class="sxs-lookup"><span data-stu-id="4a69b-122">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span>

## <a name="add-components"></a><span data-ttu-id="4a69b-123">添加组件</span><span class="sxs-lookup"><span data-stu-id="4a69b-123">Add components</span></span>

<span data-ttu-id="4a69b-124">现在，您可以像在 HTML 模板中那样正常使用任何 Microsoft Graph 工具包组件。</span><span class="sxs-lookup"><span data-stu-id="4a69b-124">Now, you can use any of the Microsoft Graph Toolkit components as you normally would in your HTML templates.</span></span> <span data-ttu-id="4a69b-125">例如，若要添加 " [人员" 组件](../components/person.md)，请向模板中添加以下内容：</span><span class="sxs-lookup"><span data-stu-id="4a69b-125">For example, to add the [Person component](../components/person.md),  add the following to your template:</span></span>

```html
<mgt-person person-query="me" view="twolines"></mgt-person>
```

## <a name="customizing-components-with-angular"></a><span data-ttu-id="4a69b-126">使用角自定义组件</span><span class="sxs-lookup"><span data-stu-id="4a69b-126">Customizing components with Angular</span></span>

<span data-ttu-id="4a69b-127">所有 Microsoft Graph 工具包组件都支持 [自定义模板](../templates.md)，从而允许您修改组件的内容。</span><span class="sxs-lookup"><span data-stu-id="4a69b-127">All Microsoft Graph Toolkit components support [custom templates](../templates.md), which allow you to modify the content of a component.</span></span> <span data-ttu-id="4a69b-128">自定义组件的默认语法是使用双花括号来引用每个返回项的属性数据，如下所示：</span><span class="sxs-lookup"><span data-stu-id="4a69b-128">The default syntax for customizing the components is to use double braces to refer to the property data for each of the returned items, as shown:</span></span>

```html
<!-- Double braces are used for data binding in Angular. This will throw an error. -->
<mgt-agenda>
    <template data-type="event">
        <div>{{event.subject}}</div>
    </template>
</mgt-agenda>
```

<span data-ttu-id="4a69b-129">但是，在角度而言，如果您尝试使用双大括号语法，则双大括号用于数据绑定，而角度编译器将引发错误。</span><span class="sxs-lookup"><span data-stu-id="4a69b-129">In Angular, however, double braces are used for data binding and the Angular compiler will throw an error if you try to use the double brace syntax.</span></span>

<span data-ttu-id="4a69b-130">您可以通过将工具箱使用的默认字符更改为双括号以外的其他字符，从而避免这些错误 `TemplateHelper` 。</span><span class="sxs-lookup"><span data-stu-id="4a69b-130">You can avoid these errors by changing the default characters used by the Toolkit to something other than double braces by using the `TemplateHelper`.</span></span> <span data-ttu-id="4a69b-131">最好在顶级应用组件中执行此操作，以便全局应用。</span><span class="sxs-lookup"><span data-stu-id="4a69b-131">It is best to do this in your top-level App component so that it applies globally.</span></span>

<span data-ttu-id="4a69b-132">导入 `TemplateHelper` 并使用 `.setBindingSyntax()` 方法设置自定义绑定语法。</span><span class="sxs-lookup"><span data-stu-id="4a69b-132">Import the `TemplateHelper` and use the `.setBindingSyntax()` method to set your custom binding syntax.</span></span>

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
<span data-ttu-id="4a69b-133">现在，您可以使用自定义绑定语法定义自定义模板。</span><span class="sxs-lookup"><span data-stu-id="4a69b-133">Now, you can use your custom binding syntax to define custom templates.</span></span>

```html
<mgt-agenda>
    <template data-type="event">
        <div>[[event.subject]]</div>
    </template>
</mgt-agenda>
```

## <a name="next-steps"></a><span data-ttu-id="4a69b-134">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4a69b-134">Next steps</span></span>
- <span data-ttu-id="4a69b-135">请参阅本分步教程，了解如何 [生成角度应用](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/)。</span><span class="sxs-lookup"><span data-stu-id="4a69b-135">Check out this step-by-step tutorial on [building an Angular app](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span></span>
- <span data-ttu-id="4a69b-136">尝试 [样本](https://mgt.dev)中的组件。</span><span class="sxs-lookup"><span data-stu-id="4a69b-136">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="4a69b-137">在 [堆栈溢出](https://aka.ms/mgt-question)时提出问题。</span><span class="sxs-lookup"><span data-stu-id="4a69b-137">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="4a69b-138">在 [GitHub](https://aka.ms/mgt)上报告错误或保留功能请求。</span><span class="sxs-lookup"><span data-stu-id="4a69b-138">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>