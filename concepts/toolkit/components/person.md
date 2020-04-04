---
title: Microsoft Graph 工具包中的 "人员" 组件
description: "\"人员\" 组件用于通过使用其照片、姓名和/或电子邮件地址显示人员或联系人。"
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 53cd4d8bb7a2bb23a3c54924ee07b4843e7fc503
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144280"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的 "人员" 组件

"人员" 组件用于通过使用其照片、姓名和/或电子邮件地址显示人员或联系人。

"人员" 组件还使用 "管理员-[卡片](./person-card.md)" 显示带有有关用户的其他信息的飞出卡片。 有关详细信息，请参阅 "[人员卡片](#person-card)" 部分。

## <a name="example"></a>示例

下面的示例显示使用组件的`mgt-person`人员。 您可以使用代码编辑器来查看[属性](#properties)如何更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[在 "dev" 中打开此示例](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a>设置人员详细信息

您可以使用三个属性来设置人员详细信息。 每个实例仅使用下列属性之一：

* 通过使用`user-id`其 ID `userId`将属性或属性设置为从 Microsoft Graph 获取用户。

* 将`person-query`属性或`personQuery`属性设置为在 Microsoft Graph 中搜索给定人员。 它将选择第一个可用的人员并获取人员详细信息。 电子邮件最适用于确保查询的是正确的人员，但名称也有效。

* 将`person-details`属性或`personDetails`属性设置为手动设置人员详细信息，如下面的示例所示。


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        email: 'nikola@contoso.com',
        image: 'url'
    }
    ```

  如果未提供图像，则将获取一个图像（如果可用）。

## <a name="properties"></a>属性

您可以使用多个属性来自定义组件。

| 属性    | 属性   | 说明                                                   |
| -----------  | ---------- | ------------------------------------------------------------- |
| 显示-名称    | showName   | 设置用于显示人员显示名称的标志-默认`false`为。 |
| 显示-电子邮件   | showEmail  | 设置用于显示个人电子邮件的标志- `false`默认为。        |

## <a name="css-custom-properties"></a>CSS 自定义属性

`mgt-person`组件定义以下 CSS 自定义属性。

```css
mgt-person {
  --avatar-size-s: 24px;
  --avatar-size: 48px; // avatar size when both name and email are shown
  --avatar-font-size--s: 16px;
  --avatar-font-size: 32px; // font-size when both name and email are shown
  --avatar-border: 0;
  --initials-color: white;
  --initials-background-color: magenta;
  --font-size: 12px;
  --font-weight: 500;
  --color: black;
  --email-font-size: 12px;
  --email-color: black;
}
```

若要了解详细信息，请参阅[样式组件](../style.md)。

## <a name="templates"></a>模板

组件支持多个[模板](../templates.md)，这些模板允许您替换组件的某些部分。 `mgt-person` 若要指定模板，请在`<template>`组件内添加一个元素，并`data-type`将值设置为下列值之一：

| 数据类型 | 数据上下文 | 说明 |
| --------- | ------------ | ----------- |
| 装载 | 无 | 要在组件处于 laoding 状态时呈现的模板。 |
| 无数据 | 无 | 在没有人员图像或数据可用时要呈现的模板。 | 
| 设置 | 人员：人员详细信息对象 <br> `personImage`：图像的 URL | 默认模板会将整个组件替换为您自己的组件。 |
| 人员-卡片 | 人员：人员详细信息对象 <br> `personImage`：图像的 URL | 用于更新在悬停或单击时显示的 "管理员-卡片" 的模板。 |

下面的示例定义了 "人员" 组件的模板。

```html
<mgt-person>
  <template>
    <div data-if="person.image">
      <img src="{{person.image}}" />
    </div>
    <div data-else>
      {{person.displayName}}
    </div>
  </template>
</mgt-person>
```

## <a name="person-card"></a>个人卡片

`mgt-person`组件可显示为`mgt-person-card`悬停或单击。

### <a name="add-the-control-to-the-html-page"></a>将控件添加到 HTML 页面
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| 属性    |  属性     | 说明                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| 人员-卡片 | personCardInteraction | 一个枚举，用于确定激活浮出式面板- `hover`或`click`的必需用户操作。 默认值为`none` |


有关模板化、样式和属性的详细信息，请参阅[人员卡片组件](./person-card.md)。

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此控件使用以下 Microsoft Graph Api 和权限。

| 资源                                                                                                    | 权限     |
| ----------------------------------------------------------------------------------------------------------- | -------------------- |
| [/me](/graph/api/user-get?view=graph-rest-1.0)                              | User.Read          |
| [/me/photo/$value](/graph/api/profilephoto-get?view=graph-rest-beta)        | User.Read          |
| [/me/people/？ $search =](/graph/api/user-list-people?view=graph-rest-1.0)     | People.Read        |
| [/me/contacts/\*](/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | Contacts.Read      |
| [/users/{id}/photo/$value](/graph/api/user-list-people?view=graph-rest-1.0) | User.ReadBasic.All |

> **注意：** 若要访问`*/photo/$value`个人 Microsoft 帐户的资源，请使用 Microsoft Graph beta 终结点。

## <a name="authentication"></a>身份验证

该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序提取所需的数据。

## <a name="extend-for-more-control"></a>扩展以实现更多控制

对于更复杂的方案或真正的自定义 UX，此组件`protected render*`将公开几种用于在组件扩展中进行重写的方法。

| 方法 | 说明 |
| - | - |
| renderLoading | 呈现加载状态。 |
| renderImage | 呈现图像部件。 |
| renderNoData | 在没有图像或人员数据可用时呈现。 |
| renderDetails | 呈现人员详细信息部分。 |
| renderEmail | 呈现人员详细信息的电子邮件子部分。 |
| renderName | 呈现人员详细信息的子部分的名称。 |
