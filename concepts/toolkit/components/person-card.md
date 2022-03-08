---
title: Person-Card Microsoft Graph Toolkit 中的组件
description: Person-Card组件是显示与人员相关详细信息的组件。
ms.localizationpriority: medium
author: vogtn
ms.openlocfilehash: fcbb58a29405c5491db988a26b2c35a237aab346
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337381"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a>Person-Card Microsoft Graph Toolkit 中的组件

Person-Card组件是一个响应式组件，用于显示与人员相关的详细信息。 它通常用作组件上的一个飞出 `mgt-person` 区。

有关组件详细信息， `mgt-person` 请参阅 [mgt-person](./person.md)。

## <a name="example"></a>示例

以下示例演示了组件 `mgt-person-card` 与组件的使用 `mgt-person` 。 将鼠标悬停在人员上方以查看个人卡片，并使用代码编辑器查看属性 [如何更改组件](#properties) 的行为。
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card&source=docs" height="400"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-person-card--person-card&source=docs)


## <a name="global-component-configuration"></a>全局组件配置

类 `MgtPersonCard` 公开一个静态 `config` 对象，该对象配置应用程序中的所有人员卡片组件。 config 对象配置人员卡片使用哪些部分和哪些 API 从 Microsoft Graph。

默认情况下，所有节和 API 都已启用。 以下示例演示如何使用 config 对象禁用节或 API。

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.useContactApis = false;
MgtPersonCard.config.sections.profile = false;
```

以下属性在 config 对象上可用。

| 属性 | 说明 |
| ------------ | ------------- |
| useContactApis | `boolean`- 指示人员卡片组件是否可以使用 Microsoft Graph API 搜索联系人详细信息和照片。 默认值为 `true`。  |
| sections | `object` - 配置人员卡片中显示的部分。  |

### <a name="person-card-sections"></a>个人卡片分区

The person card contains several configurable sections for displaying person details：
* 联系人 - 联系人信息，如电子邮件、电话、位置、位置等。
* 组织 - 具有经理、直接下属和相关人员的组织图片。
* 邮件 - 具有当前登录用户的最相关的电子邮件。
* 文件 - 与当前登录用户最相关的共享文件。
* 配置文件 - 配置文件信息，如项目、技能、语言等。

默认情况下会加载节，但可通过 object 属性全局禁用 `MgtPersonCard.config.sections` 节。 以下属性可用。

| 属性 | 说明 |
| ------------ | ------------- |
| 组织 | `boolean` - 指示是否显示个人卡片组织部分。 默认值为 `true`。  |
| mailMessages | `boolean` - 指示是否显示"人员卡片邮件"部分。 默认值为 `true`。  |
| files | `boolean` - 指示是否显示人员卡片文件部分。 默认值为 `true`。  |
| 个人资料 | `boolean` - 指示是否显示个人卡片配置文件部分。 默认值为 `true`。  |

若要禁用分区，只需在应用 `false` 初始化代码中将 属性设置为 ：
```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.sections.profile = false;
```

## <a name="setup-for-teams-integrations"></a>用于集成Teams安装程序

该Person-Card组件允许用户联系目标人员，包括通过Teams聊天。 如果在选项卡应用中`microsoftTeamsLib`使用组件Teams，你可以确保组件深度直接链接到聊天，而不是通过设置 中的 打开浏览器窗口`TeamsProvider`。

如果Person-Card无法检测到 Teams lib，该组件将尝试打开 Teams Web 客户端。

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = microsoftTeams;
```

有关提供程序详细信息，`TeamsProvider`请参阅Microsoft Teams[提供程序](../providers/teams.md)。

## <a name="properties"></a>属性

默认情况下，组件 `mgt-person` 会向组件传递人员 `mgt-person-card` 详细信息。 但是，在模板化`mgt-person``mgt-person-card`组件或将组件用作独立组件时，可以使用这些属性来更改这一点。

| 属性         | 类型                     | 说明                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| person-details | MicrosoftGraph.User <br> MicrosoftGraph.Person <br> MicrosoftGraph.Contact | 由 Microsoft Graph定义的 Person 对象，包含与用户相关的详细信息。 |
| person-image   | string                    | 与卡片中显示的人员相关的图像 uri。                                   |
| inherit-details   | 无。                  | 允许个人卡片为组件演练 `mgt-person` 父树以使用相同 `person-details` 和 `person-image` 数据。                      |
| user-id | string | 允许开发人员提供用户 ID 以检索显示在个人卡片组件上的数据 |
| person-query | string | 允许开发人员提供人员查询以检索显示在个人卡片组件上的数据 |
| person-card | string | 指定悬停 `person-card` 或单击组件时组件可以显示为弹出 `mgt-person` 式卡片。 允许的值是 或 `hover` `click`。


## <a name="templates"></a>模板

该Person-Card组件 [使用允许您](../customize-components/templates.md) 添加或替换组件部分的模板。 若要指定模板，请包含 `<template>` 组件内的元素，将 `data-type` 值设置为以下值之一。

| 数据类型 | 数据上下文 | 说明 |
| - | - | - |
| no-data | 空 | 没有可用数据时所使用的模板。
| default | `person`：人员详细信息对象 <br> `personImage`：图像的 URL | 默认模板将整个组件替换为你自己的组件。 |
| person-details | `person`：人员详细信息对象 | 用于呈现人员卡片顶部的模板。 |
| additional-details | `person`：人员详细信息对象 <br> `personImage`：图像的 URL | 用于将自定义内容添加到其他详细信息容器的模板。 |

例如，可以使用模板 `mgt-person` 自定义附加到组件的组件，使用模板在卡片中添加其他详细信息。 

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

从组件中触发以下事件。

事件 | 何时发出 | 自定义数据 | Cancelable | 气泡 | 使用自定义模板
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`expanded` | 用户已打开卡片的展开详细信息部分 | 无 | 否 | 是 | 是，除非您覆盖默认模板

有关处理事件的信息，请参阅 [事件](../customize-components/events.md)。

## <a name="css-custom-properties"></a>CSS 自定义属性

组件 `mgt-person-card` 定义以下 CSS 自定义属性。 

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

若要了解更多信息，请参阅 [设置组件样式](../customize-components/style.md)。

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

该Person-Card控件使用下列 Microsoft Graph API 和权限。

| 配置 | 权限 | API | 节 |
| --- | ---------- | ------- | --------- |
| `personDetails`使用用户的 但`id`不带电子邮件进行设置，`userId`或设置为`personQuery``me` | User.ReadBasic.All | [/users/{id}](/graph/api/user-list-people)、 [/users/{id}/photo/$value](/graph/api/profilephoto-get) | 默认 |
| `personQuery` 设置为不同于 `me` | People.Read | [/me/people/？$search=](/graph/api/user-list-people) | 默认值 |
| `personQuery`设置为不同于 默认值`me``config.useContactApis`的值，`true` (设置为)  | Contacts.Read | [/me/contacts/\*](/graph/api/user-list-contacts) | 默认 |
| `showPresence` 设置为 `true` | Presence.Read.All | [/users/{id}/presence](/graph/api/presence-get) | 默认值 |
| `sections.organization` 已启用 (默认)  | User.Read.All | [/users/{id}/manager](/graph/api/user-list-manager) | 组织 |
| `sections.organization.showWorksWith` 将 (设置为默认)  | People.Read.All | [/users/{id}/people](/graph/api/user-list-people) | 组织 |
| `sections.mailMessages` 已启用 (默认)  | Mail.ReadBasic | [/me/messages](/graph/api/user-list-messages) | 消息 |
| `sections.files` 已启用 (默认)  | Sites.Read.All | [/me/insights/shared](/graph/api/insights-list-shared) 和 [/me/insights/used](/graph/api/insights-list-used) | 文件 |

该类 `MgtPersonCard` 还公开了 `getScopes` 一个静态方法，该方法返回人员卡片根据全局人员卡片配置运行所需的作用域数组。

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

const neededScopes = MgtPersonCard.getScopes();
```

## <a name="authentication"></a>身份验证

身份验证Person-Card使用身份验证文档中介绍的全局 [身份验证提供程序](../providers/providers.md)。 

## <a name="cache"></a>缓存

> [!IMPORTANT]
> 该`mgt-person-card`组件从父组件检索基本人员数据`mgt-person`，而无需调用 Microsoft Graph。 单独 `mgt-person-card` 使用时，它将检索必要的数据本身并缓存它。 卡片分区中显示的数据是单独检索的，不会进行缓存。

|对象存储|缓存数据|备注|
|---------|-----------|-------|
|`people`|人员信息|指定 时 `personQuery` 使用，其值不同于 `me`|
|`photos`|人员照片|
|`presence`|人员状态|已使用，设置为`showPresence``true`|
|`users`|人员的用户信息|指定 或 `userId` 将 设置为 `personQuery` 时使用 `me`|

请参阅 [Caching](../customize-components/cache.md)，了解有关如何配置缓存的更多详细信息。
