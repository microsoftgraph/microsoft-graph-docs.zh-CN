---
title: 微软待办 Microsoft Graph Toolkit
description: 利用微软待办组件，用户可以查看、添加、删除、完成或编辑任务。 它适用于 Microsoft 微软待办 中微软待办。
localization_priority: Normal
author: shweaver-MSFT
ms.openlocfilehash: 907d6d18380debb6e08d612d5f1d5bebec6746ec
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082018"
---
# <a name="to-do-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="2814c-104">微软待办 Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="2814c-104">To Do component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="2814c-105">微软待办 组件用于允许登录用户在 Microsoft Graph 中通过 微软待办 API 查看、添加、删除、完成和/或编辑 微软待办 中的任务。</span><span class="sxs-lookup"><span data-stu-id="2814c-105">The To Do component is used to enable the signed-in user to view, add, remove, complete, and/or edit tasks from Microsoft To Do using the To Do API in Microsoft Graph.</span></span>

## <a name="example"></a><span data-ttu-id="2814c-106">示例</span><span class="sxs-lookup"><span data-stu-id="2814c-106">Example</span></span>

<span data-ttu-id="2814c-107">以下示例显示登录用户使用组件微软待办任务 `mgt-todo` 。</span><span class="sxs-lookup"><span data-stu-id="2814c-107">The following example displays the signed-in user's Microsoft To Do tasks using the `mgt-todo` component.</span></span> <span data-ttu-id="2814c-108">可以使用代码编辑器查看 [属性如何](#properties) 更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="2814c-108">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-todo--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="2814c-109">在 mgt.dev 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="2814c-109">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-todo--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="2814c-110">属性</span><span class="sxs-lookup"><span data-stu-id="2814c-110">Properties</span></span>

<span data-ttu-id="2814c-111">可以使用下列属性和属性自定义组件。</span><span class="sxs-lookup"><span data-stu-id="2814c-111">You can use the following attributes and properties to customize the component.</span></span>

