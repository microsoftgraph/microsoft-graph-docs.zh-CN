---
title: 将 Microsoft Graph Toolkit与 Angular
description: 在应用程序应用程序中Graph Toolkit Microsoft Angular入门。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 1390b29c94fef292433e1e422fa5c44fd480e1eb
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579884"
---
# <a name="use-the-microsoft-graph-toolkit-with-angular"></a>将 Microsoft Graph Toolkit与 Angular

除了Graph Toolkit JavaScript 和 HTML 外，Microsoft Angular 还非常支持 Web 框架（如 web 框架）。 本主题介绍如何将 Microsoft Graph Toolkit与 Angular。 有关介绍如何创建新的 Angular 应用程序并使用 Microsoft Graph Toolkit 的分步演练，请参阅将[Microsoft](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/)Graph Toolkit 与 Angular。

## <a name="add-the-microsoft-graph-toolkit"></a>添加 Microsoft Graph Toolkit

首先，你需要通过将 添加到 中的 在 Angular 应用程序中启用 `CUSTOM_ELEMENT_SCHEMA` 自定义 `@NgModule() decorator` 元素 `app.module.ts` 。 以下示例显示了具体的操作方法：
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
接下来，通过Graph Toolkit npm 包将 Microsoft 加载项添加到项目中：
```bash
npm install @microsoft/mgt
```
## <a name="initialize-a-provider"></a>初始化提供程序

Microsoft Graph Toolkit提供程序支持对组件的 Microsoft Graph进行身份验证和访问。 若要了解更多信息，请参阅 [使用提供程序](../providers/providers.md)。 使用的提供程序取决于将使用解决方案的上下文。

以下示例演示如何添加 [MSAL 2 提供程序](../providers/msal2.md)，但您可以使用任何提供程序的相同模型。
>[!NOTE] 
>如果您当前使用的是 MSAL 提供程序，并且希望更新到 MSAL 2 提供程序，请按照 [MSAL 2](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider) 提供程序文章中的步骤操作。

导入提供程序，将其设置为在应用程序初始化时进行初始化。 将 `<YOUR-CLIENT-ID>` 替换为应用程序的客户端 ID。

```ts
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
### <a name="create-an-appclient-id"></a>创建应用/客户端 ID
若要获取客户端 ID，需要在 Azure AD 中 [注册](../../auth-register-app-v2.md) 应用程序。 

## <a name="add-components"></a>添加组件

现在，您可以像在 HTML 模板中Graph Toolkit一样使用任何 Microsoft 自定义组件。 例如，若要添加 ["人员"组件](../components/person.md)，请向模板中添加以下内容：

```html
<mgt-person person-query="me" view="twolines"></mgt-person>
```

## <a name="customizing-components-with-angular"></a>使用自定义组件Angular

所有 Microsoft Graph Toolkit组件都[](../customize-components/templates.md)支持自定义模板，这允许你修改组件的内容。 自定义组件的默认语法是使用双括号来引用每个返回项目的属性数据，如下所示：

```html
<!-- Double braces are used for data binding in Angular. This will throw an error. -->
<mgt-agenda>
    <template data-type="event">
        <div>{{event.subject}}</div>
    </template>
</mgt-agenda>
```

但是Angular，双括号用于数据绑定，如果尝试使用双大括号语法，Angular编译器将引发错误。

可以通过使用 将用户所使用的默认字符Toolkit大括号，而不是双括号，避免这些 `TemplateHelper` 错误。 最好在顶级应用组件中这样做，以便它可全局应用。

导入 `TemplateHelper` 并使用 `.setBindingSyntax()` 方法设置自定义绑定语法。

```ts
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
现在，您可以使用自定义绑定语法来定义自定义模板。

```html
<mgt-agenda>
    <template data-type="event">
        <div>[[event.subject]]</div>
    </template>
</mgt-agenda>
```

## <a name="next-steps"></a>后续步骤
- 请查看此有关生成应用应用的分步[Angular教程](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/)。
- 尝试在运动场中的 [组件](https://mgt.dev)。
- 在 Stack [Overflow 上提问](https://aka.ms/mgt-question)。
- 报告 Bug 或将功能请求[保留GitHub。](https://aka.ms/mgt)
