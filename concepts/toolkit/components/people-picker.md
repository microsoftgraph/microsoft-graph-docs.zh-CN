---
title: 人员-选取器组件
description: 您可以使用 "人员-选取器 web 组件" 搜索指定数量的人员，并通过 Microsoft Graph 呈现结果列表。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 2a0680a70ddfd5410e82911e5280c0b1a7e7dcaf
ms.sourcegitcommit: 3e7769ad097e9c34233fa5fea83afa23c34e14a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822793"
---
# <a name="people-picker-component"></a>人员-选取器组件

您可以使用`mgt-people-picker` web 组件搜索指定数量的人员，并通过 Microsoft Graph 呈现结果列表。 默认情况下，组件将搜索所有人员;您还可以定义组属性以进一步筛选结果。

如果要显示的用户数超过此`show-max`值，则不会在搜索列表中显示所有返回的人员数。

## <a name="example"></a>示例

[jsfiddle 示例](https://jsfiddle.net/metulev/jdv38fg0/)

```html
<mgt-people-picker></mgt-people-picker>
```

![组织-人员-选取器](./images/mgt-people-picker-image.png)

## <a name="properties"></a>属性

默认情况下， `mgt-people-picker`组件从`/me/people`终结点提取事件。 使用以下属性来更改此行为。

| 属性 | 属性 | 说明                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| showMax  | show-max  | 一个整数值，指示要显示的最大用户数。 默认值为6。                                                                                             |
| people   | people    | 获取或设置组件呈现的人员列表的人员数组。 使用此属性可访问组件加载的人员。 设置此值可加载自己的人员。 |
| group    | group     | 一个 string 值，属于 Microsoft Graph 定义的组，用于进一步筛选搜索结果。                                                                            |

示例如下。

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="css-custom-properties"></a>CSS 自定义属性

`mgt-people-picker`组件定义以下 CSS 自定义属性。

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此组件使用以下 Microsoft Graph Api 和权限。

| API                                                                                                              | 权限  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [/me/people](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0)                    | People.Read |
| [/groups/\${groupId}/members](https://docs.microsoft.com/en-us/graph/api/group-list-members?view=graph-rest-1.0) | People.Read |

## <a name="authentication"></a>身份验证

该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。
