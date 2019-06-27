---
title: Microsoft Graph 工具包中的登录组件
description: 登录组件是一个按钮和飞出控件, 可促进 Microsoft 身份平台身份验证。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e7c657b3b6c9772b2d7b7b8e64a57c9982f4caef
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242972"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的登录组件

登录组件是一个按钮和飞出控件, 可促进 Microsoft 身份平台身份验证。 它提供了两种状态:
* 当用户未登录时, 该控件是启动登录过程的简单按钮。
* 当用户登录时, 该控件将显示当前登录的用户名、配置文件图像和电子邮件中的名称。 单击时, 将打开一个带有注销命令的浮出控件。

## <a name="example"></a>示例

[jsfiddle 示例](https://jsfiddle.net/metulev/scb9muh4)

```html
<mgt-login></mgt-login>
```

## <a name="using-the-control-without-an-authentication-provider"></a>在不使用身份验证提供程序的情况下使用控件

组件与提供程序一起使用, 并在盒中使用 Microsoft Graph。 但是, 如果您希望提供自己的逻辑和身份验证, 则可以使用`userDetails`属性来设置登录用户的详细信息。 

| 属性 | 属性 | 说明 |
| --- | --- | -- |
| `userDetails` | `user-details` | 设置将在控件上显示的 user 对象。 |

下面的示例设置人员的详细信息。

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    email: 'nikola@contoso.com',
    profileImage: 'url'
}
```

设置`userDetails`为`null`将转到 "已注销" 状态。

使用`loginInitiated`和`logoutInitiated`事件处理登录和注销。 

## <a name="css-custom-properties"></a>CSS 自定义属性

`mgt-login`组件定义以下 CSS 自定义属性。

```css
mgt-login {
  --font-size: 14px;
  --font-weight: 600;
  --height: '100%';
  --margin: 0;
  --padding: 12px 20px;
  --color: #201f1e;
  --background-color: transparent;
  --background-color--hover: #edebe9;
  --popup-content-background-color: white;
  --popup-command-font-size: 12px; }
}
```

若要了解详细信息, 请参阅[样式组件](../style.md)。

## <a name="events"></a>事件

从控件触发以下事件。

| 事件 | 说明 |
| --- | --- |
| `loginInitiated` | 用户单击了 "登录" 按钮以启动登录过程 (可取消)。|
| `loginCompleted` | 登录过程成功, 用户现在已登录。 |
| `loginFailed` | 用户取消了登录进程或无法登录。|
| `logoutInitiated` | 用户已开始注销。 |
| `logoutCompleted` | 用户已注销。 |

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此组件使用 "[人员" 组件](./person.md)显示用户并继承所有权限。 

## <a name="authentication"></a>身份验证

登录控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。 
