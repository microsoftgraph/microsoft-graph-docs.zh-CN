---
title: Microsoft 服务中的登录Graph Toolkit
description: 登录组件是一个按钮和飞出控件，用于简化Microsoft 标识平台身份验证。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: ea7df01c77900eecc415b3670db0ea2736447d8c
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781077"
---
# <a name="login-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="b123a-103">Microsoft 服务中的登录Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="b123a-103">Login component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="b123a-104">登录组件是一个按钮和飞出控件，用于简化Microsoft 标识平台身份验证。</span><span class="sxs-lookup"><span data-stu-id="b123a-104">A Login component is a button and flyout control to facilitate Microsoft identity platform authentication.</span></span> <span data-ttu-id="b123a-105">它提供两种状态：</span><span class="sxs-lookup"><span data-stu-id="b123a-105">It provides two states:</span></span>
* <span data-ttu-id="b123a-106">当用户未登录时，控件是一个简单的按钮，用于启动登录过程。</span><span class="sxs-lookup"><span data-stu-id="b123a-106">When user is not signed in, the control is a simple button to initiate the sign in process.</span></span>
* <span data-ttu-id="b123a-107">用户登录后，控件将显示当前登录的用户名、个人资料图像和电子邮件。</span><span class="sxs-lookup"><span data-stu-id="b123a-107">When user is signed in, the control displays the current signed in user name, profile image, and email.</span></span> <span data-ttu-id="b123a-108">单击后，将打开一个具有注销命令的飞出。</span><span class="sxs-lookup"><span data-stu-id="b123a-108">When clicked, a flyout is opened with a command to sign out.</span></span>

## <a name="example"></a><span data-ttu-id="b123a-109">示例</span><span class="sxs-lookup"><span data-stu-id="b123a-109">Example</span></span>

<span data-ttu-id="b123a-110">以下示例显示了 `mgt-login` 具有已登录用户的组件。</span><span class="sxs-lookup"><span data-stu-id="b123a-110">The following example shows the `mgt-login` component with a signed-in user.</span></span> 

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-login--login&source=docs" height="350"></iframe>

