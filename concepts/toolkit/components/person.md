---
title: Microsoft Graph 服务中的人员Toolkit
description: 人员组件用于通过使用个人或联系人的照片、姓名和/或电子邮件地址来显示此人或联系人。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: cfe5f6b97c35c2704def8c4879522268cc8cc91e
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660037"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 服务中的人员Toolkit

人员组件用于通过使用个人或联系人的照片、姓名、电子邮件地址或任何其他人员详细信息来显示此人或联系人。

人员组件还使用 [mgt-person-card](./person-card.md) 显示包含有关用户的其他信息的飞出卡。 有关详细信息，请参阅" [人员卡片"](#person-card) 部分。

## <a name="example"></a>示例

以下示例显示使用该组件 `mgt-person` 的人。 可以使用代码编辑器查看属性 [如何](#properties) 更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a>设置人员详细信息

可以使用三个属性来设置人员详细信息。 每个实例仅使用以下属性之一：

* 设置 `user-id` 属性或 `userId` 属性以使用用户的 ID 从 Microsoft Graph 提取用户。

* 设置 `person-query` 属性或 `personQuery` 属性以搜索 Microsoft Graph 中给定人员。 它将选择第一个可用的人员并提取人员详细信息。 电子邮件最适用于确保查询正确的人员，但名称也有效。

* 设置 `person-presence` 属性或 `personPresence` 属性以手动向个人头像添加状态锁屏提醒。

* 将 `avatar-size` 属性或 `avatarSize` 属性设置为 `small` 或 `large` 确定头像的大小。 这有助于向头像 [添加正确的状态](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) 锁屏提醒。 你需要选择正确的相应的 css 自定义属性，如下所示以进一步自定义头像大小。 默认情况下，该值设置为 `auto` ，该值将自动决定如何根据属性呈现 `view` 状态。 如果你的头像小于 `small` 32px x 32px，我们建议使用。 

* 使用 `person-details` 属性或 `personDetails` 属性手动设置人员详细信息，如以下示例所示。


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  如果未提供图像，将提取一个 (（如果) ）。

## <a name="properties"></a>属性

可以使用多个属性来自定义组件。

| 属性       | 属性       | 说明                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| user-id         | userId         | 设置为用户 ID，从 Microsoft Graph 获取该用户的详细信息和图像。|
| person-query    | personQuery    | 设置为人员的名称或电子邮件，以在 Microsoft Graph 中搜索某人并提取第一个人的详细信息和图像。|
| person-details  | personDetails  | 设置为表示人员的对象。 使用来自人员、用户、联系人或组、资源的对象。 |
| person-image    | personImage    | 设置要为人员显示的图像。 |
| person-presence | personPresence | 为人员设置状态。 |
| fetch-image     | fetchImage     | 设置标志以 `personImage` 根据用户提供的对象自动从 Microsoft Graph `personDetails` 提取。 |
| view            | view           | 设置为控制人员呈现方式。 默认值为 `avatar` <br /> `avatar` - 仅显示头像 <br /> `oneline` - 默认显示头像 (`displayName` 第一)  <br /> `twolines` - 显示头像和两行文本 (`displayName` `mail` 默认显示) |
| line1-property  | line1Property  | 设置用于第一行文本的 personDetails 的属性。 默认值为“`displayName`”。|
| line2-property  | line2Property  | 设置用于第二行文本的 personDetails 的属性。 默认值为“`mail`”。|
| line3-property  | line3Property  | 设置用于第三行文本的 personDetails 的属性。 默认值为“`jobTitle`”。|
| show-presence   | showPresence   | 设置用于显示人员状态的标志 - 默认值为 `false` 。|

## <a name="css-custom-properties"></a>CSS 自定义属性

该 `mgt-person` 组件定义以下 CSS 自定义属性。

```css
mgt-person {
  --avatar-size: 48px;
  --avatar-border: 0;
  --avatar-border-radius: 50%;
  
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

若要了解更多信息，请参阅 [样式组件](../customize-components/style.md)。

## <a name="templates"></a>模板

该 `mgt-person` 组件支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。 若要指定模板，请包含组件 `<template>` 中的元素，将值设置为下列值 `data-type` 之一：

| 数据类型 | 数据上下文 | 说明 |
| --------- | ------------ | ----------- |
| loading | 无 | 组件在加载状态时要呈现的模板。 |
| no-data | 无 | 在无人员图像或数据可用时要呈现的模板。 | 
| default | person： The person details object <br> `personImage`：图像的 URL | 默认模板将整个组件替换为你自己的组件。 |
| person-card | person： The person details object <br> `personImage`：图像的 URL | 用于更新悬停或单击时显示的 mgt-person-card 的模板。 |

以下示例为人员组件定义模板。

```html
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
```

## <a name="person-card"></a>个人卡片

组件 `mgt-person` 可以在悬 `mgt-person-card` 停或单击时显示。

### <a name="add-the-control-to-the-html-page"></a>将控件添加到 HTML 页面
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| 属性    |  属性     | 说明                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| person-card | personCardInteraction | 一个枚举，用于确定激活飞出面板所需的用户操作 - `hover` 或 `click` 。 默认值为 `none` |


有关模板、样式设置和属性详细信息，请参阅 Person Card [组件](./person-card.md)。

## <a name="global-component-configuration"></a>全局组件配置

该类 `MgtPerson` 公开配置应用程序中所有人员 `config` 组件的静态对象。

下面的示例演示如何使用 config 对象。

```ts
import { MgtPerson } from `@microsoft/mgt`;

MgtPerson.config.useContactApis = false;
```

以下属性在 config 对象上可用。

| 属性 | 说明 |
| ------------ | ------------- |
| useContactApis | `boolean` - 指示人员组件是否可以使用 Microsoft Graph 个人联系人 API 搜索联系人详细信息和照片。 默认值为 `true`。  |

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此控件使用以下 Microsoft Graph API 和权限。

| 资源 | 权限     |
| -| - |
| [/me](/graph/api/user-get)                              | User.Read          |
| [/me/photo/$value](/graph/api/profilephoto-get)        | User.Read          |
| [/me/people/？$search=](/graph/api/user-list-people)     | People.Read        |
| [/me/contacts/\*](/graph/api/user-list-contacts&tabs=cs) | Contacts.Read      |
| [/users/{id}/photo/$value](/graph/api/user-list-people) | User.ReadBasic.All |
| [/me/presence](/graph/api/presence-get)                | Presence.Read |
| [/users/{id}/presence](/graph/api/presence-get)        | Presence.Read.All |

## <a name="authentication"></a>身份验证

该控件使用身份验证文档中介绍的全局身份验证提供程序[](../providers/providers.md)获取所需数据。

## <a name="extend-for-more-control"></a>扩展以更多控制

对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展中 `protected render*` 替代的方法。

| 方法 | 说明 |
| - | - |
| renderLoading | 呈现加载状态。 |
| renderNoData | 当图像或人员数据不可用时呈现。 |
| renderAvatar | 呈现头像。 |
| renderDetails | 呈现人员详细信息部分。 |
