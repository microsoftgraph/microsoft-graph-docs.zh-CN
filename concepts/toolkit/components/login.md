---
title: Login component in the Microsoft Graph Toolkit
description: 登录组件是一个按钮和飞出控件，用于简化 Microsoft 标识平台身份验证。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 3e9fc0f7960f9bd0fedb699595675479c3be0699
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266601"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="8cd7e-103">Login component in the Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="8cd7e-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="8cd7e-104">登录组件是一个按钮和飞出控件，用于简化 Microsoft 标识平台身份验证。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="8cd7e-105">它提供两种状态：</span><span class="sxs-lookup"><span data-stu-id="8cd7e-105">It provides two states:</span></span>
* <span data-ttu-id="8cd7e-106">当用户未登录时，控件是一个简单的按钮，用于启动登录过程。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="8cd7e-107">用户登录后，控件将显示当前登录的用户名、个人资料图像和电子邮件。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="8cd7e-108">单击后，将打开一个具有注销命令的飞出。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="8cd7e-109">示例</span><span class="sxs-lookup"><span data-stu-id="8cd7e-109">Example</span></span>

<span data-ttu-id="8cd7e-110">以下示例显示了 `mgt-login` 具有已登录用户的组件。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-110">The following example shows the `mgt-login` component with a signed-in user.</span></span> 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[<span data-ttu-id="8cd7e-111">在"打开"mgt.dev</span><span class="sxs-lookup"><span data-stu-id="8cd7e-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="8cd7e-112">在没有身份验证提供程序的情况下使用控件</span><span class="sxs-lookup"><span data-stu-id="8cd7e-112">Using the control without an authentication provider</span></span>

