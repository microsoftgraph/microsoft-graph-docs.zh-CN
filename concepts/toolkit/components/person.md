---
title: Microsoft Graph 工具包中的 "人员" 组件
description: "\"人员\" 组件用于通过使用其照片、姓名和/或电子邮件地址显示人员或联系人。"
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: d944fa470b8d0f6baffb56d5cd997fe2a0bd7c91
ms.sourcegitcommit: 9f1e02ab486a2c3e0a128e5d36f46cebe4961581
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2020
ms.locfileid: "45024416"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的 "人员" 组件

"人员" 组件用于通过使用照片、姓名、电子邮件地址或任何其他人员详细信息来显示个人或联系人。

"人员" 组件还使用 "管理员-[卡片](./person-card.md)" 显示带有有关用户的其他信息的飞出卡片。 有关详细信息，请参阅 "[人员卡片](#person-card)" 部分。

## <a name="example"></a>示例

下面的示例显示使用组件的人员 `mgt-person` 。 您可以使用代码编辑器来查看[属性](#properties)如何更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[在 "dev" 中打开此示例](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a>设置人员详细信息

您可以使用三个属性来设置人员详细信息。 每个实例仅使用下列属性之一：

* `user-id` `userId` 通过使用其 ID 将属性或属性设置为从 Microsoft Graph 获取用户。

* 将 `person-query` 属性或 `personQuery` 属性设置为在 Microsoft Graph 中搜索给定人员。 它将选择第一个可用的人员并获取人员详细信息。 电子邮件最适用于确保查询的是正确的人员，但名称也有效。

* 将 `person-presence` 属性或 `personPresence` 属性设置为手动向用户头像添加状态标记。

* 将 `avatar-size` 属性或 `avatarSize` 属性设置为 `small` 或 `large` 以确定头像的大小。 这有助于将[正确的状态标记](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all)添加到头像。 你将需要选择下面显示的正确的相应 css 自定义属性，以进一步自定义头像大小。 默认情况下，此值设置为 `auto` 将自动决定如何基于属性呈现状态 `view` 。 `small`如果你的头像小于32，我们建议使用32。 

* 使用 `person-details` 属性或 `personDetails` 属性可手动设置人员详细信息，如下面的示例所示。


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  如果未提供图像，则将获取一个图像（如果可用）。

## <a name="properties"></a>属性

您可以使用多个属性来自定义组件。

| 属性       | 属性       | 说明                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| 用户 id         | userId         | 设置为用户 id，以从 Microsoft Graph 中获取该用户的详细信息和图像。|
| 人员-查询    | personQuery    | 设置为要在 Microsoft Graph 中搜索人员的人员的姓名或电子邮件，并提取第一个人员的详细信息和图像。|
| 人员-详细信息  | personDetails  | 设置为代表人员的对象。 使用来自人员、用户、联系人或组资源的对象。 |
| 人员-图像    | personImage    | 设置要为此人显示的图像。 |
| 人员-状态 | personPresence | 设置人员的状态。 |
| 提取-图像     | fetchImage     | 将标志设置为 `personImage` 根据用户提供的对象从 Microsoft Graph 自动获取 `personDetails` 。 |
| view            | view           | 设置以控制如何呈现该人员。 默认值为`avatar` <br /> `avatar`-仅显示头像 <br /> `oneline`-显示头像和第一行（ `displayName` 默认情况下） <br /> `twolines`-显示头像和两行文本（ `displayName` `mail` 默认情况下）|
| line1-属性  | line1Property  | 设置要用于第一行文本的 personDetails 的属性。 默认值为 `displayName`。|
| line2-属性  | line2Property  | 设置要用于第二行文本的 personDetails 的属性。 默认值为 `mail`。|
| 展示-状态   | showPresence   | 设置显示人员状态的标志-默认值为 `false` 。|
| 显示-名称       | showName       | **已弃用-使用 `view` 。**  设置用于显示人员显示名称的标志-默认为 `false` 。 |
| 显示-电子邮件      | showEmail      | **已弃用-使用 `view` 。** 设置用于显示个人电子邮件的标志-默认为 `false` 。        |

## <a name="css-custom-properties"></a>CSS 自定义属性

`mgt-person`组件定义以下 CSS 自定义属性。

```css
mgt-person {
  --avatar-size: 48px;
  --avatar-border: 0;
  --avatar-border-radius: 50%;
  --initials-color: white;
  --initials-background-color: magenta;
  --font-family: 'Segoe UI';
  --font-size: 14px;
  --font-weight: 500;
  --color: black;
  --presence-background-color: #ffffff;
  --text-transform: none;
  --line2-font-size: 12px;
  --line2-font-weight: 400;
  --line2-color: black;
  --line2-text-transform: none;
  --details-spacing: 12px;
}
```

若要了解详细信息，请参阅[样式组件](../style.md)。

## <a name="templates"></a>模板

`mgt-person`组件支持多个[模板](../templates.md)，这些模板允许您替换组件的某些部分。 若要指定模板，请在 `<template>` 组件内添加一个元素，并将 `data-type` 值设置为下列值之一：

| 数据类型 | 数据上下文 | 说明 |
| --------- | ------------ | ----------- |
| 装载 | 无 | 要在组件处于 laoding 状态时呈现的模板。 |
| 无数据 | 无 | 在没有人员图像或数据可用时要呈现的模板。 | 
|  默认值 | 人员：人员详细信息对象 <br> `personImage`：图像的 URL | 默认模板会将整个组件替换为您自己的组件。 |
| 人员-卡片 | 人员：人员详细信息对象 <br> `personImage`：图像的 URL | 用于更新在悬停或单击时显示的 "管理员-卡片" 的模板。 |

下面的示例定义了 "人员" 组件的模板。

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

`mgt-person`组件可显示为 `mgt-person-card` 悬停或单击。

### <a name="add-the-control-to-the-html-page"></a>将控件添加到 HTML 页面
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| 属性    |  属性     | 说明                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| 人员-卡片 | personCardInteraction | 一个枚举，用于确定激活浮出式面板-或的必需用户操作 `hover` `click` 。 默认值为`none` |


有关模板化、样式和属性的详细信息，请参阅[人员卡片组件](./person-card.md)。

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此控件使用以下 Microsoft Graph Api 和权限。

| 资源                                                                                                    | Permission     |
| ----------------------------------------------------------------------------------------------------------- | -------------------- |
| [/me](/graph/api/user-get?view=graph-rest-1.0)                              | User.Read          |
| [/me/photo/$value](/graph/api/profilephoto-get?view=graph-rest-beta)        | User.Read          |
| [/me/people/？ $search =](/graph/api/user-list-people?view=graph-rest-1.0)     | People.Read        |
| [/me/contacts/\*](/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | Contacts.Read      |
| [/users/{id}/photo/$value](/graph/api/user-list-people?view=graph-rest-1.0) | User.ReadBasic.All |
| [/me/presence](/graph/api/presence-get?view=graph-rest-beta)                | Presence.Read |
| [/users/{id}/presence](/graph/api/presence-get?view=graph-rest-beta)        | Presence.Read.All |

> **注意：** 若要访问 `*/photo/$value` 个人 Microsoft 帐户的资源，请使用 Microsoft Graph beta 终结点。

## <a name="authentication"></a>身份验证

该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序提取所需的数据。

## <a name="extend-for-more-control"></a>扩展以实现更多控制

对于更复杂的方案或真正的自定义 UX，此组件将公开几种 `protected render*` 用于在组件扩展中进行重写的方法。

| 方法 | 说明 |
| - | - |
| renderLoading | 呈现加载状态。 |
| renderNoData | 在没有图像或人员数据可用时呈现。 |
| renderAvatar | 呈现头像。 |
| renderDetails | 呈现人员详细信息部分。 |
