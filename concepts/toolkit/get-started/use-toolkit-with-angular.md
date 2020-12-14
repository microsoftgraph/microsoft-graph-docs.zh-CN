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
# <a name="use-the-microsoft-graph-toolkit-with-angular"></a>将 Microsoft Graph Toolkit Angular

除了Toolkit JavaScript 和 HTML 之外，Microsoft Graph 组件还非常支持 Angular 等 Web 框架。 本主题介绍如何将 Microsoft Graph Toolkit Angular。 有关介绍如何创建新的 Angular 应用程序和使用 Microsoft Graph Toolkit的分步演练，请参阅将 Microsoft Graph Toolkit [Angular。](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/)

## <a name="add-the-microsoft-graph-toolkit"></a>添加 Microsoft Graph Toolkit

首先，你需要通过向 in 中添加来启用 Angular 应用程序中 `CUSTOM_ELEMENT_SCHEMA` 的自定义 `@NgModule() decorator` 元素 `app.module.ts` 。 以下示例显示了具体的操作方法：
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
接下来，通过以下Toolkit npm 程序包，将 Microsoft Graph Toolkit添加到你的项目中：
```bash
npm install @microsoft/mgt
```
## <a name="initialize-a-provider"></a>初始化提供程序

Microsoft Graph Toolkit提供程序为组件启用身份验证并访问 Microsoft Graph。 若要了解更多信息，请参阅["使用提供程序"。](../providers/providers.md) 使用的提供程序取决于将使用解决方案的上下文。

以下示例显示如何添加 [MSAL 提供程序](../providers/msal.md)，但可以遵循任何提供程序的相同模型。 导入提供程序，将其设置为在应用程序初始化时初始化。 替换为 `<YOUR-CLIENT-ID>` 应用程序的客户端 ID。

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
### <a name="create-an-appclient-id"></a>创建应用/客户端 ID
若要获取客户端 ID，需要在 Azure AD 中 [注册](../../auth-register-app-v2.md) 应用程序。 
>**注意**：MSAL 仅支持 OAuth 的隐式流。 请确保在 Azure 门户中启用应用程序中的隐式流 (默认情况下未启用它) 。 在 **"身份验证**"下，找到 **隐式授予** 部分并选择 **访问** 令牌和 ID 令牌 **的复选框**。

## <a name="add-components"></a>添加组件

现在，你可以像在 HTML 模板中Toolkit一样使用任何 Microsoft Graph 组件。 例如，若要添加 [Person 组件](../components/person.md)，请向模板中添加以下内容：

```html
<mgt-person person-query="me" view="twolines"></mgt-person>
```

## <a name="customizing-components-with-angular"></a>使用 Angular 自定义组件

所有 Microsoft Graph Toolkit组件都[](../customize-components/templates.md)支持自定义模板，允许您修改组件的内容。 自定义组件的默认语法是使用双括号来引用每个返回项的属性数据，如下所示：

```html
<!-- Double braces are used for data binding in Angular. This will throw an error. -->
<mgt-agenda>
    <template data-type="event">
        <div>{{event.subject}}</div>
    </template>
</mgt-agenda>
```

但是，在 Angular 中，双括号用于数据绑定，如果尝试使用双括号语法，Angular 编译器将引发错误。

可以通过使用 ...将 Toolkit 所使用的默认字符更改为双括号而非双括号，以避免这些错误 `TemplateHelper` 。 最好在顶级应用组件中这样做，以便它全局应用。

导入 `TemplateHelper` 并使用 `.setBindingSyntax()` 方法设置自定义绑定语法。

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
现在，您可以使用自定义绑定语法定义自定义模板。

```html
<mgt-agenda>
    <template data-type="event">
        <div>[[event.subject]]</div>
    </template>
</mgt-agenda>
```

## <a name="next-steps"></a>后续步骤
- 请查看此有关生成 Angular 应用的分步 [教程](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/)。
- 尝试在运动场 [中的组件](https://mgt.dev)。
- 在 Stack [Overflow](https://aka.ms/mgt-question)上提问。
- 在 GitHub 上报告 Bug 或保留 [功能请求](https://aka.ms/mgt)。