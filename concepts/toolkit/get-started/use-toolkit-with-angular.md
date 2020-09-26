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
# <a name="use-the-microsoft-graph-toolkit-with-angular"></a>使用具有角度的 Microsoft Graph 工具包

除了 vanilla JavaScript 和 HTML 之外，Microsoft Graph 工具包组件也适用于 web 框架等 web 框架。 本主题介绍如何使用具有角度的 Microsoft Graph 工具包。 有关介绍如何创建新的角度应用程序和使用 Microsoft Graph 工具包的分步演练，请参阅 [使用具有角度的 Microsoft Graph 工具包](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/)。

## <a name="add-the-microsoft-graph-toolkit"></a>添加 Microsoft Graph 工具包

首先，您需要通过将添加到中的来启用角度应用程序中的自定义元素 `CUSTOM_ELEMENT_SCHEMA` `@NgModule() decorator` `app.module.ts` 。 以下示例显示了具体的操作方法：
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
接下来，通过以下方式安装 npm 程序包以将 Microsoft Graph 工具包添加到项目中：
```bash
npm install @microsoft/mgt
```
## <a name="initialize-a-provider"></a>初始化提供程序

Microsoft Graph 工具包提供程序启用对组件的 Microsoft Graph 的身份验证和访问。 若要了解详细信息，请参阅 [使用提供程序](../providers.md)。 您使用的提供程序取决于将在其中使用解决方案的上下文。

下面的示例展示了如何添加 [MSAL 提供程序](../providers/msal.md)，但您可以使用与任何提供程序相同的模型。 导入提供程序并将其设置为在应用程序初始化时初始化。 将替换为 `<YOUR-CLIENT-ID>` 应用程序的客户端 ID。

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
为了获取客户端 ID，需要在 Azure AD 中 [注册应用程序](../../auth-register-app-v2.md) 。 
>**注意**： MSAL 仅支持 OAuth 的隐式流。 请务必在 Azure 门户中的应用程序中启用隐式流， (默认情况下不启用它) 。 在 " **身份验证**" 下，找到 " **隐式授予** " 部分，然后选择 " **访问令牌** " 和 **ID 令牌**的复选框。

## <a name="add-components"></a>添加组件

现在，您可以像在 HTML 模板中那样正常使用任何 Microsoft Graph 工具包组件。 例如，若要添加 " [人员" 组件](../components/person.md)，请向模板中添加以下内容：

```html
<mgt-person person-query="me" view="twolines"></mgt-person>
```

## <a name="customizing-components-with-angular"></a>使用角自定义组件

所有 Microsoft Graph 工具包组件都支持 [自定义模板](../templates.md)，从而允许您修改组件的内容。 自定义组件的默认语法是使用双花括号来引用每个返回项的属性数据，如下所示：

```html
<!-- Double braces are used for data binding in Angular. This will throw an error. -->
<mgt-agenda>
    <template data-type="event">
        <div>{{event.subject}}</div>
    </template>
</mgt-agenda>
```

但是，在角度而言，如果您尝试使用双大括号语法，则双大括号用于数据绑定，而角度编译器将引发错误。

您可以通过将工具箱使用的默认字符更改为双括号以外的其他字符，从而避免这些错误 `TemplateHelper` 。 最好在顶级应用组件中执行此操作，以便全局应用。

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
- 请参阅本分步教程，了解如何 [生成角度应用](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/)。
- 尝试 [样本](https://mgt.dev)中的组件。
- 在 [堆栈溢出](https://aka.ms/mgt-question)时提出问题。
- 在 [GitHub](https://aka.ms/mgt)上报告错误或保留功能请求。