---
title: Microsoft Graph 工具包中的个人卡片组件
description: "\"个人卡片\" 组件是显示与某个人相关的详细信息的组件。"
localization_priority: Normal
author: vogtn
ms.openlocfilehash: f4d8c975fe91d91658f512cea708ee104d4fd906
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275855"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的个人卡片组件

个人卡片组件是一个响应性组件，用于显示与人员相关的更多信息。 它通常用作`mgt-person`组件上的浮出控件。

有关`mgt-person`组件的详细信息，请参阅 "[管理员文档](./person.md)"。
  
## <a name="example"></a>示例

```html
<mgt-person-card person-details="{personObject}" person-image="imgUrl"></mgt-person-card>
```

## <a name="properties"></a>属性

组件使用 Microsoft Graph 提供有关用户的其他详细信息。 若要定义用户，必须使用的`mgt-person`**人员查询**属性。

| 属性         | type                     | 说明                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| 人员-详细信息 | MicrosoftGraph <br> MicrosoftGraph <br> MicrosoftGraph。联系人 | 由 Microsoft Graph 定义的 Person 对象，包含与用户相关的详细信息。 |
| 人员-图像   | png/jpg/svg                    | 与卡片中显示的人员相关的图像。                                   |



## <a name="templates"></a>模板

人员卡片组件使用允许您添加或替换部分组件的[模板](../templates.md)。 若要指定模板，请在`<template>`组件内添加一个元素，并将`data-type`值设置为下列值之一。

| 数据类型 | 数据上下文 | 说明 |
| --- | --- | --- |
| 设置 | 人员：人员详细信息对象 <br> personImage：图像的 URL | 默认模板会将整个组件替换为您自己的组件。 |
| 其他详细信息 | 人员：人员详细信息对象 <br> personImage：图像的 URL | 用于向卡片中添加其他内容的模板。 |

例如，可以使用模板自定义附加到`mgt-person`组件的组件和模板，以在卡片中添加其他详细信息。 

```html
    <mgt-person person-query="me" show-name show-email person-card="hover">
      <template data-type="person-card">
        <mgt-person-card person-details="{{person}}" 
            person-image="{{personImage}}">
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

`mgt-person-card`组件定义以下 CSS 自定义属性。

```css
mgt-person-card {
  --font-size: 14px;
  --font-weight: 600;
  --height: '100%';
  --background-color: transparent;
}
```

若要了解详细信息，请参阅[样式组件](../style.md)。

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此组件使用 "[人员" 组件](./person.md)显示用户并继承所有权限。 

## <a name="authentication"></a>身份验证

个人卡片控件使用[身份验证文档](./../providers.md)中所述的全局身份验证提供程序。 