[<span data-ttu-id="b123a-111">在"打开"mgt.dev</span><span class="sxs-lookup"><span data-stu-id="b123a-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-login--login&source=docs)

## <a name="using-the-control-without-an-authentication-provider"></a><span data-ttu-id="b123a-112">在没有身份验证提供程序的情况下使用控件</span><span class="sxs-lookup"><span data-stu-id="b123a-112">Using the control without an authentication provider</span></span>

<span data-ttu-id="b123a-113">该组件适用于提供程序和 Microsoft Graph开箱即用。</span><span class="sxs-lookup"><span data-stu-id="b123a-113">The component works with a provider and Microsoft Graph out of the box.</span></span> <span data-ttu-id="b123a-114">但是，如果要提供自己的逻辑和身份验证，可以使用 属性设置 `userDetails` 登录用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b123a-114">However, if you want to provide your own logic and authentication, you can use the `userDetails` property to set the signed in user's details.</span></span> 

| <span data-ttu-id="b123a-115">属性</span><span class="sxs-lookup"><span data-stu-id="b123a-115">Attribute</span></span> | <span data-ttu-id="b123a-116">属性</span><span class="sxs-lookup"><span data-stu-id="b123a-116">Property</span></span> | <span data-ttu-id="b123a-117">说明</span><span class="sxs-lookup"><span data-stu-id="b123a-117">Description</span></span> |
| --- | --- | -- |
| <span data-ttu-id="b123a-118">user-details</span><span class="sxs-lookup"><span data-stu-id="b123a-118">user-details</span></span> | <span data-ttu-id="b123a-119">userDetails</span><span class="sxs-lookup"><span data-stu-id="b123a-119">userDetails</span></span> | <span data-ttu-id="b123a-120">设置将在控件上显示的用户对象。</span><span class="sxs-lookup"><span data-stu-id="b123a-120">Set the user object that will be displayed on the control.</span></span> |

<span data-ttu-id="b123a-121">以下示例设置人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="b123a-121">The following example sets the person details.</span></span>

```js
let loginControl = document.getElementById('myLoginControl');
loginControl.userDetails = {
    displayName: 'Nikola Metulev',
    mail: 'nikola@contoso.com',
    personImage: 'url'
}
```

<span data-ttu-id="b123a-122">设置为 `userDetails` `null` 将转到已退出状态。</span><span class="sxs-lookup"><span data-stu-id="b123a-122">Setting `userDetails` to `null` will go to the signed out state.</span></span>

<span data-ttu-id="b123a-123">使用 `loginInitiated` 和 `logoutInitiated` 事件处理登录和退出。</span><span class="sxs-lookup"><span data-stu-id="b123a-123">Use the `loginInitiated` and `logoutInitiated` events to handle signing in and out.</span></span> 

## <a name="css-custom-properties"></a><span data-ttu-id="b123a-124">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="b123a-124">CSS custom properties</span></span>

<span data-ttu-id="b123a-125">组件 `mgt-login` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="b123a-125">The `mgt-login` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="b123a-126">若要了解更多信息，请参阅 [设置组件样式](../customize-components/style.md)。</span><span class="sxs-lookup"><span data-stu-id="b123a-126">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="b123a-127">活动</span><span class="sxs-lookup"><span data-stu-id="b123a-127">Events</span></span>

<span data-ttu-id="b123a-128">从控件中触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="b123a-128">The following events are fired from the control.</span></span>

| <span data-ttu-id="b123a-129">事件</span><span class="sxs-lookup"><span data-stu-id="b123a-129">Event</span></span> | <span data-ttu-id="b123a-130">说明</span><span class="sxs-lookup"><span data-stu-id="b123a-130">Description</span></span> |
| --- | --- |
| `loginInitiated` | <span data-ttu-id="b123a-131">用户单击登录按钮以启动登录过程 - 可取消。</span><span class="sxs-lookup"><span data-stu-id="b123a-131">The user clicked the sign in button to start the login process - cancelable.</span></span>|
| `loginCompleted` | <span data-ttu-id="b123a-132">登录过程成功，用户现已登录。</span><span class="sxs-lookup"><span data-stu-id="b123a-132">the login process was successful and the user is now signed in.</span></span> |
| `loginFailed` | <span data-ttu-id="b123a-133">用户已取消登录过程或无法登录。</span><span class="sxs-lookup"><span data-stu-id="b123a-133">The user canceled the login process or was unable to sign in.</span></span>|
| `logoutInitiated` | <span data-ttu-id="b123a-134">用户开始注销 - 可取消。</span><span class="sxs-lookup"><span data-stu-id="b123a-134">The user started to logout - cancelable.</span></span> |
| `logoutCompleted` | <span data-ttu-id="b123a-135">用户已退出。</span><span class="sxs-lookup"><span data-stu-id="b123a-135">The user signed out.</span></span> |

## <a name="templates"></a><span data-ttu-id="b123a-136">模板</span><span class="sxs-lookup"><span data-stu-id="b123a-136">Templates</span></span>

<span data-ttu-id="b123a-137">组件 `mgt-login` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="b123a-137">The `mgt-login` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="b123a-138">若要指定模板，请包含组件内的元素，将值设置为下表 `<template>` `data-type` 中列出的值之一。</span><span class="sxs-lookup"><span data-stu-id="b123a-138">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the values listed in the following table.</span></span> 

| <span data-ttu-id="b123a-139">数据类型</span><span class="sxs-lookup"><span data-stu-id="b123a-139">Data type</span></span> | <span data-ttu-id="b123a-140">数据上下文</span><span class="sxs-lookup"><span data-stu-id="b123a-140">Data context</span></span> | <span data-ttu-id="b123a-141">说明</span><span class="sxs-lookup"><span data-stu-id="b123a-141">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="b123a-142">signed-in-button-content</span><span class="sxs-lookup"><span data-stu-id="b123a-142">signed-in-button-content</span></span> | <span data-ttu-id="b123a-143">personDetails： person object， `personImage` ： person image string</span><span class="sxs-lookup"><span data-stu-id="b123a-143">personDetails: person object, `personImage`: person image string</span></span> | <span data-ttu-id="b123a-144">用于当用户登录时在按钮中呈现内容的模板。</span><span class="sxs-lookup"><span data-stu-id="b123a-144">The template used to render the content in the button when the user is signed in.</span></span> |
| <span data-ttu-id="b123a-145">signed-out-button-content</span><span class="sxs-lookup"><span data-stu-id="b123a-145">signed-out-button-content</span></span> | <span data-ttu-id="b123a-146">空</span><span class="sxs-lookup"><span data-stu-id="b123a-146">null</span></span> | <span data-ttu-id="b123a-147">用于当用户未登录时在按钮中呈现内容的模板。</span><span class="sxs-lookup"><span data-stu-id="b123a-147">The template used to render the content in the button when the user is not signed in.</span></span> |
| <span data-ttu-id="b123a-148">flyout-commands</span><span class="sxs-lookup"><span data-stu-id="b123a-148">flyout-commands</span></span> | <span data-ttu-id="b123a-149">handleSignOut：注销函数</span><span class="sxs-lookup"><span data-stu-id="b123a-149">handleSignOut: sign out function</span></span> | <span data-ttu-id="b123a-150">用于在飞出控件中呈现命令的模板</span><span class="sxs-lookup"><span data-stu-id="b123a-150">The template used to render the commands in the flyout</span></span> |
| <span data-ttu-id="b123a-151">flyout-person-details</span><span class="sxs-lookup"><span data-stu-id="b123a-151">flyout-person-details</span></span> | <span data-ttu-id="b123a-152">personDetails： person object， personImage： person image string</span><span class="sxs-lookup"><span data-stu-id="b123a-152">personDetails: person object, personImage: person image string</span></span> | <span data-ttu-id="b123a-153">用于在飞出控件中呈现人员详细信息的模板。</span><span class="sxs-lookup"><span data-stu-id="b123a-153">The template used to render the person details in the flyout.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="b123a-154">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="b123a-154">Microsoft Graph permissions</span></span>

<span data-ttu-id="b123a-155">此组件使用以下 Microsoft Graph API 和权限：</span><span class="sxs-lookup"><span data-stu-id="b123a-155">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="b123a-156">配置</span><span class="sxs-lookup"><span data-stu-id="b123a-156">Configuration</span></span> | <span data-ttu-id="b123a-157">权限</span><span class="sxs-lookup"><span data-stu-id="b123a-157">Permission</span></span> | <span data-ttu-id="b123a-158">API</span><span class="sxs-lookup"><span data-stu-id="b123a-158">API</span></span>
| - | - | - |
| <span data-ttu-id="b123a-159">default</span><span class="sxs-lookup"><span data-stu-id="b123a-159">default</span></span> | <span data-ttu-id="b123a-160">User.Read</span><span class="sxs-lookup"><span data-stu-id="b123a-160">User.Read</span></span> | [<span data-ttu-id="b123a-161">/users/me/</span><span class="sxs-lookup"><span data-stu-id="b123a-161">/users/me/</span></span>](/graph/api/user-get) |

<span data-ttu-id="b123a-162">使用默认 `signed-in-button-content` 和 `flyout-person-details` 模板时，此组件使用 [Person](./person.md) 组件显示用户并继承所有权限。</span><span class="sxs-lookup"><span data-stu-id="b123a-162">When using the default `signed-in-button-content` and `flyout-person-details` templates, this component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span>

## <a name="authentication"></a><span data-ttu-id="b123a-163">身份验证</span><span class="sxs-lookup"><span data-stu-id="b123a-163">Authentication</span></span>

<span data-ttu-id="b123a-164">登录控件使用身份验证文档 中所述的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="b123a-164">The login control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span> 

## <a name="cache"></a><span data-ttu-id="b123a-165">缓存</span><span class="sxs-lookup"><span data-stu-id="b123a-165">Cache</span></span>

<span data-ttu-id="b123a-166">此组件使用 [Person 组件](./person.md) 显示用户，并继承该用户的所有缓存配置。</span><span class="sxs-lookup"><span data-stu-id="b123a-166">This component uses the [Person component](./person.md) to display the user and inherits all cache configuration from it.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="b123a-167">扩展以了解更多控件</span><span class="sxs-lookup"><span data-stu-id="b123a-167">Extend for more control</span></span>

<span data-ttu-id="b123a-168">对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展 `protected render*` 中替代的方法。</span><span class="sxs-lookup"><span data-stu-id="b123a-168">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="b123a-169">方法</span><span class="sxs-lookup"><span data-stu-id="b123a-169">Method</span></span> | <span data-ttu-id="b123a-170">说明</span><span class="sxs-lookup"><span data-stu-id="b123a-170">Description</span></span> |
| - | - |
| <span data-ttu-id="b123a-171">renderButton</span><span class="sxs-lookup"><span data-stu-id="b123a-171">renderButton</span></span> | <span data-ttu-id="b123a-172">呈现按钮部件版式。</span><span class="sxs-lookup"><span data-stu-id="b123a-172">Renders the button chrome.</span></span> |
| <span data-ttu-id="b123a-173">renderButtonContent</span><span class="sxs-lookup"><span data-stu-id="b123a-173">renderButtonContent</span></span> | <span data-ttu-id="b123a-174">呈现按钮内容。</span><span class="sxs-lookup"><span data-stu-id="b123a-174">Renders the button content.</span></span> |
| <span data-ttu-id="b123a-175">renderSignedInButtonContent</span><span class="sxs-lookup"><span data-stu-id="b123a-175">renderSignedInButtonContent</span></span> | <span data-ttu-id="b123a-176">当用户登录时呈现按钮内容。</span><span class="sxs-lookup"><span data-stu-id="b123a-176">Render the button content when the user is signed in.</span></span> |
| <span data-ttu-id="b123a-177">renderSignedOutButtonContent</span><span class="sxs-lookup"><span data-stu-id="b123a-177">renderSignedOutButtonContent</span></span> | <span data-ttu-id="b123a-178">当用户未登录时呈现按钮内容。</span><span class="sxs-lookup"><span data-stu-id="b123a-178">Render the button content when the user is not signed in.</span></span> |
| <span data-ttu-id="b123a-179">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="b123a-179">renderFlyout</span></span> | <span data-ttu-id="b123a-180">呈现飞出部件版式。</span><span class="sxs-lookup"><span data-stu-id="b123a-180">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="b123a-181">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="b123a-181">renderFlyoutContent</span></span> | <span data-ttu-id="b123a-182">呈现飞出内容。</span><span class="sxs-lookup"><span data-stu-id="b123a-182">Renders the flyout content.</span></span> |
| <span data-ttu-id="b123a-183">renderFlyoutPersonDetails</span><span class="sxs-lookup"><span data-stu-id="b123a-183">renderFlyoutPersonDetails</span></span> | <span data-ttu-id="b123a-184">呈现飞出人员详细信息。</span><span class="sxs-lookup"><span data-stu-id="b123a-184">Render the flyout person details.</span></span> |
| <span data-ttu-id="b123a-185">renderFlyoutCommands</span><span class="sxs-lookup"><span data-stu-id="b123a-185">renderFlyoutCommands</span></span> | <span data-ttu-id="b123a-186">呈现飞出命令。</span><span class="sxs-lookup"><span data-stu-id="b123a-186">Render the flyout commands.</span></span> |

### <a name="bring-your-own-flyout"></a><span data-ttu-id="b123a-187">自带飞出</span><span class="sxs-lookup"><span data-stu-id="b123a-187">Bring your own flyout</span></span>

<span data-ttu-id="b123a-188">通过替代 方法并提供新的飞出，可以使用自己的飞出组件来替代内置 `renderFlyout()` 组件。</span><span class="sxs-lookup"><span data-stu-id="b123a-188">It is possible to use your own flyout component in place of the built-in one, by overriding the `renderFlyout()` method and providing the new flyout.</span></span>

<span data-ttu-id="b123a-189">在这种情况下，通过覆盖飞出显示方法以更新备用飞出视图的可见性，确保登录组件继续按预期 `protected` 工作。</span><span class="sxs-lookup"><span data-stu-id="b123a-189">In this case, ensure the login component continues to work as expected by overriding the `protected` flyout display methods to update the visibility of your alternative flyout.</span></span>

| <span data-ttu-id="b123a-190">方法</span><span class="sxs-lookup"><span data-stu-id="b123a-190">Method</span></span> | <span data-ttu-id="b123a-191">说明</span><span class="sxs-lookup"><span data-stu-id="b123a-191">Description</span></span> |
| - | - |
| <span data-ttu-id="b123a-192">hideFlyout</span><span class="sxs-lookup"><span data-stu-id="b123a-192">hideFlyout</span></span> | <span data-ttu-id="b123a-193">消除该飞出区。</span><span class="sxs-lookup"><span data-stu-id="b123a-193">Dismisses the flyout.</span></span> |
| <span data-ttu-id="b123a-194">showFlyout</span><span class="sxs-lookup"><span data-stu-id="b123a-194">showFlyout</span></span> | <span data-ttu-id="b123a-195">显示飞出。</span><span class="sxs-lookup"><span data-stu-id="b123a-195">Displays the flyout.</span></span> |
| <span data-ttu-id="b123a-196">toggleFlyout</span><span class="sxs-lookup"><span data-stu-id="b123a-196">toggleFlyout</span></span> | <span data-ttu-id="b123a-197">切换飞出状态。</span><span class="sxs-lookup"><span data-stu-id="b123a-197">Toggles the state of the flyout.</span></span> |
