---
title: Microsoft Graph 工具包中的登录组件
description: 登录组件是一个按钮和飞出控件，可促进 Microsoft 身份平台身份验证。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 767894cc88fa40eb96655fc8979dd5b2ef8d4eba
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39919435"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="de5ff-103">Microsoft Graph 工具包中的登录组件</span><span class="sxs-lookup"><span data-stu-id="de5ff-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="de5ff-104">登录组件是一个按钮和飞出控件，可促进 Microsoft 身份平台身份验证。</span><span class="sxs-lookup"><span data-stu-id="de5ff-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="de5ff-105">它提供了两种状态：</span><span class="sxs-lookup"><span data-stu-id="de5ff-105">It provides two states:</span></span>
* <span data-ttu-id="de5ff-106">当用户未登录时，该控件是启动登录过程的简单按钮。</span><span class="sxs-lookup"><span data-stu-id="de5ff-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="de5ff-107">当用户登录时，该控件将显示当前登录的用户名、配置文件图像和电子邮件中的名称。</span><span class="sxs-lookup"><span data-stu-id="de5ff-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="de5ff-108">单击时，将打开一个带有注销命令的浮出控件。</span><span class="sxs-lookup"><span data-stu-id="de5ff-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="de5ff-109">示例</span><span class="sxs-lookup"><span data-stu-id="de5ff-109">Example</span></span>

[<span data-ttu-id="de5ff-110">jsfiddle 示例</span><span class="sxs-lookup"><span data-stu-id="de5ff-110">jsfiddle example</span></span>](https://jsfiddle.net/metulev/scb9muh4)

```html
<mgt-login></mgt-login>
```

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="de5ff-111">在不使用身份验证提供程序的情况下使用控件</span><span class="sxs-lookup"><span data-stu-id="de5ff-111">Using the control without an authentication provider</span></span>

<span data-ttu-id="de5ff-112">组件与提供程序一起使用，并在盒中使用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="de5ff-112">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="de5ff-113">但是，如果您希望提供自己的逻辑和身份验证，则可以使用`userDetails`属性来设置登录用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="de5ff-113">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="de5ff-114">属性</span><span class="sxs-lookup"><span data-stu-id="de5ff-114">Attribute</span></span> | <span data-ttu-id="de5ff-115">属性</span><span class="sxs-lookup"><span data-stu-id="de5ff-115">Property</span></span> | <span data-ttu-id="de5ff-116">说明</span><span class="sxs-lookup"><span data-stu-id="de5ff-116">Description</span></span> |
| --- | --- | -- |
| <span data-ttu-id="de5ff-117">用户-详细信息</span><span class="sxs-lookup"><span data-stu-id="de5ff-117">user-details</span></span> | <span data-ttu-id="de5ff-118">userDetails</span><span class="sxs-lookup"><span data-stu-id="de5ff-118">userDetails</span></span> | <span data-ttu-id="de5ff-119">设置将在控件上显示的 user 对象。</span><span class="sxs-lookup"><span data-stu-id="de5ff-119">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="de5ff-120">下面的示例设置人员的详细信息。</span><span class="sxs-lookup"><span data-stu-id="de5ff-120">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    email: 'nikola@contoso.com',
    profileImage: 'url'
}
```

<span data-ttu-id="de5ff-121">设置`userDetails`为`null`将转到 "已注销" 状态。</span><span class="sxs-lookup"><span data-stu-id="de5ff-121">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="de5ff-122">使用`loginInitiated`和`logoutInitiated`事件处理登录和注销。</span><span class="sxs-lookup"><span data-stu-id="de5ff-122">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="de5ff-123">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="de5ff-123">CSS custom properties</span></span>

<span data-ttu-id="de5ff-124">`mgt-login`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="de5ff-124">The `mgt-login` component defines the following CSS custom properties.</span></span>

```css
mgt-login {
  --font-size: 14px;
  --font-weight: 600;
  --height: '100%';
  --margin: 0;
  --padding: 12px 20px;
  --color: #201f1e;
  --color-hover: var(--theme-primary-color);
  --background-color: transparent;
  --background-color--hover: #edebe9;
  --popup-content-background-color: white;
  --popup-command-font-size: 12px;
  --popup-color: #201f1e;
}
```

<span data-ttu-id="de5ff-125">若要了解详细信息，请参阅[样式组件](../style.md)。</span><span class="sxs-lookup"><span data-stu-id="de5ff-125">To learn more, see [styling components](../style.md).</span></span>

## <a name="events"></a><span data-ttu-id="de5ff-126">事件</span><span class="sxs-lookup"><span data-stu-id="de5ff-126">Events</span></span>

<span data-ttu-id="de5ff-127">从控件触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="de5ff-127">The following events are fired from the control.</span></span>

| <span data-ttu-id="de5ff-128">事件</span><span class="sxs-lookup"><span data-stu-id="de5ff-128">Event</span></span> | <span data-ttu-id="de5ff-129">说明</span><span class="sxs-lookup"><span data-stu-id="de5ff-129">Description</span></span> |
| --- | --- |
| `loginInitiated` | <span data-ttu-id="de5ff-130">用户单击了 "登录" 按钮以启动登录过程（可取消）。</span><span class="sxs-lookup"><span data-stu-id="de5ff-130">The user clicked the sign in button to start the login process - cancelable.</span></span>|
| `loginCompleted` | <span data-ttu-id="de5ff-131">登录过程成功，用户现在已登录。</span><span class="sxs-lookup"><span data-stu-id="de5ff-131">the login process was successful and the user is now signed in.</span></span> |
| `loginFailed` | <span data-ttu-id="de5ff-132">用户取消了登录进程或无法登录。</span><span class="sxs-lookup"><span data-stu-id="de5ff-132">The user canceled the login process or was unable to sign in.</span></span>|
| `logoutInitiated` | <span data-ttu-id="de5ff-133">用户已开始注销。</span><span class="sxs-lookup"><span data-stu-id="de5ff-133">The user started to logout - cancelable.</span></span> |
| `logoutCompleted` | <span data-ttu-id="de5ff-134">用户已注销。</span><span class="sxs-lookup"><span data-stu-id="de5ff-134">The user signed out.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="de5ff-135">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="de5ff-135">Microsoft Graph permissions</span></span>

<span data-ttu-id="de5ff-136">此组件使用 "[人员" 组件](./person.md)显示用户并继承所有权限。</span><span class="sxs-lookup"><span data-stu-id="de5ff-136">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="de5ff-137">身份验证</span><span class="sxs-lookup"><span data-stu-id="de5ff-137">Authentication</span></span>

<span data-ttu-id="de5ff-138">登录控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="de5ff-138">The login control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 
