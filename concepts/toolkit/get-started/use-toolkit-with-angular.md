---
title: 将 Microsoft Graph Toolkit与 Angular
description: 开始应用程序Graph Toolkit Microsoft Angular。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 9131fa4a1e161c93983fea3d615ebd1fc78bf0b7
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588755"
---
# <a name="use-the-microsoft-graph-toolkit-with-angular"></a>将 Microsoft Graph Toolkit与 Angular

除了Graph Toolkit JavaScript 和 HTML 外，Microsoft Angular 组件还非常与 Web 框架（如 web 框架）一起运行。 本主题介绍如何将 Microsoft Graph Toolkit与 Angular。 有关介绍如何创建新的 Angular 应用程序并使用 Microsoft Graph Toolkit 的分步演练，请参阅将 [Microsoft](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/) Graph Toolkit 与 Angular。

## <a name="add-the-microsoft-graph-toolkit"></a>添加 Microsoft Graph Toolkit

首先，你需要通过将 添加到 中的 在 Angular 应用程序中启用`CUSTOM_ELEMENT_SCHEMA`自定义`@NgModule() decorator`元素`app.module.ts`。 以下示例显示了具体的操作方法：
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
接下来，通过Graph Toolkit npm 包将 Microsoft 客户端添加到项目中：
```Command Line
npm install @microsoft/mgt
```
## <a name="initialize-a-provider"></a>初始化提供程序

Microsoft Graph 工具包提供程序为组件启用身份验证和对 Microsoft Graph 的访问。 若要了解详细信息，请参阅[使用提供程序](../providers/providers.md)。 使用的提供程序取决于将使用解决方案的上下文。

以下示例演示如何添加 [MSAL2 提供程序](../providers/msal2.md)，但您可以使用任何提供程序遵循同一模型。
>[!NOTE] 
>如果当前使用的是 MSAL 提供程序，并且要更新到 MSAL2 提供程序，请按照 [MSAL2 提供程序文章中的步骤](../providers/msal2.md#migrating-from-msal-provider-to-msal2-provider) 操作。

导入提供程序，将其设置为在应用程序初始化时进行初始化。 将 `<YOUR-CLIENT-ID>` 替换为应用程序的客户端 ID。

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
### <a name="create-an-appclient-id"></a>创建应用/客户端 ID
若要获取客户端 ID，需要在客户端 ID 中[注册](../../auth-register-app-v2.md)Azure AD。 

## <a name="add-components"></a>添加组件

现在，您可以像在 HTML 模板中Graph Toolkit一样使用任何 Microsoft 自定义组件。 例如，若要添加 ["人员"组件](../components/person.md)，请向模板中添加以下内容：

```html
<mgt-person person-query="me" view="twolines"></mgt-person>
```

## <a name="customizing-components-with-angular"></a>使用自定义组件Angular

所有 Microsoft Graph Toolkit组件都支持自定义模板[](../customize-components/templates.md)，通过自定义模板可以修改组件的内容。 自定义组件的默认语法是使用双括号来引用每个返回项目的属性数据，如下所示：

```html
<!-- Double braces are used for data binding in Angular. This will throw an error. -->
<mgt-agenda>
    <template data-type="event">
        <div>{{event.subject}}</div>
    </template>
</mgt-agenda>
```

但是Angular，双括号用于数据绑定，如果尝试使用双大括号语法，Angular编译器将引发错误。

可以通过使用 将用户所使用的默认字符Toolkit双括号而非双括号来避免这些错误`TemplateHelper`。 最好在顶级应用组件中这样做，以便它可全局应用。

`TemplateHelper`导入 并使用 方法`.setBindingSyntax()`设置自定义绑定语法。

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
- 在[样本](https://mgt.dev)中试用组件。
- 在 [Stack Overflow](https://aka.ms/mgt-question) 上提问。
- 在 [GitHub](https://aka.ms/mgt) 上报告 bug 或提出功能请求。
