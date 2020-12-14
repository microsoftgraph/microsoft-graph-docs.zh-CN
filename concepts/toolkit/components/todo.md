---
title: Microsoft Graph 中的"执行"组件Toolkit
description: 通过"执行"组件，用户可以查看、添加、删除、完成或编辑 todo 任务。 它适用于 Microsoft To-Do 中的任何任务。
localization_priority: Normal
author: shweaver-MSFT
ms.openlocfilehash: 1a00d045da55dc14da47770b0e56522590f4b5bc
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659163"
---
# <a name="to-do-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="8bc74-104">Microsoft Graph 中的"执行"组件Toolkit</span><span class="sxs-lookup"><span data-stu-id="8bc74-104">To Do component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="8bc74-105">"要执行"组件用于使登录用户可以使用 Microsoft Graph 中的"要执行"API 查看、添加、删除、完成和/或编辑 Microsoft To Do 中的任务。</span><span class="sxs-lookup"><span data-stu-id="8bc74-105">The To Do component is used to enable the signed-in user to view, add, remove, complete, and/or edit tasks from Microsoft To Do using the To Do API in Microsoft Graph.</span></span>

## <a name="example"></a><span data-ttu-id="8bc74-106">示例</span><span class="sxs-lookup"><span data-stu-id="8bc74-106">Example</span></span>

<span data-ttu-id="8bc74-107">以下示例使用组件显示登录用户的 Microsoft To Do `mgt-todo` 任务。</span><span class="sxs-lookup"><span data-stu-id="8bc74-107">The following example displays the signed-in user's Microsoft To Do tasks using the `mgt-todo` component.</span></span> <span data-ttu-id="8bc74-108">可以使用代码编辑器查看属性 [如何](#properties) 更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="8bc74-108">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-todo--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="8bc74-109">在 mgt.dev 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="8bc74-109">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-todo--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="8bc74-110">属性</span><span class="sxs-lookup"><span data-stu-id="8bc74-110">Properties</span></span>

<span data-ttu-id="8bc74-111">可以使用下列属性和属性自定义组件。</span><span class="sxs-lookup"><span data-stu-id="8bc74-111">You can use the following attributes and properties to customize the component.</span></span>