| <span data-ttu-id="2814c-112">属性</span><span class="sxs-lookup"><span data-stu-id="2814c-112">Attribute</span></span> | <span data-ttu-id="2814c-113">属性</span><span class="sxs-lookup"><span data-stu-id="2814c-113">Property</span></span> | <span data-ttu-id="2814c-114">说明</span><span class="sxs-lookup"><span data-stu-id="2814c-114">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="2814c-115">只读</span><span class="sxs-lookup"><span data-stu-id="2814c-115">read-only</span></span> | <span data-ttu-id="2814c-116">readOnly</span><span class="sxs-lookup"><span data-stu-id="2814c-116">readOnly</span></span> | <span data-ttu-id="2814c-117">一个布尔值，用于将任务界面设置为只读， (添加或删除任务) 。</span><span class="sxs-lookup"><span data-stu-id="2814c-117">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="2814c-118">默认值为“`false`”。</span><span class="sxs-lookup"><span data-stu-id="2814c-118">Default is `false`.</span></span> |
| <span data-ttu-id="2814c-119">hide-header</span><span class="sxs-lookup"><span data-stu-id="2814c-119">hide-header</span></span> | <span data-ttu-id="2814c-120">hideHeader</span><span class="sxs-lookup"><span data-stu-id="2814c-120">hideHeader</span></span> | <span data-ttu-id="2814c-121">显示或隐藏组件标头的布尔值。</span><span class="sxs-lookup"><span data-stu-id="2814c-121">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="2814c-122">默认值为“`false`”。</span><span class="sxs-lookup"><span data-stu-id="2814c-122">Default is `false`.</span></span> |
| <span data-ttu-id="2814c-123">hide-options</span><span class="sxs-lookup"><span data-stu-id="2814c-123">hide-options</span></span> | <span data-ttu-id="2814c-124">hideOptions</span><span class="sxs-lookup"><span data-stu-id="2814c-124">hideOptions</span></span> | <span data-ttu-id="2814c-125">用于显示或隐藏任务中的选项的布尔值。</span><span class="sxs-lookup"><span data-stu-id="2814c-125">A Boolean to show or hide the options in tasks.</span></span> <span data-ttu-id="2814c-126">默认值为“`false`”。</span><span class="sxs-lookup"><span data-stu-id="2814c-126">Default is `false`.</span></span>
| <span data-ttu-id="2814c-127">initial-id="folder_id"</span><span class="sxs-lookup"><span data-stu-id="2814c-127">initial-id="folder_id"</span></span> | <span data-ttu-id="2814c-128">initialId</span><span class="sxs-lookup"><span data-stu-id="2814c-128">initialId</span></span> | <span data-ttu-id="2814c-129">一个字符串 ID，用于将最初显示的文件夹设置为提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="2814c-129">A string ID to set the initially displayed folder to the provided ID.</span></span> |
| <span data-ttu-id="2814c-130">target-id="folder_id"</span><span class="sxs-lookup"><span data-stu-id="2814c-130">target-id="folder_id"</span></span>| <span data-ttu-id="2814c-131">targetId</span><span class="sxs-lookup"><span data-stu-id="2814c-131">targetId</span></span> | <span data-ttu-id="2814c-132">一个字符串 ID，用于将任务接口锁定为所提供的文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="2814c-132">A string ID to lock the tasks interface to the provided folder ID.</span></span> |
| <span data-ttu-id="2814c-133">不适用</span><span class="sxs-lookup"><span data-stu-id="2814c-133">N/A</span></span> | <span data-ttu-id="2814c-134">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="2814c-134">isNewTaskVisible</span></span>  | <span data-ttu-id="2814c-135">确定新任务视图在呈现时是否可见。</span><span class="sxs-lookup"><span data-stu-id="2814c-135">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="2814c-136">不适用</span><span class="sxs-lookup"><span data-stu-id="2814c-136">N/A</span></span> | <span data-ttu-id="2814c-137">taskFilter</span><span class="sxs-lookup"><span data-stu-id="2814c-137">taskFilter</span></span>  | <span data-ttu-id="2814c-138">可选函数，用于筛选向用户显示的任务。</span><span class="sxs-lookup"><span data-stu-id="2814c-138">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="2814c-139">以下示例只显示 ID 为 *12345* 的文件夹中的任务，并且不允许用户创建新任务。</span><span class="sxs-lookup"><span data-stu-id="2814c-139">The following example shows only tasks from the folder with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-todo read-only initial-id="12345"></mgt-todo>
```

## <a name="custom-css-variables"></a><span data-ttu-id="2814c-140">自定义 CSS 变量</span><span class="sxs-lookup"><span data-stu-id="2814c-140">Custom CSS variables</span></span>

<span data-ttu-id="2814c-141">组件 `mgt-todo` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="2814c-141">The `mgt-todo` component defines the following CSS custom properties.</span></span>

````css
mgt-todo {
  --tasks-background-color
  --tasks-header-padding
  --tasks-title-padding
  --tasks-plan-title-font-size
  --tasks-plan-title-padding

  --tasks-new-button-width
  --tasks-new-button-height
  --tasks-new-button-color
  --tasks-new-button-background
  --tasks-new-button-border
  --tasks-new-button-hover-background
  --tasks-new-button-active-background

  --task-margin
  --task-background
  --task-border
  --task-header-color
  --task-header-margin

  --task-new-margin
  --task-new-border
  --task-new-input-margin
  --task-new-input-padding
  --task-new-input-font-size
  --task-new-select-border

  --task-new-add-button-background
  --task-new-add-button-disabled-background
  --task-new-cancel-button-color

  --task-complete-background
  --task-complete-border

  --task-icon-alignment: flex-start (default) | center | flex-end
  --task-icon-background
  --task-icon-background-completed
  --task-icon-border
  --task-icon-border-completed
  --task-icon-border-radius
  --task-icon-color
  --task-icon-color-completed
}
````

<span data-ttu-id="2814c-142">若要了解更多信息，请参阅 [设置组件样式](https://docs.microsoft.com/graph/toolkit/style.md)。</span><span class="sxs-lookup"><span data-stu-id="2814c-142">To learn more, see [styling components](https://docs.microsoft.com/graph/toolkit/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="2814c-143">活动</span><span class="sxs-lookup"><span data-stu-id="2814c-143">Events</span></span>

<span data-ttu-id="2814c-144">从组件中触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="2814c-144">The following events are fired from the component.</span></span>

| <span data-ttu-id="2814c-145">事件</span><span class="sxs-lookup"><span data-stu-id="2814c-145">Event</span></span> | <span data-ttu-id="2814c-146">详情</span><span class="sxs-lookup"><span data-stu-id="2814c-146">Detail</span></span> | <span data-ttu-id="2814c-147">说明</span><span class="sxs-lookup"><span data-stu-id="2814c-147">Description</span></span> |
| --- | --- | --- |
| `taskAdded` | <span data-ttu-id="2814c-148">详细信息包含各自的 `task` 对象</span><span class="sxs-lookup"><span data-stu-id="2814c-148">The detail contains the respective `task` object</span></span> | <span data-ttu-id="2814c-149">新建任务后触发。</span><span class="sxs-lookup"><span data-stu-id="2814c-149">Fires when a new task has been created.</span></span> |
| `taskChanged` | <span data-ttu-id="2814c-150">详细信息包含各自的 `task` 对象</span><span class="sxs-lookup"><span data-stu-id="2814c-150">The detail contains the respective `task` object</span></span> | <span data-ttu-id="2814c-151">更改任务元数据（如标记已完成）时触发。</span><span class="sxs-lookup"><span data-stu-id="2814c-151">Fires when task metadata has been changed, such as marking completed.</span></span> |
| `taskClick` | <span data-ttu-id="2814c-152">详细信息包含各自的 `task` 对象</span><span class="sxs-lookup"><span data-stu-id="2814c-152">The detail contains the respective `task` object</span></span> | <span data-ttu-id="2814c-153">当用户单击或点击任务时触发。</span><span class="sxs-lookup"><span data-stu-id="2814c-153">Fires when the user clicks or taps on a task.</span></span> |
| `taskRemoved` | <span data-ttu-id="2814c-154">详细信息包含各自的 `task` 对象</span><span class="sxs-lookup"><span data-stu-id="2814c-154">The detail contains the respective `task` object</span></span> | <span data-ttu-id="2814c-155">删除现有任务后触发。</span><span class="sxs-lookup"><span data-stu-id="2814c-155">Fires when an existing task has been deleted.</span></span> |

<span data-ttu-id="2814c-156">有关处理事件的信息，请参阅 [事件](../customize-components/events.md)。</span><span class="sxs-lookup"><span data-stu-id="2814c-156">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="templates"></a><span data-ttu-id="2814c-157">模板</span><span class="sxs-lookup"><span data-stu-id="2814c-157">Templates</span></span>

<span data-ttu-id="2814c-158">组件 `tasks` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="2814c-158">The `tasks` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="2814c-159">若要指定模板，请包含组件 `<template>` 中的元素，将值 `data-type` 设置为以下值之一。</span><span class="sxs-lookup"><span data-stu-id="2814c-159">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="2814c-160">数据类型</span><span class="sxs-lookup"><span data-stu-id="2814c-160">Data type</span></span>     | <span data-ttu-id="2814c-161">数据上下文</span><span class="sxs-lookup"><span data-stu-id="2814c-161">Data context</span></span>              | <span data-ttu-id="2814c-162">说明</span><span class="sxs-lookup"><span data-stu-id="2814c-162">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="2814c-163">task</span><span class="sxs-lookup"><span data-stu-id="2814c-163">task</span></span>     | <span data-ttu-id="2814c-164">task： a to-do task object</span><span class="sxs-lookup"><span data-stu-id="2814c-164">task: a to-do task object</span></span> | <span data-ttu-id="2814c-165">替换整个默认任务。</span><span class="sxs-lookup"><span data-stu-id="2814c-165">Replaces the whole default task.</span></span> |
| <span data-ttu-id="2814c-166">task-details</span><span class="sxs-lookup"><span data-stu-id="2814c-166">task-details</span></span> | <span data-ttu-id="2814c-167">task： a to-do task object</span><span class="sxs-lookup"><span data-stu-id="2814c-167">task: a to-do task object</span></span> | <span data-ttu-id="2814c-168">模板将替换任务的详细信息部分。</span><span class="sxs-lookup"><span data-stu-id="2814c-168">Template replaces the details section of the task.</span></span> |

<span data-ttu-id="2814c-169">下面的示例定义任务组件的模板。</span><span class="sxs-lookup"><span data-stu-id="2814c-169">The following example defines a template for the tasks component.</span></span>

```html
<mgt-todo>
    <template data-type="task-details">
        <div>
            Importance Level: {{task.importance}}
        </div>
    </template>
