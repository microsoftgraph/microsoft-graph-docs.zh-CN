---
title: Microsoft Graph Toolkit React 组件
description: Microsoft Graph Toolkit React组件 (`mgt-react`) 允许React开发人员在应用程序Graph Toolkit Microsoft React。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 4dff722faf3f61b4ed9832c2389b674d9bf1a444
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589000"
---
# <a name="microsoft-graph-toolkit-react-components"></a>Microsoft Graph Toolkit React 组件

Microsoft Graph Toolkit React组件 (`mgt-react`) 允许React开发人员在应用程序Graph Toolkit Microsoft React。 该库包装所有 Microsoft Graph Toolkit组件，并导出为React组件。

## <a name="what-components-can-i-use"></a>可以使用哪些组件？

该库从 Microsoft Graph Toolkit Web 组件自动生成，并且所有组件都作为React组件。

这些React的名称在 PascalCase 中，不包含`Mgt`前缀。 例如，组件 `mgt-person` 可用为 ， `Person`组件 `mgt-people-picker` 为 `PeoplePicker`。

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

大多数 Microsoft Graph Toolkit 组件[都](../customize-components/templates.md)`mgt-react`支持模板，并允许你React模板。

例如，若要创建模板以用于在 `mgt-agenda` 组件中呈现事件，请首先定义用于呈现事件的组件：

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

然后，使用它作为封装组件的子项，然后将模板属性设置为 `event`。

```tsx
import { Agenda } from '@microsoft/mgt-react';

const App = (props) => {
  return <Agenda>
    <MyEvent template="event">
  </Agenda>
}
```

属性 `template` 允许您指定要覆盖的模板。 在这种情况下，将 `MyEvent` 针对每个事件重复 `event` 组件，并且对象将作为属性的一部分 `dataContext` 传递。

## <a name="see-also"></a>另请参阅

* [开始 Microsoft Graph Toolkit中React](./use-toolkit-with-react.md)
* [了解身份验证提供程序](../providers/providers.md)
