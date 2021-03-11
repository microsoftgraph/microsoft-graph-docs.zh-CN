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
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a>Person-Card Microsoft Graph Toolkit

Person-Card组件是一个响应式组件，用于显示与人员相关的详细信息。 它通常用作组件上的飞 `mgt-person` 出。

有关组件详细信息 `mgt-person` ，请参阅[mgt-person。](./person.md)

## <a name="example"></a>示例

以下示例显示组件 `mgt-person-card` 与组件的 `mgt-person` 使用。 将鼠标悬停在人员上方以查看人员卡片，并使用代码编辑器查看 [属性](#properties) 如何更改组件的行为。
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card-hover&source=docs" height="400"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-person-card--person-card-hover&source=docs)


## <a name="global-component-configuration"></a>全局组件配置

该类 `MgtPersonCard` 公开一个 `config` 静态对象，该对象配置应用程序中的所有人员卡片组件。 config 对象配置人员卡片使用哪些部分和哪些 API 从 Microsoft Graph 获取有关用户的详细信息。

默认情况下，启用所有节和 API。 以下示例演示如何使用 config 对象禁用节或 API。

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.useContactApis = false;
MgtPersonCard.config.sections.profile = false;
```

以下属性在 config 对象上可用。

| 属性 | 说明 |
| ------------ | ------------- |
| useContactApis | `boolean` - 指示人员卡片组件是否可以使用 Microsoft Graph 联系人 API 搜索联系人详细信息和照片。 默认值为 `true`。  |
| sections | `object` - 配置人员卡片中显示的部分。  |

### <a name="person-card-sections"></a>人员卡片部分

人员卡片包含用于显示人员详细信息的几个可配置部分：
* 联系人 - 联系人信息，如电子邮件、电话、位置、位置等。
* 组织 - 具有经理、直接下属和相关人员的组织图形。
* 邮件 - 与当前登录用户最相关的电子邮件。
* 文件 - 与当前登录用户最相关的共享文件。
* 配置文件 - 配置文件信息，如项目、技能、语言等。

默认情况下加载节，但可通过对象属性全局禁用 `MgtPersonCard.config.sections` 节。 以下属性可用。

| 属性 | 说明 |
| ------------ | ------------- |
| 组织 | `boolean` - 指示是否显示"人员卡片组织"部分。 默认值为 `true`。  |
| mailMessages | `boolean` - 指示是否显示"人员卡片消息"部分。 默认值为 `true`。  |
| files | `boolean` - 指示是否显示"人员卡片文件"部分。 默认值为 `true`。  |
| 个人资料 | `boolean` - 指示是否显示个人卡片配置文件部分。 默认值为 `true`。  |

若要禁用节，只需在应用初始化代码中 `false` 将属性设置为：
```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.sections.profile = false;
```

## <a name="setup-for-teams-integrations"></a>Teams 集成设置

此Person-Card组件允许用户联系目标人员，包括通过 Teams 聊天。 如果使用 Teams 选项卡应用内的组件，你可以确保组件深层链接到聊天，而不是通过设置中的打开浏览器 `microsoftTeamsLib` 窗口 `TeamsProvider` 。

如果Person-Card组件无法检测 Teams 库，则组件将改为尝试打开 Teams Web 客户端。

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = microsoftTeams;
```

有关提供程序详细信息 `TeamsProvider` ，请参阅 Microsoft [Teams 提供程序](../providers/teams.md)。

## <a name="properties"></a>属性

默认情况下， `mgt-person` 组件将人员详细信息传递到 `mgt-person-card` 组件。 但是，在模板化组件或将组件用作独立组件时，可以使用这些属性 `mgt-person` `mgt-person-card` 来更改这一点。

| 属性         | 类型                     | 说明                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| person-details | MicrosoftGraph.User <br> MicrosoftGraph.Person <br> MicrosoftGraph.Contact | Microsoft Graph 定义的 Person 对象，包含与用户相关的详细信息。 |
| person-image   | string                    | 与卡片中显示的人员相关的图像 uri。                                   |
| inherit-details   | 无。                  | 允许个人卡片为组件演练父树 `mgt-person` 以使用相同的 `person-details` `person-image` 数据和数据。                      |
| user-id | string | 允许开发人员提供用户 ID 以检索人员卡片组件上显示的数据 |
| person-query | string | 允许开发人员提供人员查询以检索人员卡片组件上显示的数据 |


## <a name="templates"></a>模板

该Person-Card组件使用模板，允许您[](../customize-components/templates.md)添加或替换组件部分。 若要指定模板，请包含组件中的元素，将值设置为 `<template>` `data-type` 下列值之一。

| 数据类型 | 数据上下文 | 说明 |
| - | - | - |
| no-data | 空 | 没有可用数据时使用的模板。
| 默认 | `person`：人员详细信息对象 <br> `personImage`：图像的 URL | 默认模板将整个组件替换为你自己的组件。 |
| person-details | `person`：人员详细信息对象 | 用于呈现人员卡片顶部部分的模板。 |
| additional-details | `person`：人员详细信息对象 <br> `personImage`：图像的 URL | 用于将自定义内容添加到其他详细信息容器的模板。 |

例如，可以使用模板自定义附加到组件的组件，使用模板在卡片中添加 `mgt-person` 其他详细信息。 

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

若要了解更多信息，请参阅 [样式组件](../customize-components/style.md)。

## <a name="microsoft-graph-apis-and-permissions"></a>Microsoft Graph API 和权限

该Person-Card控件使用以下 Microsoft Graph API 和权限。

| 资源 | 权限 | 分区 |
| - | - | - |
| [/me](/graph/api/user-get) | User.Read | 默认值 |
| [/me/photo/$value](/graph/api/profilephoto-get) | User.Read | 默认值 |
| [/me/people/？$search=](/graph/api/user-list-people) | People.Read | 默认值 |
| [/me/contacts/\*](/graph/api/user-list-contacts) | Contacts.Read | 默认值 |
| [/users/{id}](/graph/api/user-list-people) | User.ReadBasic.All | 默认值 |
| [/users/{id}/photo/$value](/graph/api/profilephoto-get) | User.ReadBasic.All | 默认值 |
| [/me/presence](/graph/api/presence-get) | Presence.Read | 默认值 |
| [/users/{id}/presence](/graph/api/presence-get) | Presence.Read.All | 默认值 |
| [/users/{id}/manager](/graph/api/user-list-manager) | User.Read.All | 组织 |
| [/users/{id}/directReports](/graph/api/user-list-directreports) | User.Read.All | 组织 |
| [/users/{id}/people](/graph/api/user-list-people) | People.Read.All | 组织 |
| [/me/messages](/graph/api/user-list-messages) | Mail.ReadBasic | 邮件 |
| [/me/insights/shared](/graph/api/insights-list-shared) 和 [/me/insights/used](/graph/api/insights-list-used) | Sites.Read.All | 文件 |
| [/users/{id}/profile](/graph/api/profile-get) | User.Read.All | 个人资料 |

该类还公开了一个静态方法，该方法返回根据全局人员卡片配置运行人员卡片所需的一 `MgtPersonCard` `getScopes` 组作用域。

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

const neededScopes = MgtPersonCard.getScopes();
```

## <a name="authentication"></a>身份验证

该Person-Card使用身份验证文档中介绍的全局 [身份验证提供程序](../providers/providers.md)。 
