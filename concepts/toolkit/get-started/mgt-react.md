---
title: Microsoft Graph Toolkit React 组件
description: Microsoft Graph Toolkit React 组件 () React 开发人员可以使用 `mgt-react` Microsoft Graph Toolkit React 应用程序。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 6781a894e451e2c4751f151beddcacf4e0cdb608
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658232"
---
# <a name="microsoft-graph-toolkit-react-components"></a>Microsoft Graph Toolkit React 组件

Microsoft Graph Toolkit React 组件 () React 开发人员可以使用 `mgt-react` Microsoft Graph Toolkit React 应用程序。 库包装所有 Microsoft Graph Toolkit组件，并导出为 React 组件。

## <a name="what-components-can-i-use"></a>我可以使用哪些组件？

库从 Microsoft Graph Toolkit Web 组件自动生成，并且所有组件都作为 React 组件提供。

React 组件的名称在 PascalCase 中，不包含 `Mgt` 前缀。 例如， `mgt-person` 组件可用为 ，组件 `Person` `mgt-people-picker` 可用为 `PeoplePicker` 。

## <a name="installation"></a>安装 

若要安装，请使用以下命令之一。

```bash
npm install @microsoft/mgt-react
```

或

```bash
yarn add @microsoft/mgt-react
```

## <a name="usage"></a>用法

所有组件均通过 npm 包提供，并且使用 PascalCase 命名。 若要使用组件，请首先将其导入顶部。

```tsx
import { Person } from '@microsoft/mgt-react';
```

现在，你可以将 `Person` JSX 中的任何位置用作常规 React 组件。

```tsx
<Person personQuery="me" />
```

所有属性和事件与组件文档中的定义完全一样。

例如，可以将该属性 `personDetails` 设置为对象：

```jsx
const App = (props) => {
  const personDetails = {
    displayName: 'Bill Gates',
  };

  return <Person personDetails={personDetails}></Person>;
};
```

或者，注册事件处理程序：

```jsx
import { PeoplePicker, People } from '@microsoft/mgt-react';

const App = (props) => {
  const [people, setPeople] = useState([]);

  const handleSelectionChanged = (e) => {
    setPeople(e.target.selectedPeople);
  };

  return
    <div>
      <PeoplePicker selectionChanged={handleSelectionChanged} />
      Selected People: <People people={people} />
    </div>;
};
```

## <a name="templates"></a>模板

大多数 Microsoft Graph Toolkit组件 [都支持模板](../customize-components/templates.md) ，并允许你 `mgt-react` 使用 React 编写模板。

例如，若要创建用于呈现组件中的事件的模板，请首先定义用于呈现 `mgt-agenda` 事件的组件：

```tsx
import { MgtTemplateProps } from '@microsoft/mgt-react';

const MyEvent = (props: MgtTemplateProps) => {
  const { event } = props.dataContext;
  return <div>{event.subject}</div>;
};
```

然后，使用它作为封装组件的子项，然后将模板属性设置为 `event` 。

```tsx
import { Agenda } from '@microsoft/mgt-react';

const App = (props) => {
  return <Agenda>
    <MyEvent template="event">
  </Agenda>
}
```

属性 `template` 允许你指定要覆盖的模板。 在这种情况下，将针对每个事件重复组件，并且对象作为属性的一 `MyEvent` `event` `dataContext` 部分传递。

## <a name="see-also"></a>另请参阅

* [在 React 中开始使用 Microsoft Graph Toolkit](./use-toolkit-with-react.md)
* [了解身份验证提供程序](../providers/providers.md)
