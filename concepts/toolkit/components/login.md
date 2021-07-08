---
title: Microsoft 服务中的登录Graph Toolkit
description: 登录组件是一个按钮和飞出控件，用于简化Microsoft 标识平台身份验证。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 5dd610407fde25089a9c323b6b0cfb7965d33671
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334764"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="ee4a6-103">Microsoft 服务中的登录Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="ee4a6-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="ee4a6-104">登录组件是一个按钮和飞出控件，用于简化Microsoft 标识平台身份验证。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="ee4a6-105">它提供两种状态：</span><span class="sxs-lookup"><span data-stu-id="ee4a6-105">It provides two states:</span></span>
* <span data-ttu-id="ee4a6-106">当用户未登录时，控件是一个简单的按钮，用于启动登录过程。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="ee4a6-107">用户登录后，控件将显示当前登录的用户名、个人资料图像和电子邮件。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="ee4a6-108">单击后，将打开一个具有注销命令的飞出。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="ee4a6-109">示例</span><span class="sxs-lookup"><span data-stu-id="ee4a6-109">Example</span></span>

<span data-ttu-id="ee4a6-110">以下示例显示了 `mgt-login` 具有已登录用户的组件。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-110">The following example shows the `mgt-login` component with a signed-in user.</span></span> 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[<span data-ttu-id="ee4a6-111">在 mgt.dev 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="ee4a6-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="ee4a6-112">在没有身份验证提供程序的情况下使用控件</span><span class="sxs-lookup"><span data-stu-id="ee4a6-112">Using the control without an authentication provider</span></span>

