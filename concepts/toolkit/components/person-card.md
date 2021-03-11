---
title: Person-Card Microsoft Graph Toolkit
description: Person-Card组件是显示与人员相关详细信息的组件。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 9acf9fd9c38128442d49d776f1f05646e2efe276
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722438"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="e81f0-103">Person-Card Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="e81f0-103">Person-Card component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="e81f0-104">Person-Card组件是一个响应式组件，用于显示与人员相关的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e81f0-104">A Person-Card component is a responsive component to display more information related to a person.</span></span> <span data-ttu-id="e81f0-105">它通常用作组件上的飞 `mgt-person` 出。</span><span class="sxs-lookup"><span data-stu-id="e81f0-105">It is generally used as a flyout on the `mgt-person` component.</span></span>

<span data-ttu-id="e81f0-106">有关组件详细信息 `mgt-person` ，请参阅[mgt-person。](./person.md)</span><span class="sxs-lookup"><span data-stu-id="e81f0-106">For more information about the `mgt-person` component, see [mgt-person](./person.md).</span></span>

## <a name="example"></a><span data-ttu-id="e81f0-107">示例</span><span class="sxs-lookup"><span data-stu-id="e81f0-107">Example</span></span>

<span data-ttu-id="e81f0-108">以下示例显示组件 `mgt-person-card` 与组件的 `mgt-person` 使用。</span><span class="sxs-lookup"><span data-stu-id="e81f0-108">The following example shows the use of the `mgt-person-card` component with a `mgt-person` component.</span></span> <span data-ttu-id="e81f0-109">将鼠标悬停在人员上方以查看人员卡片，并使用代码编辑器查看 [属性](#properties) 如何更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="e81f0-109">Hover over the person to see the Person Card and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card-hover&source=docs" height="400"></iframe>

[<span data-ttu-id="e81f0-110">在 mgt.dev 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="e81f0-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person-card--person-card-hover&source=docs)


## <a name="global-component-configuration"></a><span data-ttu-id="e81f0-111">全局组件配置</span><span class="sxs-lookup"><span data-stu-id="e81f0-111">Global component configuration</span></span>

<span data-ttu-id="e81f0-112">该类 `MgtPersonCard` 公开一个 `config` 静态对象，该对象配置应用程序中的所有人员卡片组件。</span><span class="sxs-lookup"><span data-stu-id="e81f0-112">The `MgtPersonCard` class exposes a static `config` object that configures all person card components in the application.</span></span> <span data-ttu-id="e81f0-113">config 对象配置人员卡片使用哪些部分和哪些 API 从 Microsoft Graph 获取有关用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e81f0-113">The config object configures what sections and what APIs are used by the person card to fetch details about a user from Microsoft Graph.</span></span>

<span data-ttu-id="e81f0-114">默认情况下，启用所有节和 API。</span><span class="sxs-lookup"><span data-stu-id="e81f0-114">By default, all sections and APIs are enabled.</span></span> <span data-ttu-id="e81f0-115">以下示例演示如何使用 config 对象禁用节或 API。</span><span class="sxs-lookup"><span data-stu-id="e81f0-115">The following example shows how to use the config object to disable sections or APIs.</span></span>

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.useContactApis = false;
MgtPersonCard.config.sections.profile = false;
```

<span data-ttu-id="e81f0-116">以下属性在 config 对象上可用。</span><span class="sxs-lookup"><span data-stu-id="e81f0-116">The following properties are available on the config object.</span></span>

| <span data-ttu-id="e81f0-117">属性</span><span class="sxs-lookup"><span data-stu-id="e81f0-117">Property</span></span> | <span data-ttu-id="e81f0-118">说明</span><span class="sxs-lookup"><span data-stu-id="e81f0-118">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="e81f0-119">useContactApis</span><span class="sxs-lookup"><span data-stu-id="e81f0-119">useContactApis</span></span> | <span data-ttu-id="e81f0-120">`boolean` - 指示人员卡片组件是否可以使用 Microsoft Graph 联系人 API 搜索联系人详细信息和照片。</span><span class="sxs-lookup"><span data-stu-id="e81f0-120">`boolean` - Indicates whether the person card component can use the Microsoft Graph Contact API to search for contact details and photos.</span></span> <span data-ttu-id="e81f0-121">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="e81f0-121">Default value is `true`.</span></span>  |
| <span data-ttu-id="e81f0-122">sections</span><span class="sxs-lookup"><span data-stu-id="e81f0-122">sections</span></span> | <span data-ttu-id="e81f0-123">`object` - 配置人员卡片中显示的部分。</span><span class="sxs-lookup"><span data-stu-id="e81f0-123">`object` - Configures what sections are shown in the person card.</span></span>  |

### <a name="person-card-sections"></a><span data-ttu-id="e81f0-124">人员卡片部分</span><span class="sxs-lookup"><span data-stu-id="e81f0-124">Person card sections</span></span>

<span data-ttu-id="e81f0-125">人员卡片包含用于显示人员详细信息的几个可配置部分：</span><span class="sxs-lookup"><span data-stu-id="e81f0-125">The person card contains several configurable sections for displaying person details:</span></span>
* <span data-ttu-id="e81f0-126">联系人 - 联系人信息，如电子邮件、电话、位置、位置等。</span><span class="sxs-lookup"><span data-stu-id="e81f0-126">Contact - Contact information such as email, phone, position, location, and more.</span></span>
* <span data-ttu-id="e81f0-127">组织 - 具有经理、直接下属和相关人员的组织图形。</span><span class="sxs-lookup"><span data-stu-id="e81f0-127">Organization - Organizational graph with managers, direct reports, and relevant people.</span></span>
* <span data-ttu-id="e81f0-128">邮件 - 与当前登录用户最相关的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="e81f0-128">Messages - Most relevant email messages with the current signed in user.</span></span>
* <span data-ttu-id="e81f0-129">文件 - 与当前登录用户最相关的共享文件。</span><span class="sxs-lookup"><span data-stu-id="e81f0-129">Files - Most relevant shared files with the current signed in user.</span></span>
* <span data-ttu-id="e81f0-130">配置文件 - 配置文件信息，如项目、技能、语言等。</span><span class="sxs-lookup"><span data-stu-id="e81f0-130">Profile - Profile information such as projects, skills, languages, and more.</span></span>

<span data-ttu-id="e81f0-131">默认情况下加载节，但可通过对象属性全局禁用 `MgtPersonCard.config.sections` 节。</span><span class="sxs-lookup"><span data-stu-id="e81f0-131">Sections are loaded by default, but they can be disabled globally via the `MgtPersonCard.config.sections` object property.</span></span> <span data-ttu-id="e81f0-132">以下属性可用。</span><span class="sxs-lookup"><span data-stu-id="e81f0-132">The following properties are available.</span></span>

| <span data-ttu-id="e81f0-133">属性</span><span class="sxs-lookup"><span data-stu-id="e81f0-133">Property</span></span> | <span data-ttu-id="e81f0-134">说明</span><span class="sxs-lookup"><span data-stu-id="e81f0-134">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="e81f0-135">组织</span><span class="sxs-lookup"><span data-stu-id="e81f0-135">organization</span></span> | <span data-ttu-id="e81f0-136">`boolean` - 指示是否显示"人员卡片组织"部分。</span><span class="sxs-lookup"><span data-stu-id="e81f0-136">`boolean` - Indicates whether the person card organization section is shown.</span></span> <span data-ttu-id="e81f0-137">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="e81f0-137">Default value is `true`.</span></span>  |
| <span data-ttu-id="e81f0-138">mailMessages</span><span class="sxs-lookup"><span data-stu-id="e81f0-138">mailMessages</span></span> | <span data-ttu-id="e81f0-139">`boolean` - 指示是否显示"人员卡片消息"部分。</span><span class="sxs-lookup"><span data-stu-id="e81f0-139">`boolean` - Indicates whether the person card messages section is shown.</span></span> <span data-ttu-id="e81f0-140">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="e81f0-140">Default value is `true`.</span></span>  |
| <span data-ttu-id="e81f0-141">files</span><span class="sxs-lookup"><span data-stu-id="e81f0-141">files</span></span> | <span data-ttu-id="e81f0-142">`boolean` - 指示是否显示"人员卡片文件"部分。</span><span class="sxs-lookup"><span data-stu-id="e81f0-142">`boolean` - Indicates whether the person card files section is shown.</span></span> <span data-ttu-id="e81f0-143">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="e81f0-143">Default value is `true`.</span></span>  |
| <span data-ttu-id="e81f0-144">个人资料</span><span class="sxs-lookup"><span data-stu-id="e81f0-144">profile</span></span> | <span data-ttu-id="e81f0-145">`boolean` - 指示是否显示个人卡片配置文件部分。</span><span class="sxs-lookup"><span data-stu-id="e81f0-145">`boolean` - Indicates whether the person card profile section is shown.</span></span> <span data-ttu-id="e81f0-146">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="e81f0-146">Default value is `true`.</span></span>  |

<span data-ttu-id="e81f0-147">若要禁用节，只需在应用初始化代码中 `false` 将属性设置为：</span><span class="sxs-lookup"><span data-stu-id="e81f0-147">To disable a section, simply set the property to `false` in your app initialization code:</span></span>
```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.sections.profile = false;
```

## <a name="setup-for-teams-integrations"></a><span data-ttu-id="e81f0-148">Teams 集成设置</span><span class="sxs-lookup"><span data-stu-id="e81f0-148">Setup for Teams integrations</span></span>

<span data-ttu-id="e81f0-149">此Person-Card组件允许用户联系目标人员，包括通过 Teams 聊天。</span><span class="sxs-lookup"><span data-stu-id="e81f0-149">The Person-Card component allows the user to contact the target person, including via Teams chat.</span></span> <span data-ttu-id="e81f0-150">如果使用 Teams 选项卡应用内的组件，你可以确保组件深层链接到聊天，而不是通过设置中的打开浏览器 `microsoftTeamsLib` 窗口 `TeamsProvider` 。</span><span class="sxs-lookup"><span data-stu-id="e81f0-150">If using the component inside a Teams tab app, you can ensure that the component deep links directly to a chat instead of opening a browser window by setting the `microsoftTeamsLib` in `TeamsProvider`.</span></span>

<span data-ttu-id="e81f0-151">如果Person-Card组件无法检测 Teams 库，则组件将改为尝试打开 Teams Web 客户端。</span><span class="sxs-lookup"><span data-stu-id="e81f0-151">If the Person-Card component is unable to detect the Teams lib, the component will attempt to open the Teams web client instead.</span></span>

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = microsoftTeams;
```

<span data-ttu-id="e81f0-152">有关提供程序详细信息 `TeamsProvider` ，请参阅 Microsoft [Teams 提供程序](../providers/teams.md)。</span><span class="sxs-lookup"><span data-stu-id="e81f0-152">For more information about the `TeamsProvider` provider, see [Microsoft Teams provider](../providers/teams.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e81f0-153">属性</span><span class="sxs-lookup"><span data-stu-id="e81f0-153">Properties</span></span>

<span data-ttu-id="e81f0-154">默认情况下， `mgt-person` 组件将人员详细信息传递到 `mgt-person-card` 组件。</span><span class="sxs-lookup"><span data-stu-id="e81f0-154">By default, the `mgt-person` component will pass the person details to the `mgt-person-card` component.</span></span> <span data-ttu-id="e81f0-155">但是，在模板化组件或将组件用作独立组件时，可以使用这些属性 `mgt-person` `mgt-person-card` 来更改这一点。</span><span class="sxs-lookup"><span data-stu-id="e81f0-155">However, you can use these attributes to change this when templating the `mgt-person` component or when using the `mgt-person-card` component as a standalone component.</span></span>

| <span data-ttu-id="e81f0-156">属性</span><span class="sxs-lookup"><span data-stu-id="e81f0-156">Attribute</span></span>         | <span data-ttu-id="e81f0-157">类型</span><span class="sxs-lookup"><span data-stu-id="e81f0-157">Type</span></span>                     | <span data-ttu-id="e81f0-158">说明</span><span class="sxs-lookup"><span data-stu-id="e81f0-158">Description</span></span>                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| <span data-ttu-id="e81f0-159">person-details</span><span class="sxs-lookup"><span data-stu-id="e81f0-159">person-details</span></span> | <span data-ttu-id="e81f0-160">MicrosoftGraph.User</span><span class="sxs-lookup"><span data-stu-id="e81f0-160">MicrosoftGraph.User</span></span> <br> <span data-ttu-id="e81f0-161">MicrosoftGraph.Person</span><span class="sxs-lookup"><span data-stu-id="e81f0-161">MicrosoftGraph.Person</span></span> <br> <span data-ttu-id="e81f0-162">MicrosoftGraph.Contact</span><span class="sxs-lookup"><span data-stu-id="e81f0-162">MicrosoftGraph.Contact</span></span> | <span data-ttu-id="e81f0-163">Microsoft Graph 定义的 Person 对象，包含与用户相关的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e81f0-163">Person object as defined by Microsoft Graph, containing details related to the user.</span></span> |
| <span data-ttu-id="e81f0-164">person-image</span><span class="sxs-lookup"><span data-stu-id="e81f0-164">person-image</span></span>   | <span data-ttu-id="e81f0-165">string</span><span class="sxs-lookup"><span data-stu-id="e81f0-165">string</span></span>                    | <span data-ttu-id="e81f0-166">与卡片中显示的人员相关的图像 uri。</span><span class="sxs-lookup"><span data-stu-id="e81f0-166">Image uri related to the person displayed in the card.</span></span>                                   |
| <span data-ttu-id="e81f0-167">inherit-details</span><span class="sxs-lookup"><span data-stu-id="e81f0-167">inherit-details</span></span>   | <span data-ttu-id="e81f0-168">无。</span><span class="sxs-lookup"><span data-stu-id="e81f0-168">None.</span></span>                  | <span data-ttu-id="e81f0-169">允许个人卡片为组件演练父树 `mgt-person` 以使用相同的 `person-details` `person-image` 数据和数据。</span><span class="sxs-lookup"><span data-stu-id="e81f0-169">Allows person-card to walk parent tree for `mgt-person` component to use the same `person-details` and `person-image` data.</span></span>                      |
| <span data-ttu-id="e81f0-170">user-id</span><span class="sxs-lookup"><span data-stu-id="e81f0-170">user-id</span></span> | <span data-ttu-id="e81f0-171">string</span><span class="sxs-lookup"><span data-stu-id="e81f0-171">string</span></span> | <span data-ttu-id="e81f0-172">允许开发人员提供用户 ID 以检索人员卡片组件上显示的数据</span><span class="sxs-lookup"><span data-stu-id="e81f0-172">Allows developers to supply user-id to retrieve data shown on person-card component</span></span> |
| <span data-ttu-id="e81f0-173">person-query</span><span class="sxs-lookup"><span data-stu-id="e81f0-173">person-query</span></span> | <span data-ttu-id="e81f0-174">string</span><span class="sxs-lookup"><span data-stu-id="e81f0-174">string</span></span> | <span data-ttu-id="e81f0-175">允许开发人员提供人员查询以检索人员卡片组件上显示的数据</span><span class="sxs-lookup"><span data-stu-id="e81f0-175">Allows developers to supply person-query to retrieve data shown on person-card component</span></span> |


## <a name="templates"></a><span data-ttu-id="e81f0-176">模板</span><span class="sxs-lookup"><span data-stu-id="e81f0-176">Templates</span></span>

<span data-ttu-id="e81f0-177">该Person-Card组件使用模板，允许您[](../customize-components/templates.md)添加或替换组件部分。</span><span class="sxs-lookup"><span data-stu-id="e81f0-177">The Person-Card component uses [templates](../customize-components/templates.md) that allow you to add or replace portions of the component.</span></span> <span data-ttu-id="e81f0-178">若要指定模板，请包含组件中的元素，将值设置为 `<template>` `data-type` 下列值之一。</span><span class="sxs-lookup"><span data-stu-id="e81f0-178">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="e81f0-179">数据类型</span><span class="sxs-lookup"><span data-stu-id="e81f0-179">Data type</span></span> | <span data-ttu-id="e81f0-180">数据上下文</span><span class="sxs-lookup"><span data-stu-id="e81f0-180">Data context</span></span> | <span data-ttu-id="e81f0-181">说明</span><span class="sxs-lookup"><span data-stu-id="e81f0-181">Description</span></span> |
| - | - | - |
| <span data-ttu-id="e81f0-182">no-data</span><span class="sxs-lookup"><span data-stu-id="e81f0-182">no-data</span></span> | <span data-ttu-id="e81f0-183">空</span><span class="sxs-lookup"><span data-stu-id="e81f0-183">null</span></span> | <span data-ttu-id="e81f0-184">没有可用数据时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="e81f0-184">The template used when no data is available.</span></span>
| <span data-ttu-id="e81f0-185">默认</span><span class="sxs-lookup"><span data-stu-id="e81f0-185">default</span></span> | <span data-ttu-id="e81f0-186">`person`：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="e81f0-186">`person`: The person details object</span></span> <br> <span data-ttu-id="e81f0-187">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="e81f0-187">`personImage`: The URL of the image</span></span> | <span data-ttu-id="e81f0-188">默认模板将整个组件替换为你自己的组件。</span><span class="sxs-lookup"><span data-stu-id="e81f0-188">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="e81f0-189">person-details</span><span class="sxs-lookup"><span data-stu-id="e81f0-189">person-details</span></span> | <span data-ttu-id="e81f0-190">`person`：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="e81f0-190">`person`: The person details object</span></span> | <span data-ttu-id="e81f0-191">用于呈现人员卡片顶部部分的模板。</span><span class="sxs-lookup"><span data-stu-id="e81f0-191">The template used to render the top part of the person card.</span></span> |
| <span data-ttu-id="e81f0-192">additional-details</span><span class="sxs-lookup"><span data-stu-id="e81f0-192">additional-details</span></span> | <span data-ttu-id="e81f0-193">`person`：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="e81f0-193">`person`: The person details object</span></span> <br> <span data-ttu-id="e81f0-194">`personImage`：图像的 URL</span><span class="sxs-lookup"><span data-stu-id="e81f0-194">`personImage`: the URL of the image</span></span> | <span data-ttu-id="e81f0-195">用于将自定义内容添加到其他详细信息容器的模板。</span><span class="sxs-lookup"><span data-stu-id="e81f0-195">The template used to add custom content to the additional details container.</span></span> |

<span data-ttu-id="e81f0-196">例如，可以使用模板自定义附加到组件的组件，使用模板在卡片中添加 `mgt-person` 其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="e81f0-196">For example, you can use a template to customize the component attached to the `mgt-person` component and a template to add additional details in the card.</span></span> 

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

## <a name="css-custom-properties"></a><span data-ttu-id="e81f0-197">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="e81f0-197">CSS custom properties</span></span>

<span data-ttu-id="e81f0-198">组件 `mgt-person-card` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="e81f0-198">The `mgt-person-card` component defines the following CSS custom properties.</span></span> 

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

<span data-ttu-id="e81f0-199">若要了解更多信息，请参阅 [样式组件](../customize-components/style.md)。</span><span class="sxs-lookup"><span data-stu-id="e81f0-199">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="microsoft-graph-apis-and-permissions"></a><span data-ttu-id="e81f0-200">Microsoft Graph API 和权限</span><span class="sxs-lookup"><span data-stu-id="e81f0-200">Microsoft Graph APIs and permissions</span></span>

<span data-ttu-id="e81f0-201">该Person-Card控件使用以下 Microsoft Graph API 和权限。</span><span class="sxs-lookup"><span data-stu-id="e81f0-201">The Person-Card control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="e81f0-202">资源</span><span class="sxs-lookup"><span data-stu-id="e81f0-202">Resource</span></span> | <span data-ttu-id="e81f0-203">权限</span><span class="sxs-lookup"><span data-stu-id="e81f0-203">Permission</span></span> | <span data-ttu-id="e81f0-204">分区</span><span class="sxs-lookup"><span data-stu-id="e81f0-204">Section</span></span> |
| - | - | - |
| [<span data-ttu-id="e81f0-205">/me</span><span class="sxs-lookup"><span data-stu-id="e81f0-205">/me</span></span>](/graph/api/user-get) | <span data-ttu-id="e81f0-206">User.Read</span><span class="sxs-lookup"><span data-stu-id="e81f0-206">User.Read</span></span> | <span data-ttu-id="e81f0-207">默认值</span><span class="sxs-lookup"><span data-stu-id="e81f0-207">Default</span></span> |
| [<span data-ttu-id="e81f0-208">/me/photo/$value</span><span class="sxs-lookup"><span data-stu-id="e81f0-208">/me/photo/$value</span></span>](/graph/api/profilephoto-get) | <span data-ttu-id="e81f0-209">User.Read</span><span class="sxs-lookup"><span data-stu-id="e81f0-209">User.Read</span></span> | <span data-ttu-id="e81f0-210">默认值</span><span class="sxs-lookup"><span data-stu-id="e81f0-210">Default</span></span> |
| [<span data-ttu-id="e81f0-211">/me/people/？$search=</span><span class="sxs-lookup"><span data-stu-id="e81f0-211">/me/people/?$search=</span></span>](/graph/api/user-list-people) | <span data-ttu-id="e81f0-212">People.Read</span><span class="sxs-lookup"><span data-stu-id="e81f0-212">People.Read</span></span> | <span data-ttu-id="e81f0-213">默认值</span><span class="sxs-lookup"><span data-stu-id="e81f0-213">Default</span></span> |
| [<span data-ttu-id="e81f0-214">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="e81f0-214">/me/contacts/\*</span></span>](/graph/api/user-list-contacts) | <span data-ttu-id="e81f0-215">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e81f0-215">Contacts.Read</span></span> | <span data-ttu-id="e81f0-216">默认值</span><span class="sxs-lookup"><span data-stu-id="e81f0-216">Default</span></span> |
| [<span data-ttu-id="e81f0-217">/users/{id}</span><span class="sxs-lookup"><span data-stu-id="e81f0-217">/users/{id}</span></span>](/graph/api/user-list-people) | <span data-ttu-id="e81f0-218">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="e81f0-218">User.ReadBasic.All</span></span> | <span data-ttu-id="e81f0-219">默认值</span><span class="sxs-lookup"><span data-stu-id="e81f0-219">Default</span></span> |
| [<span data-ttu-id="e81f0-220">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="e81f0-220">/users/{id}/photo/$value</span></span>](/graph/api/profilephoto-get) | <span data-ttu-id="e81f0-221">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="e81f0-221">User.ReadBasic.All</span></span> | <span data-ttu-id="e81f0-222">默认值</span><span class="sxs-lookup"><span data-stu-id="e81f0-222">Default</span></span> |
| [<span data-ttu-id="e81f0-223">/me/presence</span><span class="sxs-lookup"><span data-stu-id="e81f0-223">/me/presence</span></span>](/graph/api/presence-get) | <span data-ttu-id="e81f0-224">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="e81f0-224">Presence.Read</span></span> | <span data-ttu-id="e81f0-225">默认值</span><span class="sxs-lookup"><span data-stu-id="e81f0-225">Default</span></span> |
| [<span data-ttu-id="e81f0-226">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="e81f0-226">/users/{id}/presence</span></span>](/graph/api/presence-get) | <span data-ttu-id="e81f0-227">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="e81f0-227">Presence.Read.All</span></span> | <span data-ttu-id="e81f0-228">默认值</span><span class="sxs-lookup"><span data-stu-id="e81f0-228">Default</span></span> |
| [<span data-ttu-id="e81f0-229">/users/{id}/manager</span><span class="sxs-lookup"><span data-stu-id="e81f0-229">/users/{id}/manager</span></span>](/graph/api/user-list-manager) | <span data-ttu-id="e81f0-230">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e81f0-230">User.Read.All</span></span> | <span data-ttu-id="e81f0-231">组织</span><span class="sxs-lookup"><span data-stu-id="e81f0-231">Organization</span></span> |
| [<span data-ttu-id="e81f0-232">/users/{id}/directReports</span><span class="sxs-lookup"><span data-stu-id="e81f0-232">/users/{id}/directReports</span></span>](/graph/api/user-list-directreports) | <span data-ttu-id="e81f0-233">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e81f0-233">User.Read.All</span></span> | <span data-ttu-id="e81f0-234">组织</span><span class="sxs-lookup"><span data-stu-id="e81f0-234">Organization</span></span> |
| [<span data-ttu-id="e81f0-235">/users/{id}/people</span><span class="sxs-lookup"><span data-stu-id="e81f0-235">/users/{id}/people</span></span>](/graph/api/user-list-people) | <span data-ttu-id="e81f0-236">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="e81f0-236">People.Read.All</span></span> | <span data-ttu-id="e81f0-237">组织</span><span class="sxs-lookup"><span data-stu-id="e81f0-237">Organization</span></span> |
| [<span data-ttu-id="e81f0-238">/me/messages</span><span class="sxs-lookup"><span data-stu-id="e81f0-238">/me/messages</span></span>](/graph/api/user-list-messages) | <span data-ttu-id="e81f0-239">Mail.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="e81f0-239">Mail.ReadBasic</span></span> | <span data-ttu-id="e81f0-240">邮件</span><span class="sxs-lookup"><span data-stu-id="e81f0-240">Messages</span></span> |
| <span data-ttu-id="e81f0-241">[/me/insights/shared](/graph/api/insights-list-shared) 和 [/me/insights/used](/graph/api/insights-list-used)</span><span class="sxs-lookup"><span data-stu-id="e81f0-241">[/me/insights/shared](/graph/api/insights-list-shared) and [/me/insights/used](/graph/api/insights-list-used)</span></span> | <span data-ttu-id="e81f0-242">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="e81f0-242">Sites.Read.All</span></span> | <span data-ttu-id="e81f0-243">文件</span><span class="sxs-lookup"><span data-stu-id="e81f0-243">Files</span></span> |
| [<span data-ttu-id="e81f0-244">/users/{id}/profile</span><span class="sxs-lookup"><span data-stu-id="e81f0-244">/users/{id}/profile</span></span>](/graph/api/profile-get) | <span data-ttu-id="e81f0-245">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e81f0-245">User.Read.All</span></span> | <span data-ttu-id="e81f0-246">个人资料</span><span class="sxs-lookup"><span data-stu-id="e81f0-246">Profile</span></span> |

<span data-ttu-id="e81f0-247">该类还公开了一个静态方法，该方法返回根据全局人员卡片配置运行人员卡片所需的一 `MgtPersonCard` `getScopes` 组作用域。</span><span class="sxs-lookup"><span data-stu-id="e81f0-247">The `MgtPersonCard` class also exposes a `getScopes` static method that returns an array of scopes required for the person card to function based on the global person card configuration.</span></span>

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

const neededScopes = MgtPersonCard.getScopes();
```

## <a name="authentication"></a><span data-ttu-id="e81f0-248">身份验证</span><span class="sxs-lookup"><span data-stu-id="e81f0-248">Authentication</span></span>

<span data-ttu-id="e81f0-249">该Person-Card使用身份验证文档中介绍的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="e81f0-249">The Person-Card control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span> 
