---
title: 处理 Microsoft 组件公开Graph Toolkit事件
description: 许多 Microsoft Graph Toolkit组件发出自定义事件。 将事件处理程序附加到这些事件后，你可以响应它们并控制应用的行为。
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: f20de269ed7f304f9c1d7198475b6fdb81b709c7
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082390"
---
# <a name="handle-events-exposed-by-microsoft-graph-toolkit-components"></a><span data-ttu-id="98112-104">处理 Microsoft 组件公开Graph Toolkit事件</span><span class="sxs-lookup"><span data-stu-id="98112-104">Handle events exposed by Microsoft Graph Toolkit components</span></span>

<span data-ttu-id="98112-105">许多 Microsoft Graph Toolkit组件发出自定义事件。</span><span class="sxs-lookup"><span data-stu-id="98112-105">Many Microsoft Graph Toolkit components emit custom events.</span></span> <span data-ttu-id="98112-106">将事件处理程序附加到这些事件后，你可以响应它们并控制应用的行为。</span><span class="sxs-lookup"><span data-stu-id="98112-106">Attaching event handlers to these events allows you to respond to them and control the behavior of your app.</span></span>

## <a name="discover-which-events-components-emit"></a><span data-ttu-id="98112-107">发现组件发出的事件</span><span class="sxs-lookup"><span data-stu-id="98112-107">Discover which events components emit</span></span>

<span data-ttu-id="98112-108">每个 Microsoft Graph Toolkit组件发出特定于其功能的不同事件。</span><span class="sxs-lookup"><span data-stu-id="98112-108">Each Microsoft Graph Toolkit component emits different events, specific to its functionality.</span></span> <span data-ttu-id="98112-109">若要查看特定组件发出的事件列表，请参阅 **该组件的文档** 的"事件"部分。</span><span class="sxs-lookup"><span data-stu-id="98112-109">To see the list of events emitted by the specific component, see the **Events** section of the documentation for that component.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="98112-110">某些事件（ `itemClick` 如文件列表组件中）仅在使用默认模板时发出。</span><span class="sxs-lookup"><span data-stu-id="98112-110">Some events, like `itemClick` in the File list component, are emitted only when using the default template.</span></span> <span data-ttu-id="98112-111">如果使用自定义模板，将覆盖负责发出事件的默认呈现。</span><span class="sxs-lookup"><span data-stu-id="98112-111">If you use a custom template, you overwrite the default rendering that is responsible for emitting the event.</span></span>

## <a name="add-event-handlers-to-events"></a><span data-ttu-id="98112-112">将事件处理程序添加到事件</span><span class="sxs-lookup"><span data-stu-id="98112-112">Add event handlers to events</span></span>

<span data-ttu-id="98112-113">Microsoft Graph Toolkit 使用标准 [`EventTarget.dispatchEvent()`](https://developer.mozilla.org/docs/Web/API/EventTarget/dispatchEvent) 函数在其组件中发出自定义事件。</span><span class="sxs-lookup"><span data-stu-id="98112-113">Microsoft Graph Toolkit uses the standard [`EventTarget.dispatchEvent()`](https://developer.mozilla.org/docs/Web/API/EventTarget/dispatchEvent) function to emit custom events in its components.</span></span> <span data-ttu-id="98112-114">若要将事件处理程序附加到工具包组件发出的自定义事件，请使用标准 [`EventTarget.addEventListener()`](https://developer.mozilla.org/docs/Web/API/EventTarget/addEventListener) 函数。</span><span class="sxs-lookup"><span data-stu-id="98112-114">To attach an event handler to a custom event emitted by a toolkit's component, use the standard [`EventTarget.addEventListener()`](https://developer.mozilla.org/docs/Web/API/EventTarget/addEventListener) function.</span></span>

<span data-ttu-id="98112-115">例如，若要处理 `itemClick` "文件"列表组件发出的事件，请向代码添加以下内容。</span><span class="sxs-lookup"><span data-stu-id="98112-115">For example, to handle the `itemClick` event emitted by the File list component, add the following to your code.</span></span>

```javascript
document.querySelector('mgt-file-list').addEventListener('itemClick' e => {
  // your event handler code goes here
});
```

### <a name="access-additional-information-exposed-by-the-event"></a><span data-ttu-id="98112-116">访问事件公开的其他信息</span><span class="sxs-lookup"><span data-stu-id="98112-116">Access additional information exposed by the event</span></span>

<span data-ttu-id="98112-117">Microsoft 报告发出的某些Graph Toolkit包含与事件相关的其他信息。</span><span class="sxs-lookup"><span data-stu-id="98112-117">Some events emitted by Microsoft Graph Toolkit contain additional information relevant to the event.</span></span> <span data-ttu-id="98112-118">例如， `itemClick` 由文件列表组件发出的事件包含有关在文件列表中单击的文件的信息。</span><span class="sxs-lookup"><span data-stu-id="98112-118">For example, the `itemClick` event, emitted by the File list component, contains information about the file that was clicked in the file list.</span></span> <span data-ttu-id="98112-119">若要了解特定事件是否包含其他信息，请参阅相应组件的文档的"事件"部分。</span><span class="sxs-lookup"><span data-stu-id="98112-119">To see if the particular event contains additional information, see the **Events** section of the documentation for the corresponding component.</span></span>

<span data-ttu-id="98112-120">可以通过传递到事件处理程序的对象的 属性访问事件公开的其他 `details` `event` 信息，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="98112-120">You can access the additional information exposed by an event through the `details` property of the `event` object passed into your event handler, as shown in the following example.</span></span>

```javascript
document.querySelector('mgt-file-list').addEventListener('itemClick', e => {
  const clickedFile = e.details;
});
```
