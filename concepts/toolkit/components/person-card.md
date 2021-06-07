---
title: Person-Card Microsoft Graph Toolkit 中的组件
description: Person-Card组件是显示与人员相关详细信息的组件。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 8497dbb3b3d9a3173cdbf8ee8ec6bfe74859868b
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2021
ms.locfileid: "52780699"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="d2b50-103">Person-Card Microsoft Graph Toolkit 中的组件</span><span class="sxs-lookup"><span data-stu-id="d2b50-103">Person-Card component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="d2b50-104">Person-Card组件是一个响应式组件，用于显示与人员相关的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d2b50-104">A Person-Card component is a responsive component to display more information related to a person.</span></span> <span data-ttu-id="d2b50-105">它通常用作组件上的一个飞 `mgt-person` 出区。</span><span class="sxs-lookup"><span data-stu-id="d2b50-105">It is generally used as a flyout on the `mgt-person` component.</span></span>

<span data-ttu-id="d2b50-106">有关组件详细信息 `mgt-person` ，请参阅 [mgt-person](./person.md)。</span><span class="sxs-lookup"><span data-stu-id="d2b50-106">For more information about the `mgt-person` component, see [mgt-person](./person.md).</span></span>

## <a name="example"></a><span data-ttu-id="d2b50-107">示例</span><span class="sxs-lookup"><span data-stu-id="d2b50-107">Example</span></span>

