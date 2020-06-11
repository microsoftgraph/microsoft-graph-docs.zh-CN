---
title: Microsoft Graph 工具包中的登录组件
description: 登录组件是一个按钮和飞出控件，可促进 Microsoft 身份平台身份验证。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 441639c309025eb8fefbbe551dd60b6324a7fd3c
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682031"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="81d38-103">Microsoft Graph 工具包中的登录组件</span><span class="sxs-lookup"><span data-stu-id="81d38-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="81d38-104">登录组件是一个按钮和飞出控件，可促进 Microsoft 身份平台身份验证。</span><span class="sxs-lookup"><span data-stu-id="81d38-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="81d38-105">它提供了两种状态：</span><span class="sxs-lookup"><span data-stu-id="81d38-105">It provides two states:</span></span>
* <span data-ttu-id="81d38-106">当用户未登录时，该控件是启动登录过程的简单按钮。</span><span class="sxs-lookup"><span data-stu-id="81d38-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="81d38-107">当用户登录时，该控件将显示当前登录的用户名、配置文件图像和电子邮件中的名称。</span><span class="sxs-lookup"><span data-stu-id="81d38-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="81d38-108">单击时，将打开一个带有注销命令的浮出控件。</span><span class="sxs-lookup"><span data-stu-id="81d38-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="81d38-109">示例</span><span class="sxs-lookup"><span data-stu-id="81d38-109">Example</span></span>

