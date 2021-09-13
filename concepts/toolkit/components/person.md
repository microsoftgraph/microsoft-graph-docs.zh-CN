---
title: Microsoft 服务中的人员Graph Toolkit
description: 人员组件用于通过使用联系人的照片、姓名和/或电子邮件地址来显示此人或联系人。
ms.localizationpriority: medium
author: nmetulev
ms.openlocfilehash: 0cb5c1306a9cec54df6ab6a9d3cbd1aa0995a64a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59103842"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a>Microsoft 服务中的人员Graph Toolkit

人员组件用于通过使用其照片、姓名、电子邮件地址或其他任何人员详细信息来显示此人或联系人。

人员组件还使用 [mgt-person-card](./person-card.md) 显示包含有关用户的其他信息的飞出卡。 有关详细信息，请参阅人员 [卡片](#person-card) 部分。

## <a name="example"></a>示例

以下示例显示使用该组件 `mgt-person` 的人。 可以使用代码编辑器查看属性 [如何](#properties) 更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a>设置人员详细信息

可以使用三个属性来设置人员详细信息。 每个实例仅使用以下属性之一：

* 设置 `user-id` 属性或 `userId` 属性以使用用户的 ID 从 Microsoft Graph获取用户。

* 设置 `person-query` 属性或 `personQuery` 属性以搜索 microsoft Graph给定人员。 它将选择第一个可用的人员并提取该人员的详细信息。 电子邮件最适用于确保查询正确的人员，但名称也有效。

* 设置 `person-presence` 属性或 `personPresence` 属性以手动向个人头像添加状态锁屏提醒。

* 将 `avatar-size` 属性或 `avatarSize` 属性设置为 `small` 或 `large` 确定头像的大小。 这有助于向头像 [添加正确的状态](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) 锁屏提醒。 你将需要选择正确的相应的 css 自定义属性，如下所示以进一步自定义头像大小。 默认情况下，值设置为 ，该值将自动根据 属性 `auto` 决定如何呈现 `view` 状态。 如果你的头 `small` 像小于 32px x 32px，我们建议使用 。 

* 使用 `person-details` 属性 `personDetails` 或 属性手动设置人员详细信息，如以下示例所示。


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  如果未提供图像，将提取一个图像 (（如果) ）。

* 默认情况下，人员组件将仅请求标准 Microsoft Graph用户属性[集](/graph/api/user-get?&tabs=http#optional-query-parameters)。 为了请求其他属性，请将其声明为 的任何部分 `line(x)Property` 。 


## <a name="properties"></a>属性

可以使用多个属性来自定义组件。

| 属性       | 属性       | 说明                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| user-id         | userId         | 设置为用户 ID 以从 Microsoft Graph 获取该用户的详细信息和Graph。|
| person-query    | personQuery    | 设置为某人的姓名或电子邮件，以在 Microsoft Graph并提取第一个人的详细信息和图像。|
| person-details  | personDetails  | 设置为表示人员的对象。 使用来自人员、用户、联系人或组、资源的对象。 |
| fallback-details| fallbackDetails| 设置为一个对象，该对象表示在图中找不到用户/人员/联系人时的用户。
| person-image    | personImage    | 设置要向人员显示的图像。 |
| person-presence | personPresence | 为人员设置状态。 |
| fetch-image     | fetchImage     | 将标志设置为根据Graph自动从 Microsoft `personImage` `personDetails` 网站提取。 |
| 头像类型     | 头像类型     | 设置为 或 `initials` `photo` 呈现任一显示状态 - 默认为照片。 |
| view            | view           | 设置为控制呈现人员的方式。 默认值为 `avatar` <br /> `avatar` - 仅显示头像 <br /> `oneline` - 默认情况下显示头像 (`displayName` 一线)  <br /> `twolines` - 显示头像和两行文本 (`displayName` `mail` 默认显示) |
| line1-property  | line1Property  | 设置要用于第一行文本的 personDetails 的属性。 默认值为 `displayName`。|
| line2-property  | line2Property  | 设置要用于第二行文本的 personDetails 的属性。 默认值为 `mail`。|
| line3-property  | line3Property  | 设置要用于第三行文本的 personDetails 的属性。 默认值为 `jobTitle`。|
| show-presence   | showPresence   | 设置用于显示人员状态的标志 - 默认为 `false` 。|

## <a name="css-custom-properties"></a>CSS 自定义属性

组件 `mgt-person` 定义以下 CSS 自定义属性。

```css
mgt-person {
  --avatar-size: 48px;
  --avatar-border: 0;
  --avatar-border-radius: 50%;
  --avatar-cursor: default;
  
  --initials-color: white;
  --initials-background-color: magenta;

  --presence-background-color: #ffffff;
  --presence-icon-color: #ffffff;

  --font-family: 'Segoe UI';
  --font-size: 14px;
  --font-weight: 500;
  --color: black;
  --text-transform: none;

  --line2-font-size: 12px;
  --line2-font-weight: 400;
  --line2-color: black;
  --line2-text-transform: none;

  --line3-font-size: 12px;
  --line3-font-weight: 400;
  --line3-color: black;
  --line3-text-transform: none;

  --details-spacing: 12px;
}
```

若要了解更多信息，请参阅 [设置组件样式](../customize-components/style.md)。

## <a name="events"></a>活动

从组件中触发以下事件。

Event | 何时发出 | 自定义数据 | Cancelable | 气泡 | 使用自定义模板
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`line1clicked` | 单击第 1 行时触发 | `person`对象，可以是包含[](/graph/api/resources/user)[](/graph/api/resources/person)Graph URL 的其他属性的用户、人员[](/graph/api/resources/contact) `personImage` 或联系人 | 否 | 否 | 是，除非您覆盖默认模板
`line2clicked` | 单击第 2 行时触发 | `person`对象，可以是包含[](/graph/api/resources/user)[](/graph/api/resources/person)Graph URL 的其他属性的用户、人员[](/graph/api/resources/contact) `personImage` 或联系人 | 否 | 否 | 是，除非您覆盖默认模板
`line3clicked` | 单击第 3 行时触发 | `person`对象，可以是包含[](/graph/api/resources/user)[](/graph/api/resources/person)Graph URL 的其他属性的用户、人员[](/graph/api/resources/contact) `personImage` 或联系人 | 否 | 否 | 是，除非您覆盖默认模板

有关处理事件的信息，请参阅 [事件](../customize-components/events.md)。

## <a name="templates"></a>模板

组件 `mgt-person` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。 若要指定模板，请包含组件 `<template>` 中的元素，将值 `data-type` 设置为下列值之一：

| 数据类型 | 数据上下文 | 说明 |
| --------- | ------------ | ----------- |
| loading | 无 | 组件在加载状态时要呈现的模板。 |
| no-data | 无 | 在没有任何人员图像或数据可用时要呈现的模板。 | 
| default | person： The person details object <br> `personImage`：图像的 URL <br> `personPresence`：人员状态详细信息对象  | 默认模板将整个组件替换为你自己的组件。 |
| person-card | person： The person details object <br> `personImage`：图像的 URL | 用于更新悬停或单击时显示的 mgt-person-card 的模板。 |
| line1 | person： The person details object | 第一行人员元数据的模板。 |
| line2 | person： The person details object | 第二行人员元数据的模板。 |
| line3 | person： The person details object | 第三行人员元数据的模板。 |

下面的示例定义人员组件的模板。

```html
<!-- Retemplate the entire person component -->
<mgt-person>
  <template>
    <div data-if="personImage">
      <img src="{{personImage}}" />
    </div>
    <div data-else>
      {{person.displayName}}
    </div>
  </template>
</mgt-person>

<!-- Retemplate the line properties -->
<mgt-person view="threeLines">
  <template data-type="line1">
    <div>
      Hello, my name is: {{person.displayName}}
    </div>
  </template>
  <template data-type="line2">
    <div>
      Super cool
    </div>
  </template>
  <template data-type="line3">
    <div>
      Loves MGT
    </div>
  </template>
</mgt-person>
```

## <a name="person-card"></a>个人卡片

组件 `mgt-person` 可以在悬停 `mgt-person-card` 或单击时显示 。

### <a name="add-the-control-to-the-html-page"></a>将控件添加到 HTML 页面
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| 属性    |  属性     | 说明                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| person-card | personCardInteraction | 一个枚举，用于确定激活飞出面板或 所需的用户 `hover` 操作 `click` 。 默认值为 `none` |


有关模板、样式设置和属性详细信息，请参阅 Person Card [component](./person-card.md)。

## <a name="global-component-configuration"></a>全局组件配置

类 `MgtPerson` 公开一个 `config` 静态对象，该对象配置应用程序中的每个人组件。

以下示例演示如何使用 config 对象。

```ts
import { MgtPerson } from `@microsoft/mgt`;

MgtPerson.config.useContactApis = false;
```

以下属性在 config 对象上可用。

| 属性 | 说明 |
| ------------ | ------------- |
| useContactApis | `boolean`- 指示人员组件是否可以使用 Microsoft Graph联系人 API 搜索联系人详细信息和照片。 默认值为 `true`。  |

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此控件使用下列 Microsoft Graph API 和权限。

| 配置 | 权限 | API |
| ------------- | ---------- | --- |
| `personDetails` set without image， `fetchImage` set to ， set to ， `true` `avatarType` `photo` retrieved person is a contact and `useContactApis` set to `true` | Contacts.Read | [/me/contacts/\*](/graph/api/user-list-contacts) |
| `personDetails` set without image， `fetchImage` set to ， set to and person is not a contact or is set `true` `avatarType` `photo` `useContactApis` to `false` | User.ReadBasic.All | [/users/{id}/photo/$value](/graph/api/profilephoto-get) |
| `personDetails` set without image， `fetchImage` set to ， set to and user specified via `true` `avatarType` `photo` email | User.ReadBasic.All | [/users/{id}/photo/$value](/graph/api/profilephoto-get) |
| `personDetails` set without image， `fetchImage` set to ， set to and contact specified via `true` `avatarType` `photo` email | Contacts.Read | [/me/contacts/\*](/graph/api/user-list-contacts) |
| `userId` set | User.ReadBasic.All | [/users/{id}](/graph/api/user-list-people) |
| `personQuery` 设置为 `me` ， `avatarType` 设置为 `photo` | User.Read | [/me/photo/$value](/graph/api/profilephoto-get) |
| `personQuery` 设置为 `me` ， `avatarType` 并设置为其他内容 `photo` | User.Read | [/me](/graph/api/user-get) |
| `personQuery` 设置为值，而不是 `me` `useContactApis` 设置为 `true` | People.Read、User.ReadBasic.All、Contacts.Read | [/me/people/？$search=](/graph/api/user-list-people)、 [/users？$search=](/graph/api/user-list-people)、 [/me/contacts/ \* ](/graph/api/user-list-contacts) |
| `personQuery` 设置为值，而不是 `me` `useContactApis` 设置为 `false` | People.Read、User.ReadBasic.All | [/me/people/？$search=](/graph/api/user-list-people)、 [/users？$search=](/graph/api/user-list-people) |
| `showPresence` 设置为 `true` ， `personQuery` 设置为 `me` | Presence.Read | [/me/presence](/graph/api/presence-get) |
| `showPresence` 设置为 `true` 并 `personQuery` 设置为 `me` | Presence.Read.All | [/users/{id}/presence](/graph/api/presence-get) |
| `personCardInteraction` 设置为除 `PersonCardInteraction.none` | 查看 [个人卡片权限](/graph/toolkit/components/person-card#microsoft-graph-permissions) | 查看 [个人卡片 API 调用](/graph/toolkit/components/person-card#microsoft-graph-permissions) |

## <a name="authentication"></a>身份验证

该控件使用身份验证文档中介绍的全局身份验证提供程序[](../providers/providers.md)获取所需数据。

## <a name="cache"></a>缓存

|对象存储|缓存数据|备注|
|---------|-----------|-------|
|`photos`|人员照片|使用 时 `avatarType` ，将 设置为 `photo` `fetchImage` ，将 设置为 `true`|
|`presence`|人员状态|已使用， `showPresence` 设置为 `true`|
|`users`|人员的用户信息|

请参阅[Caching，](../customize-components/cache.md)了解有关如何配置缓存的更多详细信息。

## <a name="extend-for-more-control"></a>扩展以了解更多控件

对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展 `protected render*` 中替代的方法。

| 方法 | 说明 |
| - | - |
| renderLoading | 呈现加载状态。 |
| renderNoData | 当图像或人员数据不可用时呈现。 |
| renderAvatar | 呈现头像。 |
| renderDetails | 呈现人员详细信息部分。 |
