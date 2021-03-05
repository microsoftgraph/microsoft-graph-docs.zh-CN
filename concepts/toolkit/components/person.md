---
title: Microsoft Graph 服务中的人员Toolkit
description: 人员组件用于使用联系人的照片、姓名和/或电子邮件地址显示此人或联系人。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 9ac8eebfaa4d95ccd935414329ab1dd145839dd2
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475056"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 服务中的人员Toolkit

人员组件用于通过使用联系人的照片、姓名、电子邮件地址或任何其他人员详细信息来显示此人或联系人。

人员组件还使用 [mgt-person-card](./person-card.md) 显示包含有关用户的其他信息的飞出卡。 有关详细信息，请参阅" [人员卡片"](#person-card) 部分。

## <a name="example"></a>示例

以下示例显示使用该组件 `mgt-person` 的人。 可以使用代码编辑器查看属性 [如何](#properties) 更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a>设置人员详细信息

可以使用三个属性来设置人员详细信息。 每个实例仅使用以下属性之一：

* 设置 `user-id` 属性或 `userId` 属性以使用用户的 ID 从 Microsoft Graph 提取用户。

* 设置 `person-query` 属性或 `personQuery` 属性以搜索 Microsoft Graph 中给定人员。 它将选择第一个可用的人员并提取人员详细信息。 电子邮件最好确保查询正确的人员，但名称也有效。

* 设置 `person-presence` 属性以手动向个人头像添加状态 `personPresence` 锁屏提醒。

* 将 `avatar-size` 属性设置为 `avatarSize` 或确定头像 `small` `large` 的大小。 这有助于向头像 [添加正确的状态锁](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) 屏提醒。 你需要选择正确的相应的 css 自定义属性，如下所示以进一步自定义头像大小。 默认情况下，该值设置为 `auto` ，该值将自动决定如何根据属性呈现 `view` 状态。 如果你的头 `small` 像小于 32px x 32px，我们建议使用。 

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
| user-id         | userId         | 设置为用户 ID 以从 Microsoft Graph 提取该用户的详细信息和图像。|
| person-query    | personQuery    | 设置为人员的名称或电子邮件，以在 Microsoft Graph 中搜索人员并提取第一个人的详细信息和图像。|
| person-details  | personDetails  | 设置为表示人员的对象。 使用来自人员、用户、联系人或组、资源的对象。 |
| 回退详细信息| fallbackDetails| 设置为在图中未找到用户/人员/联系人时代表人员的对象。
| person-image    | personImage    | 设置要向人员显示的图像。 |
| person-presence | personPresence | 设置人员状态。 |
| fetch-image     | fetchImage     | 将标志设置为 `personImage` 根据用户提供的对象自动从 Microsoft Graph `personDetails` 提取。 |
| 头像类型     | 头像类型     | 设置为 `initials` 或 `photo` 呈现任一显示状态 - 默认为照片。 |
| view            | view           | 设置为控制人员呈现方式。 默认值为 `avatar` <br /> `avatar` - 仅显示头像 <br /> `oneline` - 默认情况下显示头像 (`displayName` 第一)  <br /> `twolines` - 显示头像和两行文本 (`displayName` `mail` 默认显示) |
| line1-property  | line1Property  | 设置要用于第一行文本的 personDetails 的属性。 默认值为“`displayName`”。|
| line2-property  | line2Property  | 设置要用于第二行文本的 personDetails 的属性。 默认值为“`mail`”。|
| line3-property  | line3Property  | 设置要用于第三行文本的 personDetails 的属性。 默认值为“`jobTitle`”。|
| show-presence   | showPresence   | 设置用于显示人员状态的标志 - 默认值为 `false` 。|

## <a name="css-custom-properties"></a>CSS 自定义属性

组件 `mgt-person` 定义以下 CSS 自定义属性。

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

## <a name="events"></a>活动

从组件中触发以下事件。

| 事件 | 详情 | 说明 |
| --- | --- | --- |
| line1clicked | 详细信息包含各自的 `person` 对象 | 单击第 1 行时触发。 |
| line2clicked | 详细信息包含各自的 `person` 对象 | 单击第 2 行时触发。 |
| line3clicked | 详细信息包含各自的 `person` 对象 | 单击第 3 行时触发。 |

## <a name="templates"></a>模板

组件 `mgt-person` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。 若要指定模板，请包含 `<template>` 组件中的元素，将值设置为下列 `data-type` 值之一：

| 数据类型 | 数据上下文 | 说明 |
| --------- | ------------ | ----------- |
| loading | 无 | 组件在加载状态时要呈现的模板。 |
| no-data | 无 | 在无人员图像或数据可用时呈现的模板。 | 
| 默认 | person：人员详细信息对象 <br> `personImage`：图像的 URL | 默认模板将整个组件替换为你自己的组件。 |
| person-card | person：人员详细信息对象 <br> `personImage`：图像的 URL | 用于更新悬停或单击时显示的 mgt-person-card 的模板。 |
| line1 | person：人员详细信息对象 | 第一行人员元数据的模板。 |
| line2 | person：人员详细信息对象 | 第二行人员元数据的模板。 |
| line3 | person：人员详细信息对象 | 第三行人员元数据的模板。 |

以下示例为人员组件定义模板。

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

组件 `mgt-person` 可以显示 `mgt-person-card` 鼠标悬停或单击。

### <a name="add-the-control-to-the-html-page"></a>将控件添加到 HTML 页面
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| 属性    |  属性     | 说明                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| person-card | personCardInteraction | 一个枚举，用于确定激活飞出面板或所需的用户 `hover` 操作 `click` 。 默认值为 `none` |


有关模板、样式设置和属性详细信息，请参阅 Person Card [组件](./person-card.md)。

## <a name="global-component-configuration"></a>全局组件配置

该类 `MgtPerson` 公开配置应用程序中所有 `config` 人员组件的静态对象。

以下示例演示如何使用 config 对象。

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

对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展 `protected render*` 中替代的方法。

| 方法 | 说明 |
| - | - |
| renderLoading | 呈现加载状态。 |
| renderNoData | 当图像或人员数据不可用时呈现。 |
| renderAvatar | 呈现头像。 |
| renderDetails | 呈现人员详细信息部分。 |
