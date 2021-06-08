---
title: 将 Microsoft Graph Toolkit与 Angular
description: 在应用程序应用程序中Graph Toolkit Microsoft Angular入门。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: b1985598985f85c0f33676fee49656324c65c7c5
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813185"
---
# <a name="use-the-microsoft-graph-toolkit-with-angular"></a><span data-ttu-id="f3c8d-103">将 Microsoft Graph Toolkit与 Angular</span><span class="sxs-lookup"><span data-stu-id="f3c8d-103">Use the Microsoft Graph Toolkit with Angular</span></span>

<span data-ttu-id="f3c8d-104">除了Graph Toolkit JavaScript 和 HTML 外，Microsoft Angular 还非常支持 Web 框架（如 web 框架）。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-104">Microsoft Graph Toolkit components work great with web frameworks like Angular in addition to vanilla JavaScript and HTML.</span></span> <span data-ttu-id="f3c8d-105">本主题介绍如何将 Microsoft Graph Toolkit与 Angular。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-105">This topic describes how to use the Microsoft Graph Toolkit with Angular.</span></span> <span data-ttu-id="f3c8d-106">有关介绍如何创建新的 Angular 应用程序并使用 Microsoft Graph Toolkit 的分步演练，请参阅将[Microsoft](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/)Graph Toolkit 与 Angular。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-106">For a step-by-step walkthrough that describes how to create a new Angular application and use the Microsoft Graph Toolkit, see [Using Microsoft Graph Toolkit with Angular](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span></span>

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="f3c8d-107">添加 Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="f3c8d-107">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="f3c8d-108">首先，你需要通过将 添加到 中的 在 Angular 应用程序中启用 `CUSTOM_ELEMENT_SCHEMA` 自定义 `@NgModule() decorator` 元素 `app.module.ts` 。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-108">First, you need to enable custom elements in your Angular application by adding the `CUSTOM_ELEMENT_SCHEMA` to the `@NgModule() decorator` in `app.module.ts`.</span></span> <span data-ttu-id="f3c8d-109">以下示例显示了具体的操作方法：</span><span class="sxs-lookup"><span data-stu-id="f3c8d-109">The following example shows how to do this:</span></span>
```TypeScript
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
<span data-ttu-id="f3c8d-110">接下来，通过Graph Toolkit npm 包将 Microsoft 加载项添加到项目中：</span><span class="sxs-lookup"><span data-stu-id="f3c8d-110">Next, add the Microsoft Graph Toolkit to your project by installing the npm package with:</span></span>
```Command Line
npm install @microsoft/mgt
```
## <a name="initialize-a-provider"></a><span data-ttu-id="f3c8d-111">初始化提供程序</span><span class="sxs-lookup"><span data-stu-id="f3c8d-111">Initialize a provider</span></span>

<span data-ttu-id="f3c8d-112">Microsoft Graph Toolkit提供程序支持对组件的 Microsoft Graph进行身份验证和访问。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-112">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="f3c8d-113">若要了解更多信息，请参阅 [使用提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-113">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="f3c8d-114">使用的提供程序取决于将使用解决方案的上下文。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-114">The provider you use depends on the context in which your solution will be used.</span></span>

<span data-ttu-id="f3c8d-115">以下示例演示如何添加 [MSAL 2 提供程序](../providers/msal2.md)，但您可以使用任何提供程序的相同模型。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-115">The following example shows how to add the [MSAL 2 Provider](../providers/msal2.md), but you can follow the same model with any of the providers.</span></span>
>[!NOTE] 
><span data-ttu-id="f3c8d-116">如果您当前使用的是 MSAL 提供程序，并且希望更新到 MSAL 2 提供程序，请按照 [MSAL 2](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider) 提供程序文章中的步骤操作。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-116">If you are currently using the MSAL Provider and would like to update to the MSAL 2 Provider, follow the steps in the [MSAL 2 provider](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider) article.</span></span>

<span data-ttu-id="f3c8d-117">导入提供程序，将其设置为在应用程序初始化时进行初始化。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-117">Import the provider and set it to initialize when the application initializes.</span></span> <span data-ttu-id="f3c8d-118">将 `<YOUR-CLIENT-ID>` 替换为应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-118">Replace `<YOUR-CLIENT-ID>` with the client ID for your application.</span></span>

```TypeScript
import { Component, OnInit } from '@angular/core';
import { Providers, Msal2Provider } from '@microsoft/mgt';

@Component({
    selector: 'app-root',
    templateUrl: './app.component.html',
    styleUrls: ['./app.component.css']
})
export class AppComponent implements OnInit {