<span data-ttu-id="8cd7e-113">该组件适用于提供程序和开箱即用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-113">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="8cd7e-114">但是，如果要提供自己的逻辑和身份验证，可以使用 属性设置 `userDetails` 登录用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-114">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="8cd7e-115">属性</span><span class="sxs-lookup"><span data-stu-id="8cd7e-115">Attribute</span></span> | <span data-ttu-id="8cd7e-116">属性</span><span class="sxs-lookup"><span data-stu-id="8cd7e-116">Property</span></span> | <span data-ttu-id="8cd7e-117">说明</span><span class="sxs-lookup"><span data-stu-id="8cd7e-117">Description</span></span> |
| --- | --- | -- |
| <span data-ttu-id="8cd7e-118">user-details</span><span class="sxs-lookup"><span data-stu-id="8cd7e-118">user-details</span></span> | <span data-ttu-id="8cd7e-119">userDetails</span><span class="sxs-lookup"><span data-stu-id="8cd7e-119">userDetails</span></span> | <span data-ttu-id="8cd7e-120">设置将在控件上显示的用户对象。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-120">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="8cd7e-121">以下示例设置人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-121">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    mail: 'nikola@contoso.com',
    personImage: 'url'
}
```

<span data-ttu-id="8cd7e-122">设置为 `userDetails` `null` 将转到已退出状态。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-122">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="8cd7e-123">使用 `loginInitiated` 和 `logoutInitiated` 事件处理登录和退出。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-123">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="8cd7e-124">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="8cd7e-124">CSS custom properties</span></span>

<span data-ttu-id="8cd7e-125">组件 `mgt-login` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-125">The `mgt-login` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="8cd7e-126">若要了解更多信息，请参阅 [设置组件样式](../customize-components/style.md)。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-126">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="8cd7e-127">事件</span><span class="sxs-lookup"><span data-stu-id="8cd7e-127">Events</span></span>

<span data-ttu-id="8cd7e-128">从控件中触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-128">The following events are fired from the control.</span></span>

| <span data-ttu-id="8cd7e-129">事件</span><span class="sxs-lookup"><span data-stu-id="8cd7e-129">Event</span></span> | <span data-ttu-id="8cd7e-130">说明</span><span class="sxs-lookup"><span data-stu-id="8cd7e-130">Description</span></span> |
| --- | --- |
| `loginInitiated` | <span data-ttu-id="8cd7e-131">用户单击登录按钮以启动登录过程 - 可取消。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-131">The user clicked the sign in button to start the login process - cancelable.</span></span>|
| `loginCompleted` | <span data-ttu-id="8cd7e-132">登录过程成功，用户现已登录。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-132">the login process was successful and the user is now signed in.</span></span> |
| `loginFailed` | <span data-ttu-id="8cd7e-133">用户已取消登录过程或无法登录。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-133">The user canceled the login process or was unable to sign in.</span></span>|
| `logoutInitiated` | <span data-ttu-id="8cd7e-134">用户开始注销 - 可取消。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-134">The user started to logout - cancelable.</span></span> |
| `logoutCompleted` | <span data-ttu-id="8cd7e-135">用户已退出。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-135">The user signed out.</span></span> |

## <a name="templates"></a><span data-ttu-id="8cd7e-136">模板</span><span class="sxs-lookup"><span data-stu-id="8cd7e-136">Templates</span></span>

<span data-ttu-id="8cd7e-137">组件 `mgt-login` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-137">The `mgt-login` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="8cd7e-138">若要指定模板，请包含组件内的元素，将值设置为下表 `<template>` `data-type` 中列出的值之一。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-138">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the values listed in the following table.</span></span> 

| <span data-ttu-id="8cd7e-139">数据类型</span><span class="sxs-lookup"><span data-stu-id="8cd7e-139">Data type</span></span> | <span data-ttu-id="8cd7e-140">数据上下文</span><span class="sxs-lookup"><span data-stu-id="8cd7e-140">Data context</span></span> | <span data-ttu-id="8cd7e-141">说明</span><span class="sxs-lookup"><span data-stu-id="8cd7e-141">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="8cd7e-142">signed-in-button-content</span><span class="sxs-lookup"><span data-stu-id="8cd7e-142">signed-in-button-content</span></span> | <span data-ttu-id="8cd7e-143">personDetails： person object， `personImage` ： person image string</span><span class="sxs-lookup"><span data-stu-id="8cd7e-143">personDetails: person object, `personImage`: person image string</span></span> | <span data-ttu-id="8cd7e-144">用于当用户登录时在按钮中呈现内容的模板。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-144">The template used to render the content in the button when the user is signed in.</span></span> |
| <span data-ttu-id="8cd7e-145">signed-out-button-content</span><span class="sxs-lookup"><span data-stu-id="8cd7e-145">signed-out-button-content</span></span> | <span data-ttu-id="8cd7e-146">空</span><span class="sxs-lookup"><span data-stu-id="8cd7e-146">null</span></span> | <span data-ttu-id="8cd7e-147">用于当用户未登录时在按钮中呈现内容的模板。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-147">The template used to render the content in the button when the user is not signed in.</span></span> |
| <span data-ttu-id="8cd7e-148">flyout-commands</span><span class="sxs-lookup"><span data-stu-id="8cd7e-148">flyout-commands</span></span> | <span data-ttu-id="8cd7e-149">handleSignOut：注销函数</span><span class="sxs-lookup"><span data-stu-id="8cd7e-149">handleSignOut: sign out function</span></span> | <span data-ttu-id="8cd7e-150">用于在飞出控件中呈现命令的模板</span><span class="sxs-lookup"><span data-stu-id="8cd7e-150">The template used to render the commands in the flyout</span></span> |
| <span data-ttu-id="8cd7e-151">flyout-person-details</span><span class="sxs-lookup"><span data-stu-id="8cd7e-151">flyout-person-details</span></span> | <span data-ttu-id="8cd7e-152">personDetails： person object， personImage： person image string</span><span class="sxs-lookup"><span data-stu-id="8cd7e-152">personDetails: person object, personImage: person image string</span></span> | <span data-ttu-id="8cd7e-153">用于在飞出控件中呈现人员详细信息的模板。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-153">The template used to render the person details in the flyout.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="8cd7e-154">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="8cd7e-154">Microsoft Graph permissions</span></span>

<span data-ttu-id="8cd7e-155">此组件使用 [Person 组件](./person.md) 显示用户并继承所有权限。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-155">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="8cd7e-156">身份验证</span><span class="sxs-lookup"><span data-stu-id="8cd7e-156">Authentication</span></span>

<span data-ttu-id="8cd7e-157">登录控件使用身份验证文档 中所述的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-157">The login control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span> 

## <a name="cache"></a><span data-ttu-id="8cd7e-158">缓存</span><span class="sxs-lookup"><span data-stu-id="8cd7e-158">Cache</span></span>

<span data-ttu-id="8cd7e-159">此组件使用 [Person 组件](./person.md) 显示用户，并继承该用户的所有缓存配置。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-159">This component uses the [Person component](./person.md) to display the user and inherits all cache configuration from it.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="8cd7e-160">扩展以了解更多控件</span><span class="sxs-lookup"><span data-stu-id="8cd7e-160">Extend for more control</span></span>

<span data-ttu-id="8cd7e-161">对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展 `protected render*` 中替代的方法。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-161">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="8cd7e-162">方法</span><span class="sxs-lookup"><span data-stu-id="8cd7e-162">Method</span></span> | <span data-ttu-id="8cd7e-163">说明</span><span class="sxs-lookup"><span data-stu-id="8cd7e-163">Description</span></span> |
| - | - |
| <span data-ttu-id="8cd7e-164">renderButton</span><span class="sxs-lookup"><span data-stu-id="8cd7e-164">renderButton</span></span> | <span data-ttu-id="8cd7e-165">呈现按钮部件版式。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-165">Renders the button chrome.</span></span> |
| <span data-ttu-id="8cd7e-166">renderButtonContent</span><span class="sxs-lookup"><span data-stu-id="8cd7e-166">renderButtonContent</span></span> | <span data-ttu-id="8cd7e-167">呈现按钮内容。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-167">Renders the button content.</span></span> |
| <span data-ttu-id="8cd7e-168">renderSignedInButtonContent</span><span class="sxs-lookup"><span data-stu-id="8cd7e-168">renderSignedInButtonContent</span></span> | <span data-ttu-id="8cd7e-169">当用户登录时呈现按钮内容。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-169">Render the button content when the user is signed in.</span></span> |
| <span data-ttu-id="8cd7e-170">renderSignedOutButtonContent</span><span class="sxs-lookup"><span data-stu-id="8cd7e-170">renderSignedOutButtonContent</span></span> | <span data-ttu-id="8cd7e-171">当用户未登录时呈现按钮内容。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-171">Render the button content when the user is not signed in.</span></span> |
| <span data-ttu-id="8cd7e-172">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="8cd7e-172">renderFlyout</span></span> | <span data-ttu-id="8cd7e-173">呈现飞出部件版式。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-173">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="8cd7e-174">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="8cd7e-174">renderFlyoutContent</span></span> | <span data-ttu-id="8cd7e-175">呈现飞出内容。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-175">Renders the flyout content.</span></span> |
| <span data-ttu-id="8cd7e-176">renderFlyoutPersonDetails</span><span class="sxs-lookup"><span data-stu-id="8cd7e-176">renderFlyoutPersonDetails</span></span> | <span data-ttu-id="8cd7e-177">呈现飞出人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-177">Render the flyout person details.</span></span> |
| <span data-ttu-id="8cd7e-178">renderFlyoutCommands</span><span class="sxs-lookup"><span data-stu-id="8cd7e-178">renderFlyoutCommands</span></span> | <span data-ttu-id="8cd7e-179">呈现飞出命令。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-179">Render the flyout commands.</span></span> |

### <a name="bring-your-own-flyout"></a><span data-ttu-id="8cd7e-180">自带飞出</span><span class="sxs-lookup"><span data-stu-id="8cd7e-180">Bring your own flyout</span></span>

<span data-ttu-id="8cd7e-181">通过替代 方法并提供新的飞出，可以使用自己的飞出组件来替代内置 `renderFlyout()` 组件。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-181">It is possible to use your own flyout component in place of the built-in one, by overriding the `renderFlyout()` method and providing the new flyout.</span></span>

<span data-ttu-id="8cd7e-182">在这种情况下，通过覆盖飞出显示方法以更新备用飞出视图的可见性，确保登录组件继续按预期 `protected` 工作。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-182">In this case, ensure the login component continues to work as expected by overriding the `protected` flyout display methods to update the visibility of your alternative flyout.</span></span>

| <span data-ttu-id="8cd7e-183">方法</span><span class="sxs-lookup"><span data-stu-id="8cd7e-183">Method</span></span> | <span data-ttu-id="8cd7e-184">说明</span><span class="sxs-lookup"><span data-stu-id="8cd7e-184">Description</span></span> |
| - | - |
| <span data-ttu-id="8cd7e-185">hideFlyout</span><span class="sxs-lookup"><span data-stu-id="8cd7e-185">hideFlyout</span></span> | <span data-ttu-id="8cd7e-186">消除该飞出区。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-186">Dismisses the flyout.</span></span> |
| <span data-ttu-id="8cd7e-187">showFlyout</span><span class="sxs-lookup"><span data-stu-id="8cd7e-187">showFlyout</span></span> | <span data-ttu-id="8cd7e-188">显示飞出。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-188">Displays the flyout.</span></span> |
| <span data-ttu-id="8cd7e-189">toggleFlyout</span><span class="sxs-lookup"><span data-stu-id="8cd7e-189">toggleFlyout</span></span> | <span data-ttu-id="8cd7e-190">切换飞出状态。</span><span class="sxs-lookup"><span data-stu-id="8cd7e-190">Toggles the state of the flyout.</span></span> |
