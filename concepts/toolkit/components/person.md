---
title: Microsoft Graph 工具包中的 "人员" 组件
description: "\"人员\" 组件用于通过使用其照片、姓名和/或电子邮件地址显示人员或联系人。"
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b4664cf545c858dbb2d49ad5191ab7cf5118092e
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275701"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的 "人员" 组件

"人员" 组件用于通过使用其照片、姓名和/或电子邮件地址显示人员或联系人。 

"人员" 组件还使用 "管理员-[卡片](./person-card.md)" 显示带有有关用户的其他信息的飞出卡片。 有关详细信息，请参阅 "[人员卡片](#person-card)" 部分。

## <a name="example"></a>示例

[jsfiddle 示例](https://jsfiddle.net/metulev/0jkzfr42/)

### <a name="add-the-control-to-the-html-page"></a>将控件添加到 HTML 页面
```html
<mgt-person person-query=""></mgt-person>
```

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

## <a name="changing-how-the-component-looks"></a>更改组件的外观

您可以使用多个属性来自定义组件。

| 属性    | 属性    | 说明                                                   |
| ----------- | ------------ | ------------------------------------------------------------- |
| showName  | 显示-名称  | 设置用于显示人员显示名称的标志-默认`false`为。 |
| showEmail | 显示-电子邮件 | 设置用于显示个人电子邮件的标志- `false`默认为。        |

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

| 数据类型     | 数据上下文              | 说明                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| 设置     | 人员：人员详细信息对象 <br> `personImage`：图像的 URL | 默认模板会将整个组件替换为您自己的组件。 |
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

| 属性     | 属性     | 说明                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| personCard | 人员-卡片 | 一个枚举，用于确定激活浮出式面板- `hover`或`click`的必需用户操作。 默认值为`none` |


有关模板化、样式和属性的详细信息，请参阅[人员卡片组件](./person-card.md)。

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此控件使用以下 Microsoft Graph Api 和权限。

| 资源                                                                                                    | 权限     |
| ----------------------------------------------------------------------------------------------------------- | -------------------- |
| [/me](https://docs.microsoft.com/en-us/graph/api/user-get?view=graph-rest-1.0)                              | User.Read          |
| [/me/photo/$value](https://docs.microsoft.com/en-us/graph/api/profilephoto-get?view=graph-rest-beta)        | User.Read          |
| [/me/people/？ $search =](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0)     | People.Read        |
| [/me/contacts/*](https://docs.microsoft.com/en-us/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | Contacts.Read      |
| [/users/{id}/photo/$value](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | User.ReadBasic.All |

> **注意：** 若要访问`*/photo/$value`个人 Microsoft 帐户的资源，请使用 Microsoft Graph beta 终结点。

## <a name="authentication"></a>身份验证

该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序提取所需的数据。