    ngOnInit()
    {
        Providers.globalProvider = new Msal2Provider({
            clientId: '<YOUR-CLIENT-ID>'
        });
    }
}
```
### <a name="create-an-appclient-id"></a><span data-ttu-id="f3c8d-119">创建应用/客户端 ID</span><span class="sxs-lookup"><span data-stu-id="f3c8d-119">Create an app/client ID</span></span>
<span data-ttu-id="f3c8d-120">若要获取客户端 ID，需要在 Azure AD 中 [注册](../../auth-register-app-v2.md) 应用程序。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-120">In order to get a client ID, you need to [register your application](../../auth-register-app-v2.md) in Azure AD.</span></span> 

## <a name="add-components"></a><span data-ttu-id="f3c8d-121">添加组件</span><span class="sxs-lookup"><span data-stu-id="f3c8d-121">Add components</span></span>

<span data-ttu-id="f3c8d-122">现在，您可以像在 HTML 模板中Graph Toolkit一样使用任何 Microsoft 自定义组件。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-122">Now, you can use any of the Microsoft Graph Toolkit components as you normally would in your HTML templates.</span></span> <span data-ttu-id="f3c8d-123">例如，若要添加 ["人员"组件](../components/person.md)，请向模板中添加以下内容：</span><span class="sxs-lookup"><span data-stu-id="f3c8d-123">For example, to add the [Person component](../components/person.md),  add the following to your template:</span></span>

```html
<mgt-person person-query="me" view="twolines"></mgt-person>
```

## <a name="customizing-components-with-angular"></a><span data-ttu-id="f3c8d-124">使用自定义组件Angular</span><span class="sxs-lookup"><span data-stu-id="f3c8d-124">Customizing components with Angular</span></span>

<span data-ttu-id="f3c8d-125">所有 Microsoft Graph Toolkit组件都[](../customize-components/templates.md)支持自定义模板，这允许你修改组件的内容。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-125">All Microsoft Graph Toolkit components support [custom templates](../customize-components/templates.md), which allow you to modify the content of a component.</span></span> <span data-ttu-id="f3c8d-126">自定义组件的默认语法是使用双括号来引用每个返回项目的属性数据，如下所示：</span><span class="sxs-lookup"><span data-stu-id="f3c8d-126">The default syntax for customizing the components is to use double braces to refer to the property data for each of the returned items, as shown:</span></span>

```html
<!-- Double braces are used for data binding in Angular. This will throw an error. -->
<mgt-agenda>
    <template data-type="event">
        <div>{{event.subject}}</div>
    </template>
</mgt-agenda>
```

<span data-ttu-id="f3c8d-127">但是Angular，双括号用于数据绑定，如果尝试使用双大括号语法，Angular编译器将引发错误。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-127">In Angular, however, double braces are used for data binding and the Angular compiler will throw an error if you try to use the double brace syntax.</span></span>

<span data-ttu-id="f3c8d-128">可以通过使用 将用户所使用的默认字符Toolkit大括号，而不是双括号，避免这些 `TemplateHelper` 错误。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-128">You can avoid these errors by changing the default characters used by the Toolkit to something other than double braces by using the `TemplateHelper`.</span></span> <span data-ttu-id="f3c8d-129">最好在顶级应用组件中这样做，以便它可全局应用。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-129">It is best to do this in your top-level App component so that it applies globally.</span></span>

<span data-ttu-id="f3c8d-130">导入 `TemplateHelper` 并使用 `.setBindingSyntax()` 方法设置自定义绑定语法。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-130">Import the `TemplateHelper` and use the `.setBindingSyntax()` method to set your custom binding syntax.</span></span>

```TypeScript
import { Component, OnInit } from '@angular/core';
import { Providers, Msal2Provider, TemplateHelper } from '@microsoft/mgt';

@Component({
    selector: 'app-root',
    templateUrl: './app.component.html',
    styleUrls: ['./app.component.css']
})
export class AppComponent implements OnInit {

    ngOnInit()
    {
        Providers.globalProvider = new Msal2Provider({ clientId: '<YOUR-CLIENT-ID>'})
        TemplateHelper.setBindingSyntax('[[',']]');
    }
}
```
<span data-ttu-id="f3c8d-131">现在，您可以使用自定义绑定语法来定义自定义模板。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-131">Now, you can use your custom binding syntax to define custom templates.</span></span>

```html
<mgt-agenda>
    <template data-type="event">
        <div>[[event.subject]]</div>
    </template>
</mgt-agenda>
```

## <a name="next-steps"></a><span data-ttu-id="f3c8d-132">后续步骤</span><span class="sxs-lookup"><span data-stu-id="f3c8d-132">Next steps</span></span>
- <span data-ttu-id="f3c8d-133">请查看此有关生成应用应用的分步[Angular教程](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/)。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-133">Check out this step-by-step tutorial on [building an Angular app](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span></span>
- <span data-ttu-id="f3c8d-134">尝试在运动场中的 [组件](https://mgt.dev)。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-134">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="f3c8d-135">在 Stack [Overflow 上提问](https://aka.ms/mgt-question)。</span><span class="sxs-lookup"><span data-stu-id="f3c8d-135">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="f3c8d-136">报告 Bug 或将功能请求[保留GitHub。](https://aka.ms/mgt)</span><span class="sxs-lookup"><span data-stu-id="f3c8d-136">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