<span data-ttu-id="d2b50-108">以下示例演示了组件 `mgt-person-card` 与组件的 `mgt-person` 使用。</span><span class="sxs-lookup"><span data-stu-id="d2b50-108">The following example shows the use of the `mgt-person-card` component with a `mgt-person` component.</span></span> <span data-ttu-id="d2b50-109">将鼠标悬停在人员上方以查看个人卡片，并使用代码编辑器查看属性 [如何更改组件](#properties) 的行为。</span><span class="sxs-lookup"><span data-stu-id="d2b50-109">Hover over the person to see the Person Card and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card&source=docs" height="400"></iframe>

[<span data-ttu-id="d2b50-110">在"打开"mgt.dev</span><span class="sxs-lookup"><span data-stu-id="d2b50-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person-card--person-card&source=docs)


## <a name="global-component-configuration"></a><span data-ttu-id="d2b50-111">全局组件配置</span><span class="sxs-lookup"><span data-stu-id="d2b50-111">Global component configuration</span></span>

<span data-ttu-id="d2b50-112">类 `MgtPersonCard` 公开一个 `config` 静态对象，该对象配置应用程序中的所有人员卡片组件。</span><span class="sxs-lookup"><span data-stu-id="d2b50-112">The `MgtPersonCard` class exposes a static `config` object that configures all person card components in the application.</span></span> <span data-ttu-id="d2b50-113">config 对象配置人员卡片使用哪些部分和哪些 API 从 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="d2b50-113">The config object configures what sections and what APIs are used by the person card to fetch details about a user from Microsoft Graph.</span></span>

<span data-ttu-id="d2b50-114">默认情况下，所有节和 API 都已启用。</span><span class="sxs-lookup"><span data-stu-id="d2b50-114">By default, all sections and APIs are enabled.</span></span> <span data-ttu-id="d2b50-115">以下示例演示如何使用 config 对象禁用节或 API。</span><span class="sxs-lookup"><span data-stu-id="d2b50-115">The following example shows how to use the config object to disable sections or APIs.</span></span>

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.useContactApis = false;
MgtPersonCard.config.sections.profile = false;
```

<span data-ttu-id="d2b50-116">以下属性在 config 对象上可用。</span><span class="sxs-lookup"><span data-stu-id="d2b50-116">The following properties are available on the config object.</span></span>

| <span data-ttu-id="d2b50-117">属性</span><span class="sxs-lookup"><span data-stu-id="d2b50-117">Property</span></span> | <span data-ttu-id="d2b50-118">说明</span><span class="sxs-lookup"><span data-stu-id="d2b50-118">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="d2b50-119">useContactApis</span><span class="sxs-lookup"><span data-stu-id="d2b50-119">useContactApis</span></span> | <span data-ttu-id="d2b50-120">`boolean`- 指示人员卡片组件是否可以使用 Microsoft Graph API 搜索联系人详细信息和照片。</span><span class="sxs-lookup"><span data-stu-id="d2b50-120">`boolean` - Indicates whether the person card component can use the Microsoft Graph Contact API to search for contact details and photos.</span></span> <span data-ttu-id="d2b50-121">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="d2b50-121">Default value is `true`.</span></span>  |
| <span data-ttu-id="d2b50-122">sections</span><span class="sxs-lookup"><span data-stu-id="d2b50-122">sections</span></span> | <span data-ttu-id="d2b50-123">`object` - 配置人员卡片中显示的部分。</span><span class="sxs-lookup"><span data-stu-id="d2b50-123">`object` - Configures what sections are shown in the person card.</span></span>  |

### <a name="person-card-sections"></a><span data-ttu-id="d2b50-124">个人卡片分区</span><span class="sxs-lookup"><span data-stu-id="d2b50-124">Person card sections</span></span>

<span data-ttu-id="d2b50-125">The person card contains several configurable sections for displaying person details：</span><span class="sxs-lookup"><span data-stu-id="d2b50-125">The person card contains several configurable sections for displaying person details:</span></span>
* <span data-ttu-id="d2b50-126">联系人 - 联系人信息，如电子邮件、电话、位置、位置等。</span><span class="sxs-lookup"><span data-stu-id="d2b50-126">Contact - Contact information such as email, phone, position, location, and more.</span></span>
* <span data-ttu-id="d2b50-127">组织 - 具有经理、直接下属和相关人员的组织图片。</span><span class="sxs-lookup"><span data-stu-id="d2b50-127">Organization - Organizational graph with managers, direct reports, and relevant people.</span></span>
* <span data-ttu-id="d2b50-128">邮件 - 具有当前登录用户的最相关的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="d2b50-128">Messages - Most relevant email messages with the current signed in user.</span></span>
* <span data-ttu-id="d2b50-129">文件 - 与当前登录用户最相关的共享文件。</span><span class="sxs-lookup"><span data-stu-id="d2b50-129">Files - Most relevant shared files with the current signed in user.</span></span>
* <span data-ttu-id="d2b50-130">配置文件 - 配置文件信息，如项目、技能、语言等。</span><span class="sxs-lookup"><span data-stu-id="d2b50-130">Profile - Profile information such as projects, skills, languages, and more.</span></span>

<span data-ttu-id="d2b50-131">默认情况下会加载节，但可通过 object 属性全局禁用 `MgtPersonCard.config.sections` 节。</span><span class="sxs-lookup"><span data-stu-id="d2b50-131">Sections are loaded by default, but they can be disabled globally via the `MgtPersonCard.config.sections` object property.</span></span> <span data-ttu-id="d2b50-132">以下属性可用。</span><span class="sxs-lookup"><span data-stu-id="d2b50-132">The following properties are available.</span></span>

| <span data-ttu-id="d2b50-133">属性</span><span class="sxs-lookup"><span data-stu-id="d2b50-133">Property</span></span> | <span data-ttu-id="d2b50-134">说明</span><span class="sxs-lookup"><span data-stu-id="d2b50-134">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="d2b50-135">组织</span><span class="sxs-lookup"><span data-stu-id="d2b50-135">organization</span></span> | <span data-ttu-id="d2b50-136">`boolean` - 指示是否显示个人卡片组织部分。</span><span class="sxs-lookup"><span data-stu-id="d2b50-136">`boolean` - Indicates whether the person card organization section is shown.</span></span> <span data-ttu-id="d2b50-137">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="d2b50-137">Default value is `true`.</span></span>  |
| <span data-ttu-id="d2b50-138">mailMessages</span><span class="sxs-lookup"><span data-stu-id="d2b50-138">mailMessages</span></span> | <span data-ttu-id="d2b50-139">`boolean` - 指示是否显示"人员卡片邮件"部分。</span><span class="sxs-lookup"><span data-stu-id="d2b50-139">`boolean` - Indicates whether the person card messages section is shown.</span></span> <span data-ttu-id="d2b50-140">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="d2b50-140">Default value is `true`.</span></span>  |
| <span data-ttu-id="d2b50-141">files</span><span class="sxs-lookup"><span data-stu-id="d2b50-141">files</span></span> | <span data-ttu-id="d2b50-142">`boolean` - 指示是否显示人员卡片文件部分。</span><span class="sxs-lookup"><span data-stu-id="d2b50-142">`boolean` - Indicates whether the person card files section is shown.</span></span> <span data-ttu-id="d2b50-143">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="d2b50-143">Default value is `true`.</span></span>  |
| <span data-ttu-id="d2b50-144">个人资料</span><span class="sxs-lookup"><span data-stu-id="d2b50-144">profile</span></span> | <span data-ttu-id="d2b50-145">`boolean` - 指示是否显示个人卡片配置文件部分。</span><span class="sxs-lookup"><span data-stu-id="d2b50-145">`boolean` - Indicates whether the person card profile section is shown.</span></span> <span data-ttu-id="d2b50-146">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="d2b50-146">Default value is `true`.</span></span>  |

<span data-ttu-id="d2b50-147">若要禁用分区，只需在应用初始化代码中将 `false` 属性设置为 ：</span><span class="sxs-lookup"><span data-stu-id="d2b50-147">To disable a section, simply set the property to `false` in your app initialization code:</span></span>
```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.sections.profile = false;
```

## <a name="setup-for-teams-integrations"></a><span data-ttu-id="d2b50-148">用于集成Teams安装程序</span><span class="sxs-lookup"><span data-stu-id="d2b50-148">Setup for Teams integrations</span></span>

<span data-ttu-id="d2b50-149">该Person-Card组件允许用户联系目标人员，包括通过Teams聊天。</span><span class="sxs-lookup"><span data-stu-id="d2b50-149">The Person-Card component allows the user to contact the target person, including via Teams chat.</span></span> <span data-ttu-id="d2b50-150">如果在选项卡应用中使用组件Teams，你可以确保组件深度直接链接到聊天，而不是通过设置 中的 打开浏览器 `microsoftTeamsLib` 窗口 `TeamsProvider` 。</span><span class="sxs-lookup"><span data-stu-id="d2b50-150">If using the component inside a Teams tab app, you can ensure that the component deep links directly to a chat instead of opening a browser window by setting the `microsoftTeamsLib` in `TeamsProvider`.</span></span>

<span data-ttu-id="d2b50-151">如果Person-Card无法检测到 Teams lib，该组件将尝试打开 Teams Web 客户端。</span><span class="sxs-lookup"><span data-stu-id="d2b50-151">If the Person-Card component is unable to detect the Teams lib, the component will attempt to open the Teams web client instead.</span></span>

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = microsoftTeams;
```

<span data-ttu-id="d2b50-152">有关提供程序详细信息 `TeamsProvider` ，请参阅Microsoft Teams[提供程序](../providers/teams.md)。</span><span class="sxs-lookup"><span data-stu-id="d2b50-152">For more information about the `TeamsProvider` provider, see [Microsoft Teams provider](../providers/teams.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d2b50-153">属性</span><span class="sxs-lookup"><span data-stu-id="d2b50-153">Properties</span></span>

<span data-ttu-id="d2b50-154">默认情况下， `mgt-person` 组件会向组件传递人员 `mgt-person-card` 详细信息。</span><span class="sxs-lookup"><span data-stu-id="d2b50-154">By default, the `mgt-person` component will pass the person details to the `mgt-person-card` component.</span></span> <span data-ttu-id="d2b50-155">但是，在模板化组件或将组件用作独立组件时，可以使用这些属性 `mgt-person` `mgt-person-card` 来更改这一点。</span><span class="sxs-lookup"><span data-stu-id="d2b50-155">However, you can use these attributes to change this when templating the `mgt-person` component or when using the `mgt-person-card` component as a standalone component.</span></span>

| <span data-ttu-id="d2b50-156">属性</span><span class="sxs-lookup"><span data-stu-id="d2b50-156">Attribute</span></span>         | <span data-ttu-id="d2b50-157">类型</span><span class="sxs-lookup"><span data-stu-id="d2b50-157">Type</span></span>                     | <span data-ttu-id="d2b50-158">说明</span><span class="sxs-lookup"><span data-stu-id="d2b50-158">Description</span></span>                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| <span data-ttu-id="d2b50-159">person-details</span><span class="sxs-lookup"><span data-stu-id="d2b50-159">person-details</span></span> | <span data-ttu-id="d2b50-160">MicrosoftGraph.User</span><span class="sxs-lookup"><span data-stu-id="d2b50-160">MicrosoftGraph.User</span></span> <br> <span data-ttu-id="d2b50-161">MicrosoftGraph.Person</span><span class="sxs-lookup"><span data-stu-id="d2b50-161">MicrosoftGraph.Person</span></span> <br> <span data-ttu-id="d2b50-162">MicrosoftGraph.Contact</span><span class="sxs-lookup"><span data-stu-id="d2b50-162">MicrosoftGraph.Contact</span></span> | <span data-ttu-id="d2b50-163">由 Microsoft Graph定义的 Person 对象，包含与用户相关的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d2b50-163">Person object as defined by Microsoft Graph, containing details related to the user.</span></span> |
| <span data-ttu-id="d2b50-164">person-image</span><span class="sxs-lookup"><span data-stu-id="d2b50-164">person-image</span></span>   | <span data-ttu-id="d2b50-165">string</span><span class="sxs-lookup"><span data-stu-id="d2b50-165">string</span></span>                    | <span data-ttu-id="d2b50-166">与卡片中显示的人员相关的图像 uri。</span><span class="sxs-lookup"><span data-stu-id="d2b50-166">Image uri related to the person displayed in the card.</span></span>                                   |
| <span data-ttu-id="d2b50-167">inherit-details</span><span class="sxs-lookup"><span data-stu-id="d2b50-167">inherit-details</span></span>   | <span data-ttu-id="d2b50-168">无。</span><span class="sxs-lookup"><span data-stu-id="d2b50-168">None.</span></span>                  | <span data-ttu-id="d2b50-169">允许个人卡片为组件演练父 `mgt-person` 树以使用相同 和 `person-details` `person-image` 数据。</span><span class="sxs-lookup"><span data-stu-id="d2b50-169">Allows person-card to walk parent tree for `mgt-person` component to use the same `person-details` and `person-image` data.</span></span>                      |
| <span data-ttu-id="d2b50-170">user-id</span><span class="sxs-lookup"><span data-stu-id="d2b50-170">user-id</span></span> | <span data-ttu-id="d2b50-171">string</span><span class="sxs-lookup"><span data-stu-id="d2b50-171">string</span></span> | <span data-ttu-id="d2b50-172">允许开发人员提供用户 ID 以检索显示在个人卡片组件上的数据</span><span class="sxs-lookup"><span data-stu-id="d2b50-172">Allows developers to supply user-id to retrieve data shown on person-card component</span></span> |
| <span data-ttu-id="d2b50-173">person-query</span><span class="sxs-lookup"><span data-stu-id="d2b50-173">person-query</span></span> | <span data-ttu-id="d2b50-174">string</span><span class="sxs-lookup"><span data-stu-id="d2b50-174">string</span></span> | <span data-ttu-id="d2b50-175">允许开发人员提供人员查询以检索显示在个人卡片组件上的数据</span><span class="sxs-lookup"><span data-stu-id="d2b50-175">Allows developers to supply person-query to retrieve data shown on person-card component</span></span> |


## <a name="templates"></a><span data-ttu-id="d2b50-176">模板</span><span class="sxs-lookup"><span data-stu-id="d2b50-176">Templates</span></span>

<span data-ttu-id="d2b50-177">该Person-Card组件使用允许您添加或[](../customize-components/templates.md)替换组件部分的模板。</span><span class="sxs-lookup"><span data-stu-id="d2b50-177">The Person-Card component uses [templates](../customize-components/templates.md) that allow you to add or replace portions of the component.</span></span> <span data-ttu-id="d2b50-178">若要指定模板，请包含组件 `<template>` 内的元素，将值 `data-type` 设置为以下值之一。</span><span class="sxs-lookup"><span data-stu-id="d2b50-178">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="d2b50-179">数据类型</span><span class="sxs-lookup"><span data-stu-id="d2b50-179">Data type</span></span> | <span data-ttu-id="d2b50-180">数据上下文</span><span class="sxs-lookup"><span data-stu-id="d2b50-180">Data context</span></span> | <span data-ttu-id="d2b50-181">说明</span><span class="sxs-lookup"><span data-stu-id="d2b50-181">Description</span></span> |
| - | - | - |
| <span data-ttu-id="d2b50-182">no-data</span><span class="sxs-lookup"><span data-stu-id="d2b50-182">no-data</span></span> | <span data-ttu-id="d2b50-183">空</span><span class="sxs-lookup"><span data-stu-id="d2b50-183">null</span></span> | <span data-ttu-id="d2b50-184">没有可用数据时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="d2b50-184">The template used when no data is available.</span></span>
| <span data-ttu-id="d2b50-185">default</span><span class="sxs-lookup"><span data-stu-id="d2b50-185">default</span></span> | <span data-ttu-id="d2b50-186">`person`：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="d2b50-186">`person`: The person details object</span></span> <br> <span data-ttu-id="d2b50-187">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="d2b50-187">`personImage`: The URL of the image</span></span> | <span data-ttu-id="d2b50-188">默认模板将整个组件替换为你自己的组件。</span><span class="sxs-lookup"><span data-stu-id="d2b50-188">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="d2b50-189">person-details</span><span class="sxs-lookup"><span data-stu-id="d2b50-189">person-details</span></span> | <span data-ttu-id="d2b50-190">`person`：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="d2b50-190">`person`: The person details object</span></span> | <span data-ttu-id="d2b50-191">用于呈现人员卡片顶部的模板。</span><span class="sxs-lookup"><span data-stu-id="d2b50-191">The template used to render the top part of the person card.</span></span> |
| <span data-ttu-id="d2b50-192">additional-details</span><span class="sxs-lookup"><span data-stu-id="d2b50-192">additional-details</span></span> | <span data-ttu-id="d2b50-193">`person`：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="d2b50-193">`person`: The person details object</span></span> <br> <span data-ttu-id="d2b50-194">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="d2b50-194">`personImage`: the URL of the image</span></span> | <span data-ttu-id="d2b50-195">用于将自定义内容添加到其他详细信息容器的模板。</span><span class="sxs-lookup"><span data-stu-id="d2b50-195">The template used to add custom content to the additional details container.</span></span> |

<span data-ttu-id="d2b50-196">例如，可以使用模板自定义附加到组件的组件，使用模板在 `mgt-person` 卡片中添加其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="d2b50-196">For example, you can use a template to customize the component attached to the `mgt-person` component and a template to add additional details in the card.</span></span> 

```html
    <mgt-person person-query="me" view="twolines" person-card="hover">
      <template data-type="person-card">
        <mgt-person-card inherit-details>
          <template data-type="additional-details">
            <h3>Stuffed Animal Friends:</h3>
            <ul>
              <li>Giraffe</li>
              <li>lion</li>
              <li>Rabbit</li>
            </ul>
          </template>
        </mgt-person-card>
      </template>
    </mgt-person>

```

## <a name="events"></a><span data-ttu-id="d2b50-197">活动</span><span class="sxs-lookup"><span data-stu-id="d2b50-197">Events</span></span>

<span data-ttu-id="d2b50-198">从组件中触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="d2b50-198">The following events are fired from the component.</span></span>

| <span data-ttu-id="d2b50-199">事件</span><span class="sxs-lookup"><span data-stu-id="d2b50-199">Event</span></span> | <span data-ttu-id="d2b50-200">说明</span><span class="sxs-lookup"><span data-stu-id="d2b50-200">Description</span></span> |
| --- | --- |
| `expanded` | <span data-ttu-id="d2b50-201">用户已打开卡片的展开详细信息部分。</span><span class="sxs-lookup"><span data-stu-id="d2b50-201">The user has opened the expanded details section of the card.</span></span> |

## <a name="css-custom-properties"></a><span data-ttu-id="d2b50-202">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="d2b50-202">CSS custom properties</span></span>

<span data-ttu-id="d2b50-203">组件 `mgt-person-card` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="d2b50-203">The `mgt-person-card` component defines the following CSS custom properties.</span></span> 

```css
mgt-person {
  --person-card-display-name-font-size: 40px;
  --person-card-display-name-color: #ffffff;
  --person-card-title-font-size: 20px;
  --person-card-title-color: #ffffff;
  --person-card-subtitle-font-size: 10px;
  --person-card-subtitle-color: #ffffff;
  --person-card-details-title-font-size: 10px;
  --person-card-details-title-color: #b3bf0a;
  --person-card-details-item-font-size: 20px;
  --person-card-details-item-color: #3abf0a;
  --person-card-background-color: #000000;
}
```

<span data-ttu-id="d2b50-204">若要了解更多信息，请参阅 [设置组件样式](../customize-components/style.md)。</span><span class="sxs-lookup"><span data-stu-id="d2b50-204">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="d2b50-205">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="d2b50-205">Microsoft Graph permissions</span></span>

<span data-ttu-id="d2b50-206">该Person-Card控件使用下列 Microsoft Graph API 和权限。</span><span class="sxs-lookup"><span data-stu-id="d2b50-206">The Person-Card control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="d2b50-207">配置</span><span class="sxs-lookup"><span data-stu-id="d2b50-207">Configuration</span></span> | <span data-ttu-id="d2b50-208">权限</span><span class="sxs-lookup"><span data-stu-id="d2b50-208">Permission</span></span> | <span data-ttu-id="d2b50-209">API</span><span class="sxs-lookup"><span data-stu-id="d2b50-209">API</span></span> | <span data-ttu-id="d2b50-210">节</span><span class="sxs-lookup"><span data-stu-id="d2b50-210">Section</span></span> |
| --- | ---------- | ------- | --------- |
| <span data-ttu-id="d2b50-211">`personDetails`使用用户的 但 `id` 不带电子邮件进行设置，或 `userId` 设置为 `personQuery``me`</span><span class="sxs-lookup"><span data-stu-id="d2b50-211">`personDetails` set with user's `id` but without e-mail, or `userId` set, or `personQuery` set to `me`</span></span> | <span data-ttu-id="d2b50-212">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="d2b50-212">User.ReadBasic.All</span></span> | <span data-ttu-id="d2b50-213">[/users/{id}](/graph/api/user-list-people)、 [/users/{id}/photo/$value](/graph/api/profilephoto-get)</span><span class="sxs-lookup"><span data-stu-id="d2b50-213">[/users/{id}](/graph/api/user-list-people), [/users/{id}/photo/$value](/graph/api/profilephoto-get)</span></span> | <span data-ttu-id="d2b50-214">默认值</span><span class="sxs-lookup"><span data-stu-id="d2b50-214">Default</span></span> |
| <span data-ttu-id="d2b50-215">`personQuery` 设置为不同于 `me`</span><span class="sxs-lookup"><span data-stu-id="d2b50-215">`personQuery` set to a value different than `me`</span></span> | <span data-ttu-id="d2b50-216">People.Read</span><span class="sxs-lookup"><span data-stu-id="d2b50-216">People.Read</span></span> | [<span data-ttu-id="d2b50-217">/me/people/？$search=</span><span class="sxs-lookup"><span data-stu-id="d2b50-217">/me/people/?$search=</span></span>](/graph/api/user-list-people) | <span data-ttu-id="d2b50-218">默认值</span><span class="sxs-lookup"><span data-stu-id="d2b50-218">Default</span></span> |
| <span data-ttu-id="d2b50-219">`personQuery` 设置为不同于 默认值的值 `me` `config.useContactApis` `true` ， (设置为) </span><span class="sxs-lookup"><span data-stu-id="d2b50-219">`personQuery` set to a value different than `me` and `config.useContactApis` set to `true` (default)</span></span> | <span data-ttu-id="d2b50-220">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d2b50-220">Contacts.Read</span></span> | [<span data-ttu-id="d2b50-221">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="d2b50-221">/me/contacts/\*</span></span>](/graph/api/user-list-contacts) | <span data-ttu-id="d2b50-222">默认值</span><span class="sxs-lookup"><span data-stu-id="d2b50-222">Default</span></span> |
| <span data-ttu-id="d2b50-223">`showPresence` 设置为 `true`</span><span class="sxs-lookup"><span data-stu-id="d2b50-223">`showPresence` set to `true`</span></span> | <span data-ttu-id="d2b50-224">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2b50-224">Presence.Read.All</span></span> | [<span data-ttu-id="d2b50-225">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="d2b50-225">/users/{id}/presence</span></span>](/graph/api/presence-get) | <span data-ttu-id="d2b50-226">默认值</span><span class="sxs-lookup"><span data-stu-id="d2b50-226">Default</span></span> |
| <span data-ttu-id="d2b50-227">`sections.organization` 已启用 (默认) </span><span class="sxs-lookup"><span data-stu-id="d2b50-227">`sections.organization` enabled (default)</span></span> | <span data-ttu-id="d2b50-228">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2b50-228">User.Read.All</span></span> | [<span data-ttu-id="d2b50-229">/users/{id}/manager</span><span class="sxs-lookup"><span data-stu-id="d2b50-229">/users/{id}/manager</span></span>](/graph/api/user-list-manager) | <span data-ttu-id="d2b50-230">组织</span><span class="sxs-lookup"><span data-stu-id="d2b50-230">Organization</span></span> |
| <span data-ttu-id="d2b50-231">`sections.organization.showWorksWith` 设置 (默认) </span><span class="sxs-lookup"><span data-stu-id="d2b50-231">`sections.organization.showWorksWith` set (default)</span></span> | <span data-ttu-id="d2b50-232">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2b50-232">People.Read.All</span></span> | [<span data-ttu-id="d2b50-233">/users/{id}/people</span><span class="sxs-lookup"><span data-stu-id="d2b50-233">/users/{id}/people</span></span>](/graph/api/user-list-people) | <span data-ttu-id="d2b50-234">组织</span><span class="sxs-lookup"><span data-stu-id="d2b50-234">Organization</span></span> |
| <span data-ttu-id="d2b50-235">`sections.mailMessages` 已启用 (默认) </span><span class="sxs-lookup"><span data-stu-id="d2b50-235">`sections.mailMessages` enabled (default)</span></span> | <span data-ttu-id="d2b50-236">Mail.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="d2b50-236">Mail.ReadBasic</span></span> | [<span data-ttu-id="d2b50-237">/me/messages</span><span class="sxs-lookup"><span data-stu-id="d2b50-237">/me/messages</span></span>](/graph/api/user-list-messages) | <span data-ttu-id="d2b50-238">邮件</span><span class="sxs-lookup"><span data-stu-id="d2b50-238">Messages</span></span> |
| <span data-ttu-id="d2b50-239">`sections.files` 已启用 (默认) </span><span class="sxs-lookup"><span data-stu-id="d2b50-239">`sections.files` enabled (default)</span></span> | <span data-ttu-id="d2b50-240">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2b50-240">Sites.Read.All</span></span> | <span data-ttu-id="d2b50-241">[/me/insights/shared](/graph/api/insights-list-shared) 和 [/me/insights/used](/graph/api/insights-list-used)</span><span class="sxs-lookup"><span data-stu-id="d2b50-241">[/me/insights/shared](/graph/api/insights-list-shared) and [/me/insights/used](/graph/api/insights-list-used)</span></span> | <span data-ttu-id="d2b50-242">文件</span><span class="sxs-lookup"><span data-stu-id="d2b50-242">Files</span></span> |

<span data-ttu-id="d2b50-243">该类还公开了一个静态方法，该方法返回人员卡片根据全局人员卡片配置运行所需的 `MgtPersonCard` `getScopes` 作用域数组。</span><span class="sxs-lookup"><span data-stu-id="d2b50-243">The `MgtPersonCard` class also exposes a `getScopes` static method that returns an array of scopes required for the person card to function based on the global person card configuration.</span></span>

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

const neededScopes = MgtPersonCard.getScopes();
```

## <a name="authentication"></a><span data-ttu-id="d2b50-244">身份验证</span><span class="sxs-lookup"><span data-stu-id="d2b50-244">Authentication</span></span>

<span data-ttu-id="d2b50-245">该Person-Card控件使用身份验证文档 中所述的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="d2b50-245">The Person-Card control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span> 

## <a name="cache"></a><span data-ttu-id="d2b50-246">缓存</span><span class="sxs-lookup"><span data-stu-id="d2b50-246">Cache</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d2b50-247">该 `mgt-person-card` 组件从父组件检索基本人员数据，而无需 `mgt-person` 调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="d2b50-247">The `mgt-person-card` component retrieves the basic person data from the parent `mgt-person` component without calling Microsoft Graph.</span></span> <span data-ttu-id="d2b50-248">单独 `mgt-person-card` 使用时，它将检索必要的数据本身并缓存它。</span><span class="sxs-lookup"><span data-stu-id="d2b50-248">When `mgt-person-card` is used separately, it will retrieve the necessary data itself and cache it.</span></span> <span data-ttu-id="d2b50-249">卡片分区中显示的数据是单独检索的，不会进行缓存。</span><span class="sxs-lookup"><span data-stu-id="d2b50-249">The data displayed in card's sections is retrieved separately and is not cached.</span></span>

|<span data-ttu-id="d2b50-250">对象存储</span><span class="sxs-lookup"><span data-stu-id="d2b50-250">Object store</span></span>|<span data-ttu-id="d2b50-251">缓存数据</span><span class="sxs-lookup"><span data-stu-id="d2b50-251">Cached data</span></span>|<span data-ttu-id="d2b50-252">备注</span><span class="sxs-lookup"><span data-stu-id="d2b50-252">Remarks</span></span>|
|---------|-----------|-------|
|`people`|<span data-ttu-id="d2b50-253">人员信息</span><span class="sxs-lookup"><span data-stu-id="d2b50-253">Person's information</span></span>|<span data-ttu-id="d2b50-254">指定 `personQuery` 时使用，其值不同于 `me`</span><span class="sxs-lookup"><span data-stu-id="d2b50-254">Used when `personQuery` is specified and its value is different than `me`</span></span>|
|`photos`|<span data-ttu-id="d2b50-255">人员照片</span><span class="sxs-lookup"><span data-stu-id="d2b50-255">Person's photo</span></span>|
|`presence`|<span data-ttu-id="d2b50-256">人员状态</span><span class="sxs-lookup"><span data-stu-id="d2b50-256">Person's presence</span></span>|<span data-ttu-id="d2b50-257">已使用， `showPresence` 设置为 `true`</span><span class="sxs-lookup"><span data-stu-id="d2b50-257">Used, when `showPresence` is set to `true`</span></span>|
|`users`|<span data-ttu-id="d2b50-258">人员的用户信息</span><span class="sxs-lookup"><span data-stu-id="d2b50-258">Person's user information</span></span>|<span data-ttu-id="d2b50-259">指定 `userId` 或 将 设置为 `personQuery` 时使用 `me`</span><span class="sxs-lookup"><span data-stu-id="d2b50-259">Used when `userId` is specified or the `personQuery` is set to `me`</span></span>|

<span data-ttu-id="d2b50-260">请参阅[Caching，](../customize-components/cache.md)了解有关如何配置缓存的更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="d2b50-260">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>
