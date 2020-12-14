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
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="dc5fd-103">Login component in the Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="dc5fd-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="dc5fd-104">登录组件是一个按钮和飞出控件，用于简化 Microsoft 标识平台身份验证。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="dc5fd-105">它提供两种状态：</span><span class="sxs-lookup"><span data-stu-id="dc5fd-105">It provides two states:</span></span>
* <span data-ttu-id="dc5fd-106">当用户未登录时，控件是启动登录过程的一个简单按钮。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="dc5fd-107">用户登录后，控件将显示当前登录的用户名、个人资料图像和电子邮件。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="dc5fd-108">单击后，将打开一个显示注销命令的飞出。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="dc5fd-109">示例</span><span class="sxs-lookup"><span data-stu-id="dc5fd-109">Example</span></span>

<span data-ttu-id="dc5fd-110">以下示例显示了 `mgt-login` 具有已登录用户的组件。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-110">The following example shows the `mgt-login` component with a signed-in user.</span></span> 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[<span data-ttu-id="dc5fd-111">在 mgt.dev 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="dc5fd-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="dc5fd-112">在没有身份验证提供程序的情况下使用控件</span><span class="sxs-lookup"><span data-stu-id="dc5fd-112">Using the control without an authentication provider</span></span>

<span data-ttu-id="dc5fd-113">该组件适用于提供程序和开箱即用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-113">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="dc5fd-114">但是，如果要提供自己的逻辑和身份验证，可以使用该属性设置 `userDetails` 登录用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-114">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="dc5fd-115">属性</span><span class="sxs-lookup"><span data-stu-id="dc5fd-115">Attribute</span></span> | <span data-ttu-id="dc5fd-116">属性</span><span class="sxs-lookup"><span data-stu-id="dc5fd-116">Property</span></span> | <span data-ttu-id="dc5fd-117">说明</span><span class="sxs-lookup"><span data-stu-id="dc5fd-117">Description</span></span> |
| --- | --- | -- |
| <span data-ttu-id="dc5fd-118">user-details</span><span class="sxs-lookup"><span data-stu-id="dc5fd-118">user-details</span></span> | <span data-ttu-id="dc5fd-119">userDetails</span><span class="sxs-lookup"><span data-stu-id="dc5fd-119">userDetails</span></span> | <span data-ttu-id="dc5fd-120">设置将在控件上显示的用户对象。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-120">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="dc5fd-121">以下示例设置人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-121">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    mail: 'nikola@contoso.com',
    personImage: 'url'
}
```

<span data-ttu-id="dc5fd-122">设置为 `userDetails` `null` 将转到已签名状态。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-122">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="dc5fd-123">使用 `loginInitiated` and `logoutInitiated` 事件处理登录和退出。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-123">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="dc5fd-124">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="dc5fd-124">CSS custom properties</span></span>

<span data-ttu-id="dc5fd-125">该 `mgt-login` 组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-125">The `mgt-login` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="dc5fd-126">若要了解更多信息，请参阅 [样式组件](../customize-components/style.md)。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-126">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="dc5fd-127">活动</span><span class="sxs-lookup"><span data-stu-id="dc5fd-127">Events</span></span>

<span data-ttu-id="dc5fd-128">从控件中触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-128">The following events are fired from the control.</span></span>

| <span data-ttu-id="dc5fd-129">事件</span><span class="sxs-lookup"><span data-stu-id="dc5fd-129">Event</span></span> | <span data-ttu-id="dc5fd-130">说明</span><span class="sxs-lookup"><span data-stu-id="dc5fd-130">Description</span></span> |
| --- | --- |
| `loginInitiated` | <span data-ttu-id="dc5fd-131">用户单击登录按钮以启动登录过程 - 可取消。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-131">The user clicked the sign in button to start the login process - cancelable.</span></span>|
| `loginCompleted` | <span data-ttu-id="dc5fd-132">登录过程成功，用户现在已登录。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-132">the login process was successful and the user is now signed in.</span></span> |
| `loginFailed` | <span data-ttu-id="dc5fd-133">用户已取消登录过程或无法登录。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-133">The user canceled the login process or was unable to sign in.</span></span>|
| `logoutInitiated` | <span data-ttu-id="dc5fd-134">用户开始注销 - 可取消。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-134">The user started to logout - cancelable.</span></span> |
| `logoutCompleted` | <span data-ttu-id="dc5fd-135">用户已登录。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-135">The user signed out.</span></span> |

## <a name="templates"></a><span data-ttu-id="dc5fd-136">模板</span><span class="sxs-lookup"><span data-stu-id="dc5fd-136">Templates</span></span>

<span data-ttu-id="dc5fd-137">该 `mgt-login` 组件支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-137">The `mgt-login` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="dc5fd-138">若要指定模板，请包含组件中的元素，将值设置为下表 `<template>` `data-type` 中列出的值之一。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-138">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the values listed in the following table.</span></span> 

| <span data-ttu-id="dc5fd-139">数据类型</span><span class="sxs-lookup"><span data-stu-id="dc5fd-139">Data type</span></span> | <span data-ttu-id="dc5fd-140">数据上下文</span><span class="sxs-lookup"><span data-stu-id="dc5fd-140">Data context</span></span> | <span data-ttu-id="dc5fd-141">说明</span><span class="sxs-lookup"><span data-stu-id="dc5fd-141">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="dc5fd-142">登录按钮内容</span><span class="sxs-lookup"><span data-stu-id="dc5fd-142">signed-in-button-content</span></span> | <span data-ttu-id="dc5fd-143">personDetails： person 对象， `personImage` ： person 图像字符串</span><span class="sxs-lookup"><span data-stu-id="dc5fd-143">personDetails: person object, `personImage`: person image string</span></span> | <span data-ttu-id="dc5fd-144">用于在用户登录时呈现按钮中内容的模板。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-144">The template used to render the content in the button when the user is signed in.</span></span> |
| <span data-ttu-id="dc5fd-145">signed-out-button-content</span><span class="sxs-lookup"><span data-stu-id="dc5fd-145">signed-out-button-content</span></span> | <span data-ttu-id="dc5fd-146">空</span><span class="sxs-lookup"><span data-stu-id="dc5fd-146">null</span></span> | <span data-ttu-id="dc5fd-147">用于在用户未登录时呈现按钮中内容的模板。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-147">The template used to render the content in the button when the user is not signed in.</span></span> |
| <span data-ttu-id="dc5fd-148">flyout-commands</span><span class="sxs-lookup"><span data-stu-id="dc5fd-148">flyout-commands</span></span> | <span data-ttu-id="dc5fd-149">handleSignOut：注销函数</span><span class="sxs-lookup"><span data-stu-id="dc5fd-149">handleSignOut: sign out function</span></span> | <span data-ttu-id="dc5fd-150">用于在飞出控件中呈现命令的模板</span><span class="sxs-lookup"><span data-stu-id="dc5fd-150">The template used to render the commands in the flyout</span></span> |
| <span data-ttu-id="dc5fd-151">flyout-person-details</span><span class="sxs-lookup"><span data-stu-id="dc5fd-151">flyout-person-details</span></span> | <span data-ttu-id="dc5fd-152">personDetails： person object， personImage： person image string</span><span class="sxs-lookup"><span data-stu-id="dc5fd-152">personDetails: person object, personImage: person image string</span></span> | <span data-ttu-id="dc5fd-153">用于在飞出控件中呈现人员详细信息的模板。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-153">The template used to render the person details in the flyout.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="dc5fd-154">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="dc5fd-154">Microsoft Graph permissions</span></span>

<span data-ttu-id="dc5fd-155">此组件使用 [Person 组件](./person.md) 显示用户并继承所有权限。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-155">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="dc5fd-156">身份验证</span><span class="sxs-lookup"><span data-stu-id="dc5fd-156">Authentication</span></span>

<span data-ttu-id="dc5fd-157">登录控件使用身份验证文档中介绍的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-157">The login control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span> 

## <a name="extend-for-more-control"></a><span data-ttu-id="dc5fd-158">扩展以更多控制</span><span class="sxs-lookup"><span data-stu-id="dc5fd-158">Extend for more control</span></span>

<span data-ttu-id="dc5fd-159">对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展中 `protected render*` 替代的方法。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-159">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="dc5fd-160">方法</span><span class="sxs-lookup"><span data-stu-id="dc5fd-160">Method</span></span> | <span data-ttu-id="dc5fd-161">说明</span><span class="sxs-lookup"><span data-stu-id="dc5fd-161">Description</span></span> |
| - | - |
| <span data-ttu-id="dc5fd-162">renderButton</span><span class="sxs-lookup"><span data-stu-id="dc5fd-162">renderButton</span></span> | <span data-ttu-id="dc5fd-163">呈现按钮部件版式。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-163">Renders the button chrome.</span></span> |
| <span data-ttu-id="dc5fd-164">renderButtonContent</span><span class="sxs-lookup"><span data-stu-id="dc5fd-164">renderButtonContent</span></span> | <span data-ttu-id="dc5fd-165">呈现按钮内容。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-165">Renders the button content.</span></span> |
| <span data-ttu-id="dc5fd-166">renderSignedInButtonContent</span><span class="sxs-lookup"><span data-stu-id="dc5fd-166">renderSignedInButtonContent</span></span> | <span data-ttu-id="dc5fd-167">在用户登录时呈现按钮内容。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-167">Render the button content when the user is signed in.</span></span> |
| <span data-ttu-id="dc5fd-168">renderSignedOutButtonContent</span><span class="sxs-lookup"><span data-stu-id="dc5fd-168">renderSignedOutButtonContent</span></span> | <span data-ttu-id="dc5fd-169">当用户未登录时呈现按钮内容。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-169">Render the button content when the user is not signed in.</span></span> |
| <span data-ttu-id="dc5fd-170">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="dc5fd-170">renderFlyout</span></span> | <span data-ttu-id="dc5fd-171">呈现飞出部件版式。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-171">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="dc5fd-172">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="dc5fd-172">renderFlyoutContent</span></span> | <span data-ttu-id="dc5fd-173">呈现飞出内容。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-173">Renders the flyout content.</span></span> |
| <span data-ttu-id="dc5fd-174">renderFlyoutPersonDetails</span><span class="sxs-lookup"><span data-stu-id="dc5fd-174">renderFlyoutPersonDetails</span></span> | <span data-ttu-id="dc5fd-175">呈现飞出人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-175">Render the flyout person details.</span></span> |
| <span data-ttu-id="dc5fd-176">renderFlyoutCommands</span><span class="sxs-lookup"><span data-stu-id="dc5fd-176">renderFlyoutCommands</span></span> | <span data-ttu-id="dc5fd-177">呈现飞出命令。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-177">Render the flyout commands.</span></span> |

### <a name="bring-your-own-flyout"></a><span data-ttu-id="dc5fd-178">自带飞出</span><span class="sxs-lookup"><span data-stu-id="dc5fd-178">Bring your own flyout</span></span>

<span data-ttu-id="dc5fd-179">通过替代方法并提供新的飞出，可以使用你自己的飞出组件来替代内置 `renderFlyout()` 组件。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-179">It is possible to use your own flyout component in place of the built-in one, by overriding the `renderFlyout()` method and providing the new flyout.</span></span>

<span data-ttu-id="dc5fd-180">在这种情况下，通过替代飞出显示方法更新备用飞出视图的可见性，确保登录组件继续按预期 `protected` 工作。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-180">In this case, ensure the login component continues to work as expected by overriding the `protected` flyout display methods to update the visibility of your alternative flyout.</span></span>

| <span data-ttu-id="dc5fd-181">方法</span><span class="sxs-lookup"><span data-stu-id="dc5fd-181">Method</span></span> | <span data-ttu-id="dc5fd-182">说明</span><span class="sxs-lookup"><span data-stu-id="dc5fd-182">Description</span></span> |
| - | - |
| <span data-ttu-id="dc5fd-183">hideFlyout</span><span class="sxs-lookup"><span data-stu-id="dc5fd-183">hideFlyout</span></span> | <span data-ttu-id="dc5fd-184">消除该飞出。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-184">Dismisses the flyout.</span></span> |
| <span data-ttu-id="dc5fd-185">showFlyout</span><span class="sxs-lookup"><span data-stu-id="dc5fd-185">showFlyout</span></span> | <span data-ttu-id="dc5fd-186">显示飞出。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-186">Displays the flyout.</span></span> |
| <span data-ttu-id="dc5fd-187">toggleFlyout</span><span class="sxs-lookup"><span data-stu-id="dc5fd-187">toggleFlyout</span></span> | <span data-ttu-id="dc5fd-188">切换飞出状态。</span><span class="sxs-lookup"><span data-stu-id="dc5fd-188">Toggles the state of the flyout.</span></span> |
