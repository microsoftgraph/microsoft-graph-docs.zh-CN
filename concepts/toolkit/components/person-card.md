---
title: Microsoft Graph Toolkit中的Person-Card组件
description: Person-Card组件是一个组件，用于显示与人员相关的详细信息。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 20f34becb875b7bd8dd10bfdafce28fd6d14c808
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398319"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph Toolkit中的Person-Card组件

Person-Card组件是响应式组件，用于显示与人员相关的详细信息。 它通常用作组件上的 `mgt-person` 浮出控件。

有关组件的 `mgt-person` 详细信息，请参阅 [mgt-person](./person.md)。

## <a name="example"></a>示例

以下示例演示组件与组件的`mgt-person`使用`mgt-person-card`情况。 将鼠标悬停在人员上查看人员卡片，并使用代码编辑器查看 [属性](#properties) 如何更改组件的行为。
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card&source=docs" height="400"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-person-card--person-card&source=docs)


## <a name="global-component-configuration"></a>全局组件配置

该 `MgtPersonCard` 类公开一个静态 `config` 对象，该对象配置应用程序中的所有人员卡组件。 配置对象配置人员卡使用哪些部分和哪些 API 从 Microsoft Graph 提取有关用户的详细信息。

默认情况下，所有节和 API 均已启用。 以下示例演示如何使用配置对象禁用分区或 API。

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.useContactApis = false;
MgtPersonCard.config.sections.profile = false;
```

配置对象上提供了以下属性。

| 属性 | 说明 |
| ------------ | ------------- |
| useContactApis | `boolean`- 指示人员卡组件是否可以使用 Microsoft Graph联系人 API 来搜索联系人详细信息和照片。 默认值为 `true`。  |
| sections | `object` - 配置人员卡片中显示的部分。  |

### <a name="person-card-sections"></a>人员卡片部分

人员卡包含多个可配置部分，用于显示人员详细信息：
* 联系人 - 联系人信息，如电子邮件、电话、位置、位置等。
* 组织 - 包含经理、直接报告和相关人员的组织图。
* 邮件 - 具有当前登录用户的大多数相关电子邮件。
* 文件 - 具有当前已登录用户的最相关共享文件。
* 配置文件 - 配置文件信息，如项目、技能、语言等。

默认情况下会加载节，但可以通过对象属性全局禁用 `MgtPersonCard.config.sections` 这些节。 以下属性可用。

| 属性 | 说明 |
| ------------ | ------------- |
| 组织 | `boolean` - 指示是否显示人员卡组织部分。 默认值为 `true`。  |
| mailMessages | `boolean` - 指示是否显示人员卡片消息部分。 默认值为 `true`。  |
| files | `boolean` - 指示是否显示人员卡片文件部分。 默认值为 `true`。  |
| 个人资料 | `boolean` - 指示是否显示人员卡配置文件部分。 默认值为 `true`。  |

若要禁用分区，只需在应用初始化代码中将属性设置为 `false` ：
```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.sections.profile = false;
```

## <a name="setup-for-teams-integrations"></a>设置Teams集成

Person-Card组件允许用户联系目标人员，包括通过Teams聊天。 如果在Teams选项卡应用中使用该组件，则可以确保组件直接链接到聊天，而不是通过设置`microsoftTeamsLib`其中`TeamsProvider`打开浏览器窗口。

如果Person-Card组件无法检测Teams lib，则组件将尝试打开Teams Web 客户端。

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = microsoftTeams;
```

有关提供程序的`TeamsProvider`详细信息，请[参阅Microsoft Teams提供程序](../providers/teams.md)。

## <a name="properties"></a>属性

默认情况下 `mgt-person` ，组件会将人员详细信息传递给 `mgt-person-card` 组件。 但是，在模板化 `mgt-person` 组件或将 `mgt-person-card` 组件用作独立组件时，可以使用这些属性来更改此属性。

| 属性         | 类型                     | 说明                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| person-details | MicrosoftGraph.User <br> MicrosoftGraph.Person <br> MicrosoftGraph.Contact | Microsoft Graph定义的 Person 对象，包含与用户相关的详细信息。 |
| person-image   | string                    | 与卡片中显示的人员相关的图像 uri。                                   |
| inherit-details   | 无。                  | 允许人卡走父树，使 `mgt-person` 组件使用相同 `person-details` 数据 `person-image` 。                      |
| user-id | string | 允许开发人员提供用户 ID 以检索人员卡组件上显示的数据 |
| person-query | string | 允许开发人员提供人员查询来检索人员卡组件上显示的数据 |
| person-card | string | 指定 `person-card` 在悬停或单击 `mgt-person` 组件时，组件可以显示为弹出卡片。 允许的值为 `hover` 或 `click`.


## <a name="templates"></a>模板

Person-Card组件使用允许添加或替换组件部分的 [模板](../customize-components/templates.md) 。 若要指定模板，请在组件中包含一个 `<template>` 元素， `data-type` 并将值设置为下列值之一。

| 数据类型 | 数据上下文 | 说明 |
| - | - | - |
| no-data | 空 | 没有可用数据时使用的模板。
| 默认 | `person`：人员详细信息对象 <br> `personImage`：图像的 URL | 默认模板将整个组件替换为你自己的组件。 |
| person-details | `person`：人员详细信息对象 | 用于呈现人员卡片上部的模板。 |
| additional-details | `person`：人员详细信息对象 <br> `personImage`：图像的 URL | 用于将自定义内容添加到其他详细信息容器的模板。 |

例如，可以使用模板自定义附加到组件的 `mgt-person` 组件和模板，以便在卡片中添加其他详细信息。 

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

## <a name="events"></a>活动

从组件触发以下事件。

事件 | 何时发出 | 自定义数据 | 可取消 | 泡沫 | 使用自定义模板
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`expanded` | 用户已打开卡片的展开详细信息部分 | 无 | 否 | 可访问 | 是，除非重写默认模板

有关处理事件的详细信息，请参阅 [事件](../customize-components/events.md)。

## <a name="css-custom-properties"></a>CSS 自定义属性

该 `mgt-person-card` 组件定义以下 CSS 自定义属性。 

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
  --person-card-contact-link-color: #ff0000;
  --person-card-contact-link-hover-color: #00ff00;
  --person-card-show-more-color: #ff0000;
  --person-card-show-more-hover-color: #00ff00;
  --person-card-base-links-color: #ff0000;
  --person-card-base-links-hover-color: #00ff00;
  --person-card-tab-nav-color: #ff0000;
  --person-card-active-org-member-color: #ff0000;
  --person-card-nav-back-arrow-hover-color: #00ff00;
  --person-card-nav-back-arrow-color: #ff0000;
}
```

若要了解详细信息，请参阅 [样式组件](../customize-components/style.md)。

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

Person-Card控件使用以下 Microsoft Graph API 和权限。

| 配置 | 权限 | API | 节 |
| --- | ---------- | ------- | --------- |
| `personDetails` 使用用户的 `id` 但不带电子邮件的设置、 `userId` 设置或 `personQuery` 设置为 `me` | User.ReadBasic.All | [/users/{id}](/graph/api/user-list-people)、 [/users/{id}/photo/$value](/graph/api/profilephoto-get) | 默认 |
| `personQuery` 设置为不同于值的值 `me` | People.Read | [/me/people/？$search=](/graph/api/user-list-people) | 默认值 |
| `personQuery` 设置为不同于 `me` 并 `config.useContactApis` 设置为 `true` (默认)  | Contacts.Read | [/me/contacts/\*](/graph/api/user-list-contacts) | 默认值 |
| `showPresence` 设置为 `true` | Presence.Read.All | [/users/{id}/presence](/graph/api/presence-get) | 默认 |
| `sections.organization` 已启用 (默认)  | User.Read.All | [/users/{id}/manager](/graph/api/user-list-manager) | 组织 |
| `sections.organization.showWorksWith` 设置 (默认)  | People.Read.All | [/users/{id}/people](/graph/api/user-list-people) | 组织 |
| `sections.mailMessages` 已启用 (默认)  | Mail.ReadBasic | [/me/messages](/graph/api/user-list-messages) | 消息 |
| `sections.files` 已启用 (默认)  | Sites.Read.All | [/me/insights/shared](/graph/api/insights-list-shared) and [/me/insights/used](/graph/api/insights-list-used) | 文件 |
| `sections.profile` 已启用 (默认)  | User.Read.All | [/users/{id}/profile](/graph/api/profile-get?view=graph-rest-beta&preserve-view=true) | 个人资料 |

该 `MgtPersonCard` 类还公开一个 `getScopes` 静态方法，该方法返回基于全局人员卡配置的人员卡运行所需的范围数组。

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

const neededScopes = MgtPersonCard.getScopes();
```

## <a name="authentication"></a>身份验证

Person-Card控件使用 [身份验证文档](../providers/providers.md)中所述的全局身份验证提供程序。 

## <a name="cache"></a>缓存

> [!IMPORTANT]
> 该`mgt-person-card`组件从父`mgt-person`组件中检索基本人员数据，而无需调用 Microsoft Graph。 当单独使用时 `mgt-person-card` ，它将检索必要的数据本身并缓存它。 卡片部分中显示的数据是单独检索的，不会缓存。

|对象存储|缓存的数据|备注|
|---------|-----------|-------|
|`people`|人员信息|指定时 `personQuery` 使用，其值不同于 `me`|
|`photos`|人员照片|
|`presence`|人员的状态|已使用，何时 `showPresence` 设置为 `true`|
|`users`|人员的用户信息|指定时 `userId` 使用或 `personQuery` 设置为 `me`|

有关如何配置缓存的更多详细信息，请参阅[Caching](../customize-components/cache.md)。