| <span data-ttu-id="8bc74-112">属性</span><span class="sxs-lookup"><span data-stu-id="8bc74-112">Attribute</span></span> | <span data-ttu-id="8bc74-113">属性</span><span class="sxs-lookup"><span data-stu-id="8bc74-113">Property</span></span> | <span data-ttu-id="8bc74-114">说明</span><span class="sxs-lookup"><span data-stu-id="8bc74-114">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="8bc74-115">只读</span><span class="sxs-lookup"><span data-stu-id="8bc74-115">read-only</span></span> | <span data-ttu-id="8bc74-116">readOnly</span><span class="sxs-lookup"><span data-stu-id="8bc74-116">readOnly</span></span> | <span data-ttu-id="8bc74-117">一个布尔值，用于将任务界面设置为只读， (添加或删除任务) 。</span><span class="sxs-lookup"><span data-stu-id="8bc74-117">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="8bc74-118">默认值为“`false`”。</span><span class="sxs-lookup"><span data-stu-id="8bc74-118">Default is `false`.</span></span> |
| <span data-ttu-id="8bc74-119">hide-header</span><span class="sxs-lookup"><span data-stu-id="8bc74-119">hide-header</span></span> | <span data-ttu-id="8bc74-120">hideHeader</span><span class="sxs-lookup"><span data-stu-id="8bc74-120">hideHeader</span></span> | <span data-ttu-id="8bc74-121">显示或隐藏组件标头的布尔值。</span><span class="sxs-lookup"><span data-stu-id="8bc74-121">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="8bc74-122">默认值为“`false`”。</span><span class="sxs-lookup"><span data-stu-id="8bc74-122">Default is `false`.</span></span> |
| <span data-ttu-id="8bc74-123">hide-options</span><span class="sxs-lookup"><span data-stu-id="8bc74-123">hide-options</span></span> | <span data-ttu-id="8bc74-124">hideOptions</span><span class="sxs-lookup"><span data-stu-id="8bc74-124">hideOptions</span></span> | <span data-ttu-id="8bc74-125">用于显示或隐藏任务中的选项的布尔值。</span><span class="sxs-lookup"><span data-stu-id="8bc74-125">A Boolean to show or hide the options in tasks.</span></span> <span data-ttu-id="8bc74-126">默认值为“`false`”。</span><span class="sxs-lookup"><span data-stu-id="8bc74-126">Default is `false`.</span></span>
| <span data-ttu-id="8bc74-127">initial-id="folder_id"</span><span class="sxs-lookup"><span data-stu-id="8bc74-127">initial-id="folder_id"</span></span> | <span data-ttu-id="8bc74-128">initialId</span><span class="sxs-lookup"><span data-stu-id="8bc74-128">initialId</span></span> | <span data-ttu-id="8bc74-129">一个字符串 ID，用于将最初显示的文件夹设置为所提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="8bc74-129">A string ID to set the initially displayed folder to the provided ID.</span></span> |
| <span data-ttu-id="8bc74-130">target-id="folder_id"</span><span class="sxs-lookup"><span data-stu-id="8bc74-130">target-id="folder_id"</span></span>| <span data-ttu-id="8bc74-131">targetId</span><span class="sxs-lookup"><span data-stu-id="8bc74-131">targetId</span></span> | <span data-ttu-id="8bc74-132">用于将任务接口锁定为提供的文件夹 ID 的字符串 ID。</span><span class="sxs-lookup"><span data-stu-id="8bc74-132">A string ID to lock the tasks interface to the provided folder ID.</span></span> |
| <span data-ttu-id="8bc74-133">不适用</span><span class="sxs-lookup"><span data-stu-id="8bc74-133">N/A</span></span> | <span data-ttu-id="8bc74-134">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="8bc74-134">isNewTaskVisible</span></span>  | <span data-ttu-id="8bc74-135">确定新任务视图在呈现时是否可见。</span><span class="sxs-lookup"><span data-stu-id="8bc74-135">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="8bc74-136">不适用</span><span class="sxs-lookup"><span data-stu-id="8bc74-136">N/A</span></span> | <span data-ttu-id="8bc74-137">taskFilter</span><span class="sxs-lookup"><span data-stu-id="8bc74-137">taskFilter</span></span>  | <span data-ttu-id="8bc74-138">可选函数，用于筛选向用户显示的任务。</span><span class="sxs-lookup"><span data-stu-id="8bc74-138">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="8bc74-139">以下示例只显示 ID 为 *12345* 的文件夹中的任务，并且不允许用户创建新任务。</span><span class="sxs-lookup"><span data-stu-id="8bc74-139">The following example shows only tasks from the folder with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-todo read-only initial-id="12345"></mgt-todo>
```

## <a name="custom-css-variables"></a><span data-ttu-id="8bc74-140">自定义 CSS 变量</span><span class="sxs-lookup"><span data-stu-id="8bc74-140">Custom CSS variables</span></span>

<span data-ttu-id="8bc74-141">该 `mgt-todo` 组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="8bc74-141">The `mgt-todo` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="8bc74-142">若要了解更多信息，请参阅 [样式组件](https://docs.microsoft.com/graph/toolkit/style.md)。</span><span class="sxs-lookup"><span data-stu-id="8bc74-142">To learn more, see [styling components](https://docs.microsoft.com/graph/toolkit/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="8bc74-143">活动</span><span class="sxs-lookup"><span data-stu-id="8bc74-143">Events</span></span>

<span data-ttu-id="8bc74-144">从组件中触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="8bc74-144">The following events are fired from the component.</span></span>

| <span data-ttu-id="8bc74-145">事件</span><span class="sxs-lookup"><span data-stu-id="8bc74-145">Event</span></span> | <span data-ttu-id="8bc74-146">详情</span><span class="sxs-lookup"><span data-stu-id="8bc74-146">Detail</span></span> | <span data-ttu-id="8bc74-147">说明</span><span class="sxs-lookup"><span data-stu-id="8bc74-147">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="8bc74-148">taskAdded</span><span class="sxs-lookup"><span data-stu-id="8bc74-148">taskAdded</span></span> | <span data-ttu-id="8bc74-149">详细信息包含各自的 `task` 对象</span><span class="sxs-lookup"><span data-stu-id="8bc74-149">The detail contains the respective `task` object</span></span> | <span data-ttu-id="8bc74-150">新建任务后触发。</span><span class="sxs-lookup"><span data-stu-id="8bc74-150">Fires when a new task has been created.</span></span> |
| <span data-ttu-id="8bc74-151">taskChanged</span><span class="sxs-lookup"><span data-stu-id="8bc74-151">taskChanged</span></span> | <span data-ttu-id="8bc74-152">详细信息包含各自的 `task` 对象</span><span class="sxs-lookup"><span data-stu-id="8bc74-152">The detail contains the respective `task` object</span></span> | <span data-ttu-id="8bc74-153">更改任务元数据（如标记已完成）时触发。</span><span class="sxs-lookup"><span data-stu-id="8bc74-153">Fires when task metadata has been changed, such as marking completed.</span></span> |
| <span data-ttu-id="8bc74-154">taskClick</span><span class="sxs-lookup"><span data-stu-id="8bc74-154">taskClick</span></span> | <span data-ttu-id="8bc74-155">详细信息包含各自的 `task` 对象</span><span class="sxs-lookup"><span data-stu-id="8bc74-155">The detail contains the respective `task` object</span></span> | <span data-ttu-id="8bc74-156">当用户单击或点击任务时触发。</span><span class="sxs-lookup"><span data-stu-id="8bc74-156">Fires when the user clicks or taps on a task.</span></span> |
| <span data-ttu-id="8bc74-157">taskRemoved</span><span class="sxs-lookup"><span data-stu-id="8bc74-157">taskRemoved</span></span> | <span data-ttu-id="8bc74-158">详细信息包含各自的 `task` 对象</span><span class="sxs-lookup"><span data-stu-id="8bc74-158">The detail contains the respective `task` object</span></span> | <span data-ttu-id="8bc74-159">删除现有任务后触发。</span><span class="sxs-lookup"><span data-stu-id="8bc74-159">Fires when an existing task has been deleted.</span></span> |

## <a name="templates"></a><span data-ttu-id="8bc74-160">模板</span><span class="sxs-lookup"><span data-stu-id="8bc74-160">Templates</span></span>

<span data-ttu-id="8bc74-161">该 `tasks` 组件支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="8bc74-161">The `tasks` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="8bc74-162">若要指定模板，请包含组件 `<template>` 中的元素，将值设置为下列 `data-type` 值之一。</span><span class="sxs-lookup"><span data-stu-id="8bc74-162">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="8bc74-163">数据类型</span><span class="sxs-lookup"><span data-stu-id="8bc74-163">Data type</span></span>     | <span data-ttu-id="8bc74-164">数据上下文</span><span class="sxs-lookup"><span data-stu-id="8bc74-164">Data context</span></span>              | <span data-ttu-id="8bc74-165">说明</span><span class="sxs-lookup"><span data-stu-id="8bc74-165">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="8bc74-166">task</span><span class="sxs-lookup"><span data-stu-id="8bc74-166">task</span></span>     | <span data-ttu-id="8bc74-167">task： a to-do task object</span><span class="sxs-lookup"><span data-stu-id="8bc74-167">task: a to-do task object</span></span> | <span data-ttu-id="8bc74-168">替换整个默认任务。</span><span class="sxs-lookup"><span data-stu-id="8bc74-168">Replaces the whole default task.</span></span> |
| <span data-ttu-id="8bc74-169">task-details</span><span class="sxs-lookup"><span data-stu-id="8bc74-169">task-details</span></span> | <span data-ttu-id="8bc74-170">task： a to-do task object</span><span class="sxs-lookup"><span data-stu-id="8bc74-170">task: a to-do task object</span></span> | <span data-ttu-id="8bc74-171">模板将替换任务的详细信息部分。</span><span class="sxs-lookup"><span data-stu-id="8bc74-171">Template replaces the details section of the task.</span></span> |

<span data-ttu-id="8bc74-172">下面的示例定义任务组件的模板。</span><span class="sxs-lookup"><span data-stu-id="8bc74-172">The following example defines a template for the tasks component.</span></span>

```html
<mgt-todo>
    <template data-type="task-details">
        <div>
            Importance Level: {{task.importance}}
        </div>
    </template>
