---
title: Microsoft Graph Toolkit React组件
description: Microsoft Graph Toolkit React组件 () 允许React开发人员将 `mgt-react` Microsoft Graph Toolkit用于React应用程序。
ms.localizationpriority: medium
author: nmetulev
ms.openlocfilehash: f81446c2b8a2938bd86057b1cbf5f33d583b49f9
ms.sourcegitcommit: f9e71d3b8a54a98c282ef49783babe5698300c06
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2021
ms.locfileid: "60793894"
---
# <a name="microsoft-graph-toolkit-react-components"></a>Microsoft Graph Toolkit React组件

Microsoft Graph Toolkit React组件 () 允许React开发人员将 `mgt-react` Microsoft Graph Toolkit用于React应用程序。 该库包装所有 Microsoft Graph Toolkit组件，并导出为React组件。

## <a name="what-components-can-i-use"></a>可以使用哪些组件？

该库从 Microsoft Graph Toolkit Web 组件自动生成，并且所有组件都作为React可用。

这些React的名称在 PascalCase 中，不包含 `Mgt` 前缀。 例如， `mgt-person` 组件可用为 `Person` ，组件 `mgt-people-picker` 为 `PeoplePicker` 。

## <a name="installation"></a>安装 

若要安装，请使用以下命令之一。

```bash
npm install @microsoft/mgt-react
```

或者

```bash
yarn add @microsoft/mgt-react
```

## <a name="usage"></a>用法

所有组件都可通过 npm 包使用 PascalCase 进行命名。 若要使用组件，请首先将其导入到顶部。

```tsx
import { Person } from '@microsoft/mgt-react';
```

现在，你可以将 `Person` JSX 中的任何位置用作常规React组件。

```tsx
<Person personQuery="me" />
```

所有属性和事件与组件文档中的定义完全一样。

例如，可以将属性 `personDetails` 设置为对象：

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

大多数 Microsoft Graph Toolkit 组件[都](../customize-components/templates.md)支持模板，并允许 `mgt-react` 你React模板。

例如，若要创建模板以用于在组件中呈现事件，请首先定义用于呈现 `mgt-agenda` 事件的组件：

```tsx
import { MgtTemplateProps } from '@microsoft/mgt-react';

const MyEvent = (props: MgtTemplateProps) => {
  const { event } = props.dataContext;
  return <div>
    {event.subject}<br />
    {event.attendees
      .map((attendee: any) => attendee.emailAddress.name)
      .join(', ')}
  </div>;
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

`template`属性允许您指定要覆盖的模板。 在这种情况下，将 `MyEvent` 针对每个事件重复组件，并且 `event` 对象将作为属性的一 `dataContext` 部分传递。

## <a name="see-also"></a>另请参阅

* [Microsoft Graph Toolkit入门React](./use-toolkit-with-react.md)
* [了解身份验证提供程序](../providers/providers.md)