<span data-ttu-id="ee4a6-113">该组件适用于提供程序和 Microsoft Graph开箱即用。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-113">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="ee4a6-114">但是，如果要提供自己的逻辑和身份验证，可以使用 属性设置 `userDetails` 登录用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-114">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="ee4a6-115">属性</span><span class="sxs-lookup"><span data-stu-id="ee4a6-115">Attribute</span></span> | <span data-ttu-id="ee4a6-116">属性</span><span class="sxs-lookup"><span data-stu-id="ee4a6-116">Property</span></span> | <span data-ttu-id="ee4a6-117">说明</span><span class="sxs-lookup"><span data-stu-id="ee4a6-117">Description</span></span> |
| --- | --- | -- |
| <span data-ttu-id="ee4a6-118">user-details</span><span class="sxs-lookup"><span data-stu-id="ee4a6-118">user-details</span></span> | <span data-ttu-id="ee4a6-119">userDetails</span><span class="sxs-lookup"><span data-stu-id="ee4a6-119">userDetails</span></span> | <span data-ttu-id="ee4a6-120">设置将在控件上显示的用户对象。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-120">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="ee4a6-121">以下示例设置人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-121">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    mail: 'nikola@contoso.com',
    personImage: 'url'
}
```

<span data-ttu-id="ee4a6-122">设置为 `userDetails` `null` 将转到已退出状态。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-122">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="ee4a6-123">使用 `loginInitiated` 和 `logoutInitiated` 事件处理登录和退出。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-123">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="ee4a6-124">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="ee4a6-124">CSS custom properties</span></span>

<span data-ttu-id="ee4a6-125">组件 `mgt-login` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-125">The `mgt-login` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="ee4a6-126">若要了解更多信息，请参阅 [设置组件样式](../customize-components/style.md)。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-126">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="ee4a6-127">活动</span><span class="sxs-lookup"><span data-stu-id="ee4a6-127">Events</span></span>

<span data-ttu-id="ee4a6-128">从控件中触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-128">The following events are fired from the control.</span></span>

<span data-ttu-id="ee4a6-129">事件</span><span class="sxs-lookup"><span data-stu-id="ee4a6-129">Event</span></span> | <span data-ttu-id="ee4a6-130">何时发出</span><span class="sxs-lookup"><span data-stu-id="ee4a6-130">When is it emitted</span></span> | <span data-ttu-id="ee4a6-131">自定义数据</span><span class="sxs-lookup"><span data-stu-id="ee4a6-131">Custom data</span></span> | <span data-ttu-id="ee4a6-132">Cancelable</span><span class="sxs-lookup"><span data-stu-id="ee4a6-132">Cancelable</span></span> | <span data-ttu-id="ee4a6-133">气泡</span><span class="sxs-lookup"><span data-stu-id="ee4a6-133">Bubbles</span></span> | <span data-ttu-id="ee4a6-134">使用自定义模板</span><span class="sxs-lookup"><span data-stu-id="ee4a6-134">Works with custom template</span></span>
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`loginInitiated` | <span data-ttu-id="ee4a6-135">用户单击登录按钮以启动登录过程</span><span class="sxs-lookup"><span data-stu-id="ee4a6-135">The user clicked the sign in button to start the login process</span></span> | <span data-ttu-id="ee4a6-136">无</span><span class="sxs-lookup"><span data-stu-id="ee4a6-136">None</span></span> | <span data-ttu-id="ee4a6-137">是</span><span class="sxs-lookup"><span data-stu-id="ee4a6-137">Yes</span></span> | <span data-ttu-id="ee4a6-138">否</span><span class="sxs-lookup"><span data-stu-id="ee4a6-138">No</span></span> | <span data-ttu-id="ee4a6-139">是</span><span class="sxs-lookup"><span data-stu-id="ee4a6-139">Yes</span></span>
`loginCompleted` | <span data-ttu-id="ee4a6-140">登录过程成功，用户现在已登录</span><span class="sxs-lookup"><span data-stu-id="ee4a6-140">The login process was successful and the user is now signed in</span></span> | <span data-ttu-id="ee4a6-141">无</span><span class="sxs-lookup"><span data-stu-id="ee4a6-141">None</span></span> | <span data-ttu-id="ee4a6-142">否</span><span class="sxs-lookup"><span data-stu-id="ee4a6-142">No</span></span> | <span data-ttu-id="ee4a6-143">否</span><span class="sxs-lookup"><span data-stu-id="ee4a6-143">No</span></span> | <span data-ttu-id="ee4a6-144">是</span><span class="sxs-lookup"><span data-stu-id="ee4a6-144">Yes</span></span>
`loginFailed` | <span data-ttu-id="ee4a6-145">用户已取消登录过程或无法登录</span><span class="sxs-lookup"><span data-stu-id="ee4a6-145">The user canceled the login process or was unable to sign in</span></span> | <span data-ttu-id="ee4a6-146">无</span><span class="sxs-lookup"><span data-stu-id="ee4a6-146">None</span></span> | <span data-ttu-id="ee4a6-147">否</span><span class="sxs-lookup"><span data-stu-id="ee4a6-147">No</span></span> | <span data-ttu-id="ee4a6-148">否</span><span class="sxs-lookup"><span data-stu-id="ee4a6-148">No</span></span> | <span data-ttu-id="ee4a6-149">是</span><span class="sxs-lookup"><span data-stu-id="ee4a6-149">Yes</span></span>
`logoutInitiated` | <span data-ttu-id="ee4a6-150">用户开始注销</span><span class="sxs-lookup"><span data-stu-id="ee4a6-150">The user started to logout</span></span> | <span data-ttu-id="ee4a6-151">无</span><span class="sxs-lookup"><span data-stu-id="ee4a6-151">None</span></span> | <span data-ttu-id="ee4a6-152">是</span><span class="sxs-lookup"><span data-stu-id="ee4a6-152">Yes</span></span> | <span data-ttu-id="ee4a6-153">否</span><span class="sxs-lookup"><span data-stu-id="ee4a6-153">No</span></span> | <span data-ttu-id="ee4a6-154">是</span><span class="sxs-lookup"><span data-stu-id="ee4a6-154">Yes</span></span>
`logoutCompleted` | <span data-ttu-id="ee4a6-155">用户已登录</span><span class="sxs-lookup"><span data-stu-id="ee4a6-155">The user signed out</span></span> | <span data-ttu-id="ee4a6-156">无</span><span class="sxs-lookup"><span data-stu-id="ee4a6-156">None</span></span> | <span data-ttu-id="ee4a6-157">否</span><span class="sxs-lookup"><span data-stu-id="ee4a6-157">No</span></span> | <span data-ttu-id="ee4a6-158">否</span><span class="sxs-lookup"><span data-stu-id="ee4a6-158">No</span></span> | <span data-ttu-id="ee4a6-159">是</span><span class="sxs-lookup"><span data-stu-id="ee4a6-159">Yes</span></span>

<span data-ttu-id="ee4a6-160">有关处理事件的信息，请参阅 [事件](../customize-components/events.md)。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-160">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="templates"></a><span data-ttu-id="ee4a6-161">模板</span><span class="sxs-lookup"><span data-stu-id="ee4a6-161">Templates</span></span>

<span data-ttu-id="ee4a6-162">组件 `mgt-login` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-162">The `mgt-login` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="ee4a6-163">若要指定模板，请包含组件内的元素，将值设置为下表 `<template>` `data-type` 中列出的值之一。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-163">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the values listed in the following table.</span></span> 

| <span data-ttu-id="ee4a6-164">数据类型</span><span class="sxs-lookup"><span data-stu-id="ee4a6-164">Data type</span></span> | <span data-ttu-id="ee4a6-165">数据上下文</span><span class="sxs-lookup"><span data-stu-id="ee4a6-165">Data context</span></span> | <span data-ttu-id="ee4a6-166">说明</span><span class="sxs-lookup"><span data-stu-id="ee4a6-166">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="ee4a6-167">signed-in-button-content</span><span class="sxs-lookup"><span data-stu-id="ee4a6-167">signed-in-button-content</span></span> | <span data-ttu-id="ee4a6-168">personDetails： person object， `personImage` ： person image string</span><span class="sxs-lookup"><span data-stu-id="ee4a6-168">personDetails: person object, `personImage`: person image string</span></span> | <span data-ttu-id="ee4a6-169">用于当用户登录时在按钮中呈现内容的模板。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-169">The template used to render the content in the button when the user is signed in.</span></span> |
| <span data-ttu-id="ee4a6-170">signed-out-button-content</span><span class="sxs-lookup"><span data-stu-id="ee4a6-170">signed-out-button-content</span></span> | <span data-ttu-id="ee4a6-171">空</span><span class="sxs-lookup"><span data-stu-id="ee4a6-171">null</span></span> | <span data-ttu-id="ee4a6-172">用于当用户未登录时在按钮中呈现内容的模板。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-172">The template used to render the content in the button when the user is not signed in.</span></span> |
| <span data-ttu-id="ee4a6-173">flyout-commands</span><span class="sxs-lookup"><span data-stu-id="ee4a6-173">flyout-commands</span></span> | <span data-ttu-id="ee4a6-174">handleSignOut：注销函数</span><span class="sxs-lookup"><span data-stu-id="ee4a6-174">handleSignOut: sign out function</span></span> | <span data-ttu-id="ee4a6-175">用于在飞出控件中呈现命令的模板</span><span class="sxs-lookup"><span data-stu-id="ee4a6-175">The template used to render the commands in the flyout</span></span> |
| <span data-ttu-id="ee4a6-176">flyout-person-details</span><span class="sxs-lookup"><span data-stu-id="ee4a6-176">flyout-person-details</span></span> | <span data-ttu-id="ee4a6-177">personDetails： person object， personImage： person image string</span><span class="sxs-lookup"><span data-stu-id="ee4a6-177">personDetails: person object, personImage: person image string</span></span> | <span data-ttu-id="ee4a6-178">用于在飞出控件中呈现人员详细信息的模板。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-178">The template used to render the person details in the flyout.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="ee4a6-179">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="ee4a6-179">Microsoft Graph permissions</span></span>

<span data-ttu-id="ee4a6-180">此组件使用以下 Microsoft Graph API 和权限：</span><span class="sxs-lookup"><span data-stu-id="ee4a6-180">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="ee4a6-181">配置</span><span class="sxs-lookup"><span data-stu-id="ee4a6-181">Configuration</span></span> | <span data-ttu-id="ee4a6-182">权限</span><span class="sxs-lookup"><span data-stu-id="ee4a6-182">Permission</span></span> | <span data-ttu-id="ee4a6-183">API</span><span class="sxs-lookup"><span data-stu-id="ee4a6-183">API</span></span>
| - | - | - |
| <span data-ttu-id="ee4a6-184">default</span><span class="sxs-lookup"><span data-stu-id="ee4a6-184">default</span></span> | <span data-ttu-id="ee4a6-185">User.Read</span><span class="sxs-lookup"><span data-stu-id="ee4a6-185">User.Read</span></span> | [<span data-ttu-id="ee4a6-186">/users/me/</span><span class="sxs-lookup"><span data-stu-id="ee4a6-186">/users/me/</span></span>](/graph/api/user-get) |

<span data-ttu-id="ee4a6-187">使用默认 `signed-in-button-content` 和 `flyout-person-details` 模板时，此组件使用 [Person](./person.md) 组件显示用户并继承所有权限。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-187">When using the default `signed-in-button-content` and `flyout-person-details` templates, this component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span>

## <a name="authentication"></a><span data-ttu-id="ee4a6-188">身份验证</span><span class="sxs-lookup"><span data-stu-id="ee4a6-188">Authentication</span></span>

<span data-ttu-id="ee4a6-189">登录控件使用身份验证文档 中所述的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-189">The login control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span> 

## <a name="cache"></a><span data-ttu-id="ee4a6-190">缓存</span><span class="sxs-lookup"><span data-stu-id="ee4a6-190">Cache</span></span>

<span data-ttu-id="ee4a6-191">此组件使用 [Person 组件](./person.md) 显示用户，并继承该用户的所有缓存配置。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-191">This component uses the [Person component](./person.md) to display the user and inherits all cache configuration from it.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="ee4a6-192">扩展以了解更多控件</span><span class="sxs-lookup"><span data-stu-id="ee4a6-192">Extend for more control</span></span>

<span data-ttu-id="ee4a6-193">对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展 `protected render*` 中替代的方法。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-193">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="ee4a6-194">方法</span><span class="sxs-lookup"><span data-stu-id="ee4a6-194">Method</span></span> | <span data-ttu-id="ee4a6-195">说明</span><span class="sxs-lookup"><span data-stu-id="ee4a6-195">Description</span></span> |
| - | - |
| <span data-ttu-id="ee4a6-196">renderButton</span><span class="sxs-lookup"><span data-stu-id="ee4a6-196">renderButton</span></span> | <span data-ttu-id="ee4a6-197">呈现按钮部件版式。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-197">Renders the button chrome.</span></span> |
| <span data-ttu-id="ee4a6-198">renderButtonContent</span><span class="sxs-lookup"><span data-stu-id="ee4a6-198">renderButtonContent</span></span> | <span data-ttu-id="ee4a6-199">呈现按钮内容。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-199">Renders the button content.</span></span> |
| <span data-ttu-id="ee4a6-200">renderSignedInButtonContent</span><span class="sxs-lookup"><span data-stu-id="ee4a6-200">renderSignedInButtonContent</span></span> | <span data-ttu-id="ee4a6-201">当用户登录时呈现按钮内容。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-201">Render the button content when the user is signed in.</span></span> |
| <span data-ttu-id="ee4a6-202">renderSignedOutButtonContent</span><span class="sxs-lookup"><span data-stu-id="ee4a6-202">renderSignedOutButtonContent</span></span> | <span data-ttu-id="ee4a6-203">当用户未登录时呈现按钮内容。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-203">Render the button content when the user is not signed in.</span></span> |
| <span data-ttu-id="ee4a6-204">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="ee4a6-204">renderFlyout</span></span> | <span data-ttu-id="ee4a6-205">呈现飞出部件版式。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-205">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="ee4a6-206">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="ee4a6-206">renderFlyoutContent</span></span> | <span data-ttu-id="ee4a6-207">呈现飞出内容。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-207">Renders the flyout content.</span></span> |
| <span data-ttu-id="ee4a6-208">renderFlyoutPersonDetails</span><span class="sxs-lookup"><span data-stu-id="ee4a6-208">renderFlyoutPersonDetails</span></span> | <span data-ttu-id="ee4a6-209">呈现飞出人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-209">Render the flyout person details.</span></span> |
| <span data-ttu-id="ee4a6-210">renderFlyoutCommands</span><span class="sxs-lookup"><span data-stu-id="ee4a6-210">renderFlyoutCommands</span></span> | <span data-ttu-id="ee4a6-211">呈现飞出命令。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-211">Render the flyout commands.</span></span> |

### <a name="bring-your-own-flyout"></a><span data-ttu-id="ee4a6-212">自带飞出</span><span class="sxs-lookup"><span data-stu-id="ee4a6-212">Bring your own flyout</span></span>

<span data-ttu-id="ee4a6-213">通过替代 方法并提供新的飞出，可以使用自己的飞出组件来替代内置 `renderFlyout()` 组件。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-213">It is possible to use your own flyout component in place of the built-in one, by overriding the `renderFlyout()` method and providing the new flyout.</span></span>

<span data-ttu-id="ee4a6-214">在这种情况下，通过覆盖飞出显示方法以更新备用飞出视图的可见性，确保登录组件继续按预期 `protected` 工作。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-214">In this case, ensure the login component continues to work as expected by overriding the `protected` flyout display methods to update the visibility of your alternative flyout.</span></span>

| <span data-ttu-id="ee4a6-215">方法</span><span class="sxs-lookup"><span data-stu-id="ee4a6-215">Method</span></span> | <span data-ttu-id="ee4a6-216">说明</span><span class="sxs-lookup"><span data-stu-id="ee4a6-216">Description</span></span> |
| - | - |
| <span data-ttu-id="ee4a6-217">hideFlyout</span><span class="sxs-lookup"><span data-stu-id="ee4a6-217">hideFlyout</span></span> | <span data-ttu-id="ee4a6-218">消除该飞出区。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-218">Dismisses the flyout.</span></span> |
| <span data-ttu-id="ee4a6-219">showFlyout</span><span class="sxs-lookup"><span data-stu-id="ee4a6-219">showFlyout</span></span> | <span data-ttu-id="ee4a6-220">显示飞出。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-220">Displays the flyout.</span></span> |
| <span data-ttu-id="ee4a6-221">toggleFlyout</span><span class="sxs-lookup"><span data-stu-id="ee4a6-221">toggleFlyout</span></span> | <span data-ttu-id="ee4a6-222">切换飞出状态。</span><span class="sxs-lookup"><span data-stu-id="ee4a6-222">Toggles the state of the flyout.</span></span> |