<span data-ttu-id="81d38-110">以下示例显示 `mgt-login` 具有已登录用户的组件。</span><span class="sxs-lookup"><span data-stu-id="81d38-110">The following example shows the `mgt-login` component with a signed-in user.</span></span> 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[<span data-ttu-id="81d38-111">在 "dev" 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="81d38-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="81d38-112">在不使用身份验证提供程序的情况下使用控件</span><span class="sxs-lookup"><span data-stu-id="81d38-112">Using the control without an authentication provider</span></span>

<span data-ttu-id="81d38-113">组件与提供程序一起使用，并在盒中使用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="81d38-113">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="81d38-114">但是，如果您希望提供自己的逻辑和身份验证，则可以使用 `userDetails` 属性来设置登录用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="81d38-114">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="81d38-115">属性</span><span class="sxs-lookup"><span data-stu-id="81d38-115">Attribute</span></span> | <span data-ttu-id="81d38-116">属性</span><span class="sxs-lookup"><span data-stu-id="81d38-116">Property</span></span> | <span data-ttu-id="81d38-117">说明</span><span class="sxs-lookup"><span data-stu-id="81d38-117">Description</span></span> |
| --- | --- | -- |
| <span data-ttu-id="81d38-118">用户-详细信息</span><span class="sxs-lookup"><span data-stu-id="81d38-118">user-details</span></span> | <span data-ttu-id="81d38-119">userDetails</span><span class="sxs-lookup"><span data-stu-id="81d38-119">userDetails</span></span> | <span data-ttu-id="81d38-120">设置将在控件上显示的 user 对象。</span><span class="sxs-lookup"><span data-stu-id="81d38-120">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="81d38-121">下面的示例设置人员的详细信息。</span><span class="sxs-lookup"><span data-stu-id="81d38-121">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    mail: 'nikola@contoso.com',
    personImage: 'url'
}
```

<span data-ttu-id="81d38-122">设置 `userDetails` 为 `null` 将转到 "已注销" 状态。</span><span class="sxs-lookup"><span data-stu-id="81d38-122">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="81d38-123">使用 `loginInitiated` 和 `logoutInitiated` 事件处理登录和注销。</span><span class="sxs-lookup"><span data-stu-id="81d38-123">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="81d38-124">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="81d38-124">CSS custom properties</span></span>

<span data-ttu-id="81d38-125">`mgt-login`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="81d38-125">The `mgt-login` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="81d38-126">若要了解详细信息，请参阅[样式组件](../style.md)。</span><span class="sxs-lookup"><span data-stu-id="81d38-126">To learn more, see [styling components](../style.md).</span></span>

## <a name="events"></a><span data-ttu-id="81d38-127">活动</span><span class="sxs-lookup"><span data-stu-id="81d38-127">Events</span></span>

<span data-ttu-id="81d38-128">从控件触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="81d38-128">The following events are fired from the control.</span></span>

| <span data-ttu-id="81d38-129">事件</span><span class="sxs-lookup"><span data-stu-id="81d38-129">Event</span></span> | <span data-ttu-id="81d38-130">说明</span><span class="sxs-lookup"><span data-stu-id="81d38-130">Description</span></span> |
| --- | --- |
| `loginInitiated` | <span data-ttu-id="81d38-131">用户单击了 "登录" 按钮以启动登录过程（可取消）。</span><span class="sxs-lookup"><span data-stu-id="81d38-131">The user clicked the sign in button to start the login process - cancelable.</span></span>|
| `loginCompleted` | <span data-ttu-id="81d38-132">登录过程成功，用户现在已登录。</span><span class="sxs-lookup"><span data-stu-id="81d38-132">the login process was successful and the user is now signed in.</span></span> |
| `loginFailed` | <span data-ttu-id="81d38-133">用户取消了登录进程或无法登录。</span><span class="sxs-lookup"><span data-stu-id="81d38-133">The user canceled the login process or was unable to sign in.</span></span>|
| `logoutInitiated` | <span data-ttu-id="81d38-134">用户已开始注销。</span><span class="sxs-lookup"><span data-stu-id="81d38-134">The user started to logout - cancelable.</span></span> |
| `logoutCompleted` | <span data-ttu-id="81d38-135">用户已注销。</span><span class="sxs-lookup"><span data-stu-id="81d38-135">The user signed out.</span></span> |

## <a name="templates"></a><span data-ttu-id="81d38-136">模板</span><span class="sxs-lookup"><span data-stu-id="81d38-136">Templates</span></span>

<span data-ttu-id="81d38-137">`mgt-login`组件支持多个[模板](../templates.md)，这些模板允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="81d38-137">The `mgt-login` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="81d38-138">若要指定模板，请在 `<template>` 组件内添加一个元素，并将 `data-type` 值设置为下表中列出的值之一。</span><span class="sxs-lookup"><span data-stu-id="81d38-138">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the values listed in the following table.</span></span> 

| <span data-ttu-id="81d38-139">数据类型</span><span class="sxs-lookup"><span data-stu-id="81d38-139">Data type</span></span> | <span data-ttu-id="81d38-140">数据上下文</span><span class="sxs-lookup"><span data-stu-id="81d38-140">Data context</span></span> | <span data-ttu-id="81d38-141">Description</span><span class="sxs-lookup"><span data-stu-id="81d38-141">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="81d38-142">登录按钮内容</span><span class="sxs-lookup"><span data-stu-id="81d38-142">signed-in-button-content</span></span> | <span data-ttu-id="81d38-143">personDetails： person 对象， `personImage` ：人员图像字符串</span><span class="sxs-lookup"><span data-stu-id="81d38-143">personDetails: person object, `personImage`: person image string</span></span> | <span data-ttu-id="81d38-144">用户登录时用于呈现按钮中的内容的模板。</span><span class="sxs-lookup"><span data-stu-id="81d38-144">The template used to render the content in the button when the user is signed in.</span></span> |
| <span data-ttu-id="81d38-145">签出按钮-内容</span><span class="sxs-lookup"><span data-stu-id="81d38-145">signed-out-button-content</span></span> | <span data-ttu-id="81d38-146">Null</span><span class="sxs-lookup"><span data-stu-id="81d38-146">null</span></span> | <span data-ttu-id="81d38-147">用户未登录时用于呈现按钮中的内容的模板。</span><span class="sxs-lookup"><span data-stu-id="81d38-147">The template used to render the content in the button when the user is not signed in.</span></span> |
| <span data-ttu-id="81d38-148">浮出控件-命令</span><span class="sxs-lookup"><span data-stu-id="81d38-148">flyout-commands</span></span> | <span data-ttu-id="81d38-149">handleSignOut：注销函数</span><span class="sxs-lookup"><span data-stu-id="81d38-149">handleSignOut: sign out function</span></span> | <span data-ttu-id="81d38-150">用于呈现浮出控件中的命令的模板</span><span class="sxs-lookup"><span data-stu-id="81d38-150">The template used to render the commands in the flyout</span></span> |
| <span data-ttu-id="81d38-151">飞出-人员-详细信息</span><span class="sxs-lookup"><span data-stu-id="81d38-151">flyout-person-details</span></span> | <span data-ttu-id="81d38-152">personDetails： person 对象，personImage： person image string</span><span class="sxs-lookup"><span data-stu-id="81d38-152">personDetails: person object, personImage: person image string</span></span> | <span data-ttu-id="81d38-153">用于在浮出控件中呈现人员详细信息的模板。</span><span class="sxs-lookup"><span data-stu-id="81d38-153">The template used to render the person details in the flyout.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="81d38-154">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="81d38-154">Microsoft Graph permissions</span></span>

<span data-ttu-id="81d38-155">此组件使用 "[人员" 组件](./person.md)显示用户并继承所有权限。</span><span class="sxs-lookup"><span data-stu-id="81d38-155">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="81d38-156">身份验证</span><span class="sxs-lookup"><span data-stu-id="81d38-156">Authentication</span></span>

<span data-ttu-id="81d38-157">登录控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="81d38-157">The login control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 

## <a name="extend-for-more-control"></a><span data-ttu-id="81d38-158">扩展以实现更多控制</span><span class="sxs-lookup"><span data-stu-id="81d38-158">Extend for more control</span></span>

<span data-ttu-id="81d38-159">对于更复杂的方案或真正的自定义 UX，此组件将公开几种 `protected render*` 用于在组件扩展中进行重写的方法。</span><span class="sxs-lookup"><span data-stu-id="81d38-159">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="81d38-160">方法</span><span class="sxs-lookup"><span data-stu-id="81d38-160">Method</span></span> | <span data-ttu-id="81d38-161">说明</span><span class="sxs-lookup"><span data-stu-id="81d38-161">Description</span></span> |
| - | - |
| <span data-ttu-id="81d38-162">renderButton</span><span class="sxs-lookup"><span data-stu-id="81d38-162">renderButton</span></span> | <span data-ttu-id="81d38-163">呈现按钮 chrome。</span><span class="sxs-lookup"><span data-stu-id="81d38-163">Renders the button chrome.</span></span> |
| <span data-ttu-id="81d38-164">renderButtonContent</span><span class="sxs-lookup"><span data-stu-id="81d38-164">renderButtonContent</span></span> | <span data-ttu-id="81d38-165">呈现按钮内容。</span><span class="sxs-lookup"><span data-stu-id="81d38-165">Renders the button content.</span></span> |
| <span data-ttu-id="81d38-166">renderSignedInButtonContent</span><span class="sxs-lookup"><span data-stu-id="81d38-166">renderSignedInButtonContent</span></span> | <span data-ttu-id="81d38-167">在用户登录时呈现按钮内容。</span><span class="sxs-lookup"><span data-stu-id="81d38-167">Render the button content when the user is signed in.</span></span> |
| <span data-ttu-id="81d38-168">renderSignedOutButtonContent</span><span class="sxs-lookup"><span data-stu-id="81d38-168">renderSignedOutButtonContent</span></span> | <span data-ttu-id="81d38-169">在用户未登录时呈现按钮内容。</span><span class="sxs-lookup"><span data-stu-id="81d38-169">Render the button content when the user is not signed in.</span></span> |
| <span data-ttu-id="81d38-170">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="81d38-170">renderFlyout</span></span> | <span data-ttu-id="81d38-171">呈现浮出控件的镶边。</span><span class="sxs-lookup"><span data-stu-id="81d38-171">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="81d38-172">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="81d38-172">renderFlyoutContent</span></span> | <span data-ttu-id="81d38-173">呈现浮出控件内容。</span><span class="sxs-lookup"><span data-stu-id="81d38-173">Renders the flyout content.</span></span> |
| <span data-ttu-id="81d38-174">renderFlyoutPersonDetails</span><span class="sxs-lookup"><span data-stu-id="81d38-174">renderFlyoutPersonDetails</span></span> | <span data-ttu-id="81d38-175">呈现飞出的人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="81d38-175">Render the flyout person details.</span></span> |
| <span data-ttu-id="81d38-176">renderFlyoutCommands</span><span class="sxs-lookup"><span data-stu-id="81d38-176">renderFlyoutCommands</span></span> | <span data-ttu-id="81d38-177">呈现浮出控件命令。</span><span class="sxs-lookup"><span data-stu-id="81d38-177">Render the flyout commands.</span></span> |

### <a name="bring-your-own-flyout"></a><span data-ttu-id="81d38-178">引入自己的浮出控件</span><span class="sxs-lookup"><span data-stu-id="81d38-178">Bring your own flyout</span></span>

<span data-ttu-id="81d38-179">可以通过重写 `renderFlyout()` 方法并提供新的浮出控件，使用您自己的飞出组件来替换内置的飞入组件。</span><span class="sxs-lookup"><span data-stu-id="81d38-179">It is possible to use your own flyout component in place of the built-in one, by overriding the `renderFlyout()` method and providing the new flyout.</span></span>

<span data-ttu-id="81d38-180">在这种情况下，请重写 `protected` 浮出控件的显示方法以更新您的替代浮出控件的可见性，以确保登录组件继续按预期方式工作。</span><span class="sxs-lookup"><span data-stu-id="81d38-180">In this case, ensure the login component continues to work as expected by overriding the `protected` flyout display methods to update the visibility of your alternative flyout.</span></span>

| <span data-ttu-id="81d38-181">方法</span><span class="sxs-lookup"><span data-stu-id="81d38-181">Method</span></span> | <span data-ttu-id="81d38-182">说明</span><span class="sxs-lookup"><span data-stu-id="81d38-182">Description</span></span> |
| - | - |
| <span data-ttu-id="81d38-183">hideFlyout</span><span class="sxs-lookup"><span data-stu-id="81d38-183">hideFlyout</span></span> | <span data-ttu-id="81d38-184">关闭浮出控件。</span><span class="sxs-lookup"><span data-stu-id="81d38-184">Dismisses the flyout.</span></span> |
| <span data-ttu-id="81d38-185">showFlyout</span><span class="sxs-lookup"><span data-stu-id="81d38-185">showFlyout</span></span> | <span data-ttu-id="81d38-186">显示浮出控件。</span><span class="sxs-lookup"><span data-stu-id="81d38-186">Displays the flyout.</span></span> |
| <span data-ttu-id="81d38-187">toggleFlyout</span><span class="sxs-lookup"><span data-stu-id="81d38-187">toggleFlyout</span></span> | <span data-ttu-id="81d38-188">切换浮出控件的状态。</span><span class="sxs-lookup"><span data-stu-id="81d38-188">Toggles the state of the flyout.</span></span> |