</mgt-todo>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="8bc74-173">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="8bc74-173">Microsoft Graph permissions</span></span>

<span data-ttu-id="8bc74-174">此控件使用以下 Microsoft Graph API 和权限。</span><span class="sxs-lookup"><span data-stu-id="8bc74-174">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="8bc74-175">资源</span><span class="sxs-lookup"><span data-stu-id="8bc74-175">Resource</span></span> | <span data-ttu-id="8bc74-176">权限</span><span class="sxs-lookup"><span data-stu-id="8bc74-176">Permission</span></span> |
| - | - |
| [<span data-ttu-id="8bc74-177">/me/todo/lists/</span><span class="sxs-lookup"><span data-stu-id="8bc74-177">/me/todo/lists/</span></span>](/graph/api/todo-list-lists) | <span data-ttu-id="8bc74-178">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bc74-178">Tasks.ReadWrite</span></span> |
| [<span data-ttu-id="8bc74-179">/me/todo/lists/{todoTaskListId}/tasks</span><span class="sxs-lookup"><span data-stu-id="8bc74-179">/me/todo/lists/{todoTaskListId}/tasks</span></span>](/graph/api/todotasklist-list-tasks) | <span data-ttu-id="8bc74-180">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bc74-180">Tasks.ReadWrite</span></span> |
| [<span data-ttu-id="8bc74-181">/me/todo/lists/{todoTaskListId}/tasks/{taskId}</span><span class="sxs-lookup"><span data-stu-id="8bc74-181">/me/todo/lists/{todoTaskListId}/tasks/{taskId}</span></span>](/graph/api/todotask-get) | <span data-ttu-id="8bc74-182">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bc74-182">Tasks.ReadWrite</span></span> |

## <a name="authentication"></a><span data-ttu-id="8bc74-183">身份验证</span><span class="sxs-lookup"><span data-stu-id="8bc74-183">Authentication</span></span>

<span data-ttu-id="8bc74-184">任务组件使用身份验证文档中介绍的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="8bc74-184">The tasks component uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>
