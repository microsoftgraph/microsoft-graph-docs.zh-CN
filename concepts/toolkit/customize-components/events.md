---
title: 处理 Microsoft 应用程序组件Graph Toolkit的事件
description: 许多 Microsoft Graph Toolkit组件发出自定义事件。 将事件处理程序附加到这些事件后，你可以响应它们并控制应用的行为。
ms.localizationpriority: medium
author: waldekmastykarz
ms.openlocfilehash: e58cda326bf939ad5d0850336e7d02739d372133
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129591"
---
# <a name="handle-events-exposed-by-microsoft-graph-toolkit-components"></a>处理 Microsoft 应用程序组件Graph Toolkit的事件

许多 Microsoft Graph Toolkit组件发出自定义事件。 将事件处理程序附加到这些事件后，你可以响应它们并控制应用的行为。

## <a name="discover-which-events-components-emit"></a>发现组件发出的事件

每个 Microsoft Graph Toolkit组件发出特定于其功能的不同事件。 若要查看特定组件发出的事件列表，请参阅 **该组件的文档** 的"事件"部分。

> [!IMPORTANT]
> 某些事件（ `itemClick` 如文件列表组件中）仅在使用默认模板时发出。 如果使用自定义模板，将覆盖负责发出事件的默认呈现。

## <a name="add-event-handlers-to-events"></a>将事件处理程序添加到事件

Microsoft Graph Toolkit 使用标准 [`EventTarget.dispatchEvent()`](https://developer.mozilla.org/docs/Web/API/EventTarget/dispatchEvent) 函数在其组件中发出自定义事件。 若要将事件处理程序附加到工具包组件发出的自定义事件，请使用标准 [`EventTarget.addEventListener()`](https://developer.mozilla.org/docs/Web/API/EventTarget/addEventListener) 函数。

例如，若要处理 `itemClick` "文件"列表组件发出的事件，请向代码添加以下内容。

```javascript
document.querySelector('mgt-file-list').addEventListener('itemClick' e => {
  // your event handler code goes here
});
```

### <a name="access-additional-information-exposed-by-the-event"></a>访问事件公开的其他信息

Microsoft 报告发出的某些Graph Toolkit包含与事件相关的其他信息。 例如， `itemClick` 由文件列表组件发出的事件包含有关在文件列表中单击的文件的信息。 若要了解特定事件是否包含其他信息，请参阅相应组件的文档的"事件"部分。

可以通过传递到事件处理程序的对象的 属性访问事件公开的其他 `details` `event` 信息，如以下示例所示。

```javascript
document.querySelector('mgt-file-list').addEventListener('itemClick', e => {
  const clickedFile = e.details;
});
```