</mgt-todo>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="2814c-170">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="2814c-170">Microsoft Graph permissions</span></span>

<span data-ttu-id="2814c-171">此控件使用下列 Microsoft Graph API 和权限。</span><span class="sxs-lookup"><span data-stu-id="2814c-171">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="2814c-172">配置</span><span class="sxs-lookup"><span data-stu-id="2814c-172">Configuration</span></span> | <span data-ttu-id="2814c-173">权限</span><span class="sxs-lookup"><span data-stu-id="2814c-173">Permission</span></span> | <span data-ttu-id="2814c-174">API</span><span class="sxs-lookup"><span data-stu-id="2814c-174">API</span></span> |
| ------------- | ---------- | --- |
| <span data-ttu-id="2814c-175">`targetId` set</span><span class="sxs-lookup"><span data-stu-id="2814c-175">`targetId` set</span></span> | <span data-ttu-id="2814c-176">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="2814c-176">Tasks.Read</span></span> | <span data-ttu-id="2814c-177">[/me/todo/lists/${listId}](/graph/api/todotasklist-get?view=graph-rest-1.0&tabs=http)、 [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks)</span><span class="sxs-lookup"><span data-stu-id="2814c-177">[/me/todo/lists/${listId}](/graph/api/todotasklist-get?view=graph-rest-1.0&tabs=http), [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks)</span></span> |
| <span data-ttu-id="2814c-178">`targetId` 未设置</span><span class="sxs-lookup"><span data-stu-id="2814c-178">`targetId` not set</span></span> | <span data-ttu-id="2814c-179">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="2814c-179">Tasks.Read</span></span> | <span data-ttu-id="2814c-180">[/me/todo/lists](/graph/api/todo-list-lists?view=graph-rest-1.0&tabs=http) [、/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks)</span><span class="sxs-lookup"><span data-stu-id="2814c-180">[/me/todo/lists](/graph/api/todo-list-lists?view=graph-rest-1.0&tabs=http), [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks)</span></span> |
| <span data-ttu-id="2814c-181">创建、更新或删除任务</span><span class="sxs-lookup"><span data-stu-id="2814c-181">create, update or delete task</span></span> | <span data-ttu-id="2814c-182">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2814c-182">Tasks.ReadWrite</span></span> | [<span data-ttu-id="2814c-183">/me/todo/lists/{todoTaskListId}/tasks/{taskId}</span><span class="sxs-lookup"><span data-stu-id="2814c-183">/me/todo/lists/{todoTaskListId}/tasks/{taskId}</span></span>](/graph/api/todotask-get) |

## <a name="authentication"></a><span data-ttu-id="2814c-184">身份验证</span><span class="sxs-lookup"><span data-stu-id="2814c-184">Authentication</span></span>

<span data-ttu-id="2814c-185">任务组件使用身份验证文档 中所述的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="2814c-185">The tasks component uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="2814c-186">缓存</span><span class="sxs-lookup"><span data-stu-id="2814c-186">Cache</span></span>

<span data-ttu-id="2814c-187">`mgt-todo`组件不缓存任何数据。</span><span class="sxs-lookup"><span data-stu-id="2814c-187">The `mgt-todo` component doesn't cache any data.</span></span>
