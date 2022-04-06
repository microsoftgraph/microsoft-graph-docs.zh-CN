---
title: Microsoft 服务中的登录Graph Toolkit
description: 登录组件是一个按钮和飞出控件，用于简化Microsoft 标识平台身份验证。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: fedf3a1ec1f49812b14b03d544a73a8a60baaeb3
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588818"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a>Microsoft 服务中的登录Graph Toolkit

登录组件是一个按钮和飞出控件，用于简化Microsoft 标识平台身份验证。 它提供两种状态：
* 当用户未登录时，控件是一个简单的按钮，用于启动登录过程。
* 用户登录后，控件将显示当前登录的用户名、个人资料图像和电子邮件。 单击后，将打开一个使用注销命令的飞出。

## <a name="example"></a>示例

以下示例显示了具有 `mgt-login` 已登录用户的组件。 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a>在没有身份验证提供程序的情况下使用控件

该组件适用于提供程序和 Microsoft Graph开箱即用。 但是，如果要提供自己的逻辑和身份验证， `userDetails` 可以使用 属性设置登录用户的详细信息。 

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

`null`设置为 `userDetails` 将转到已退出状态。

`loginInitiated`使用 和 `logoutInitiated` 事件处理登录和退出。 

## <a name="css-custom-properties"></a>CSS 自定义属性

组件 `mgt-login` 定义以下 CSS 自定义属性。

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

若要了解更多信息，请参阅 [设置组件样式](../customize-components/style.md)。

## <a name="events"></a>事件

从控件中触发以下事件。

事件 | 何时发出 | 自定义数据 | Cancelable | 气泡 | 使用自定义模板
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`loginInitiated` | 用户单击登录按钮以启动登录过程 | 无 | 是 | 否 | 是
`loginCompleted` | 登录过程成功，用户现在已登录 | 无 | 否 | 否 | 是
`loginFailed` | 用户已取消登录过程或无法登录 | 无 | 否 | 否 | 是
`logoutInitiated` | 用户开始注销 | 无 | 是 | 否 | 是
`logoutCompleted` | 用户已登录 | 无 | 否 | 否 | 是

有关处理事件的信息，请参阅 [事件](../customize-components/events.md)。

## <a name="templates"></a>模板

组件 `mgt-login` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。 若要指定模板，请 `<template>` 包含组件内的元素， `data-type` 将值设置为下表中列出的值之一。 

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| signed-in-button-content | personDetails： person object， `personImage`： person image string | 用于当用户登录时在按钮中呈现内容的模板。 |
| signed-out-button-content | 空 | 用于当用户未登录时在按钮中呈现内容的模板。 |
| flyout-commands | handleSignOut：注销函数 | 用于在飞出控件中呈现命令的模板 |
| flyout-person-details | personDetails： person object， personImage： person image string | 用于在飞出控件中呈现人员详细信息的模板。 |

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此组件使用下列 Microsoft Graph API 和权限：

| 配置 | 权限 | API
| - | - | - |
| default | User.Read | [/users/me/](/graph/api/user-get) |

使用默认和`signed-in-button-content``flyout-person-details`模板时，此组件使用 [Person](./person.md) 组件显示用户并继承所有权限。

## <a name="authentication"></a>身份验证

登录控件使用身份验证文档中介绍的全局 [身份验证提供程序](../providers/providers.md)。 

## <a name="cache"></a>缓存

此组件使用 [Person 组件](./person.md) 显示用户，并继承该用户的所有缓存配置。

## <a name="extend-for-more-control"></a>扩展以了解更多控件

对于更复杂的方案或真正自定义的 UX `protected render*` ，此组件公开了多个在组件扩展中替代的方法。

| 方法 | 说明 |
| - | - |
| renderButton | 呈现按钮部件版式。 |
| renderButtonContent | 呈现按钮内容。 |
| renderSignedInButtonContent | 当用户登录时呈现按钮内容。 |
| renderSignedOutButtonContent | 当用户未登录时呈现按钮内容。 |
| renderFlyout | 呈现飞出部件版式。 |
| renderFlyoutContent | 呈现飞出内容。 |
| renderFlyoutPersonDetails | 呈现飞出人员详细信息。 |
| renderFlyoutCommands | 呈现飞出命令。 |

### <a name="bring-your-own-flyout"></a>自带飞出

通过替代 方法 `renderFlyout()` 并提供新的飞出，可以使用自己的飞出组件来替代内置组件。

在这种情况下，通过 `protected` 覆盖飞出显示方法来更新备用飞出视图的可见性，确保登录组件继续按预期工作。

| 方法 | 说明 |
| - | - |
| hideFlyout | 消除该飞出区。 |
| showFlyout | 显示飞出。 |
| toggleFlyout | 切换飞出状态。 |
