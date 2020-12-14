---
title: Login component in the Microsoft Graph Toolkit
description: 登录组件是一个按钮和飞出控件，用于简化 Microsoft 标识平台身份验证。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: a54dfaede64216e8a2254aedb06cf6aa41aaa295
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660063"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a>Login component in the Microsoft Graph Toolkit

登录组件是一个按钮和飞出控件，用于简化 Microsoft 标识平台身份验证。 它提供两种状态：
* 当用户未登录时，控件是启动登录过程的一个简单按钮。
* 用户登录后，控件将显示当前登录的用户名、个人资料图像和电子邮件。 单击后，将打开一个显示注销命令的飞出。

## <a name="example"></a>示例

以下示例显示了 `mgt-login` 具有已登录用户的组件。 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a>在没有身份验证提供程序的情况下使用控件

该组件适用于提供程序和开箱即用 Microsoft Graph。 但是，如果要提供自己的逻辑和身份验证，可以使用该属性设置 `userDetails` 登录用户的详细信息。 

| 属性 | 属性 | 说明 |
| --- | --- | -- |
| user-details | userDetails | 设置将在控件上显示的用户对象。 |

以下示例设置人员详细信息。

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    mail: 'nikola@contoso.com',
    personImage: 'url'
}
```

设置为 `userDetails` `null` 将转到已签名状态。

使用 `loginInitiated` and `logoutInitiated` 事件处理登录和退出。 

## <a name="css-custom-properties"></a>CSS 自定义属性

该 `mgt-login` 组件定义以下 CSS 自定义属性。

```css
mgt-login {
  --font-size: 14px;
  --font-weight: 600;
  --weith: '100%';
  --height: '100%';
  --margin: 0;
  --padding: 12px 20px;
  --button-color: #201f1e;
  --button-color--hover: var(--theme-primary-color);
  --button-background-color: transparent;
  --button-background-color--hover: #edebe9;
  --popup-background-color: white;
  --popup-command-font-size: 12px;
  --popup-color: #201f1e;
}
```

若要了解更多信息，请参阅 [样式组件](../customize-components/style.md)。

## <a name="events"></a>活动

从控件中触发以下事件。

| 事件 | 说明 |
| --- | --- |
| `loginInitiated` | 用户单击登录按钮以启动登录过程 - 可取消。|
| `loginCompleted` | 登录过程成功，用户现在已登录。 |
| `loginFailed` | 用户已取消登录过程或无法登录。|
| `logoutInitiated` | 用户开始注销 - 可取消。 |
| `logoutCompleted` | 用户已登录。 |

## <a name="templates"></a>模板

该 `mgt-login` 组件支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。 若要指定模板，请包含组件中的元素，将值设置为下表 `<template>` `data-type` 中列出的值之一。 

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| 登录按钮内容 | personDetails： person 对象， `personImage` ： person 图像字符串 | 用于在用户登录时呈现按钮中内容的模板。 |
| signed-out-button-content | 空 | 用于在用户未登录时呈现按钮中内容的模板。 |
| flyout-commands | handleSignOut：注销函数 | 用于在飞出控件中呈现命令的模板 |
| flyout-person-details | personDetails： person object， personImage： person image string | 用于在飞出控件中呈现人员详细信息的模板。 |

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此组件使用 [Person 组件](./person.md) 显示用户并继承所有权限。 

## <a name="authentication"></a>身份验证

登录控件使用身份验证文档中介绍的全局 [身份验证提供程序](../providers/providers.md)。 

## <a name="extend-for-more-control"></a>扩展以更多控制

对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展中 `protected render*` 替代的方法。

| 方法 | 说明 |
| - | - |
| renderButton | 呈现按钮部件版式。 |
| renderButtonContent | 呈现按钮内容。 |
| renderSignedInButtonContent | 在用户登录时呈现按钮内容。 |
| renderSignedOutButtonContent | 当用户未登录时呈现按钮内容。 |
| renderFlyout | 呈现飞出部件版式。 |
| renderFlyoutContent | 呈现飞出内容。 |
| renderFlyoutPersonDetails | 呈现飞出人员详细信息。 |
| renderFlyoutCommands | 呈现飞出命令。 |

### <a name="bring-your-own-flyout"></a>自带飞出

通过替代方法并提供新的飞出，可以使用你自己的飞出组件来替代内置 `renderFlyout()` 组件。

在这种情况下，通过替代飞出显示方法更新备用飞出视图的可见性，确保登录组件继续按预期 `protected` 工作。

| 方法 | 说明 |
| - | - |
| hideFlyout | 消除该飞出。 |
| showFlyout | 显示飞出。 |
| toggleFlyout | 切换飞出状态。 |
