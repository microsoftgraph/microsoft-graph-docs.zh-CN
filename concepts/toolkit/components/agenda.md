---
title: Microsoft Graph 工具包中的 "议程" 组件
description: "\"管理中心议程\" web 组件用于表示用户或组日历中的事件。"
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: c42b62241f5eee7fef51bf57bf8617dd6e89b8c6
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/20/2020
ms.locfileid: "45183923"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="65e0f-103">Microsoft Graph 工具包中的 "议程" 组件</span><span class="sxs-lookup"><span data-stu-id="65e0f-103">Agenda component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="65e0f-104">`mgt-agenda`Web 组件表示用户或组日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="65e0f-104">The `mgt-agenda` web component represents events in a user or group calendar.</span></span> <span data-ttu-id="65e0f-105">默认情况下，日历会在当前日期的用户事件中显示当前登录的用户事件。</span><span class="sxs-lookup"><span data-stu-id="65e0f-105">By default, the calendar displays the current signed in user events for the current day.</span></span> <span data-ttu-id="65e0f-106">组件还可以使用从 Microsoft Graph 返回事件的任何终结点。</span><span class="sxs-lookup"><span data-stu-id="65e0f-106">The component can also use any endpoint that returns events from Microsoft Graph.</span></span>

## <a name="example"></a><span data-ttu-id="65e0f-107">示例</span><span class="sxs-lookup"><span data-stu-id="65e0f-107">Example</span></span>

<span data-ttu-id="65e0f-108">以下示例显示使用组件显示的已登录用户的日历事件 `mgt-agenda` 。</span><span class="sxs-lookup"><span data-stu-id="65e0f-108">The following example shows the signed-in user's calendar events displayed using the `mgt-agenda` component.</span></span> <span data-ttu-id="65e0f-109">您可以使用代码编辑器来查看[属性](#properties)如何更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="65e0f-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-agenda--simple&source=docs" height="500"></iframe>

[<span data-ttu-id="65e0f-110">在 "dev" 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="65e0f-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-agenda--simple&source=docs)

## <a name="properties"></a><span data-ttu-id="65e0f-111">属性</span><span class="sxs-lookup"><span data-stu-id="65e0f-111">Properties</span></span>

<span data-ttu-id="65e0f-112">默认情况下， `mgt-agenda` 组件从 `/me/calendarview` 终结点提取事件并显示当天的事件。</span><span class="sxs-lookup"><span data-stu-id="65e0f-112">By default, the `mgt-agenda` component fetches events from the `/me/calendarview` endpoint and displays events for the current day.</span></span> <span data-ttu-id="65e0f-113">有几个可用于更改此行为的属性。</span><span class="sxs-lookup"><span data-stu-id="65e0f-113">There are several properties you can use to change this behavior.</span></span>

| <span data-ttu-id="65e0f-114">属性</span><span class="sxs-lookup"><span data-stu-id="65e0f-114">Attribute</span></span> | <span data-ttu-id="65e0f-115">属性</span><span class="sxs-lookup"><span data-stu-id="65e0f-115">Property</span></span> | <span data-ttu-id="65e0f-116">说明</span><span class="sxs-lookup"><span data-stu-id="65e0f-116">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="65e0f-117">date</span><span class="sxs-lookup"><span data-stu-id="65e0f-117">date</span></span> | <span data-ttu-id="65e0f-118">date</span><span class="sxs-lookup"><span data-stu-id="65e0f-118">date</span></span> | <span data-ttu-id="65e0f-119">一个字符串，表示要从 Microsoft Graph 中提取的事件的开始日期。</span><span class="sxs-lookup"><span data-stu-id="65e0f-119">A string that represents the start date of the events to fetch from Microsoft Graph.</span></span> <span data-ttu-id="65e0f-120">值应采用可由[日期构造函数](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)进行分析的格式，如果设置了属性，则值不起作用 `event-query` 。</span><span class="sxs-lookup"><span data-stu-id="65e0f-120">Value should be in a format that can be parsed by the [Date constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="65e0f-121">之前</span><span class="sxs-lookup"><span data-stu-id="65e0f-121">days</span></span> | <span data-ttu-id="65e0f-122">之前</span><span class="sxs-lookup"><span data-stu-id="65e0f-122">days</span></span> | <span data-ttu-id="65e0f-123">从 Microsoft Graph 提取的天数-默认值为3。如果设置了属性，则此值不起作用 `event-query` 。</span><span class="sxs-lookup"><span data-stu-id="65e0f-123">A number of days to fetch from Microsoft Graph - default is 3 - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="65e0f-124">show-max</span><span class="sxs-lookup"><span data-stu-id="65e0f-124">show-max</span></span> | <span data-ttu-id="65e0f-125">showMax</span><span class="sxs-lookup"><span data-stu-id="65e0f-125">showMax</span></span> | <span data-ttu-id="65e0f-126">一个数字，用于指示要显示的最大事件数。</span><span class="sxs-lookup"><span data-stu-id="65e0f-126">A number to indicate the maximum number of events to show.</span></span> <span data-ttu-id="65e0f-127">未设置默认值（无最大值）。</span><span class="sxs-lookup"><span data-stu-id="65e0f-127">The default value is not set (no maximum).</span></span> |
| <span data-ttu-id="65e0f-128">组 id</span><span class="sxs-lookup"><span data-stu-id="65e0f-128">group-id</span></span> | <span data-ttu-id="65e0f-129">groupId</span><span class="sxs-lookup"><span data-stu-id="65e0f-129">groupId</span></span> | <span data-ttu-id="65e0f-130">要使用的组日历的字符串 ID，而不是当前登录的用户日历。</span><span class="sxs-lookup"><span data-stu-id="65e0f-130">A string ID for a group calendar to use instead of the current signed in user's calendar.</span></span> |
| <span data-ttu-id="65e0f-131">事件查询</span><span class="sxs-lookup"><span data-stu-id="65e0f-131">event-query</span></span> | <span data-ttu-id="65e0f-132">eventQuery</span><span class="sxs-lookup"><span data-stu-id="65e0f-132">eventQuery</span></span> | <span data-ttu-id="65e0f-133">一个字符串，表示从 Microsoft Graph 提取事件时要使用的替代查询。</span><span class="sxs-lookup"><span data-stu-id="65e0f-133">A string that represents an alternative query to be used when fetching events from Microsoft Graph.</span></span> <span data-ttu-id="65e0f-134">（可选）通过将委派作用域与（）分隔来将其添加到字符串的末尾 `|` `/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all` 。</span><span class="sxs-lookup"><span data-stu-id="65e0f-134">Optionally, add the delegated scope at the end of the string by delimiting it with `|` (`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`).</span></span> |
| <span data-ttu-id="65e0f-135">events</span><span class="sxs-lookup"><span data-stu-id="65e0f-135">events</span></span> | <span data-ttu-id="65e0f-136">events</span><span class="sxs-lookup"><span data-stu-id="65e0f-136">events</span></span> | <span data-ttu-id="65e0f-137">一个事件数组，用于获取或设置组件呈现的事件的列表-使用此属性可访问组件加载的事件。</span><span class="sxs-lookup"><span data-stu-id="65e0f-137">An array of events to get or set the list of events rendered by the component - use this property to access the events loaded by the component.</span></span> <span data-ttu-id="65e0f-138">将此值设置为加载您自己的事件-如果值是由开发人员设置的，则 `date` 、 `days` 或 `event-query` 属性不起作用。</span><span class="sxs-lookup"><span data-stu-id="65e0f-138">Set this value to load your own events - if value is set by developer, the `date`, `days`, or `event-query` attributes have no effect.</span></span> |
| <span data-ttu-id="65e0f-139">逐天分组</span><span class="sxs-lookup"><span data-stu-id="65e0f-139">group-by-day</span></span> | <span data-ttu-id="65e0f-140">groupByDay</span><span class="sxs-lookup"><span data-stu-id="65e0f-140">groupByDay</span></span> | <span data-ttu-id="65e0f-141">按天对事件分组的布尔值不按默认事件进行分组。</span><span class="sxs-lookup"><span data-stu-id="65e0f-141">A Boolean value to group events by day - by default events are not grouped.</span></span> |

<span data-ttu-id="65e0f-142">下面的示例更改组件的行为，以获取特定日期的数据，最长为三天。</span><span class="sxs-lookup"><span data-stu-id="65e0f-142">The following example changes the behavior of the component to fetch data for a specific date and up to three days.</span></span>

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

<span data-ttu-id="65e0f-143">下面的示例将更改组件的行为，以从特定查询中获取数据。</span><span class="sxs-lookup"><span data-stu-id="65e0f-143">The following example changes the behavior of the component to fetch data from a specific query.</span></span>

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="css-custom-properties"></a><span data-ttu-id="65e0f-144">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="65e0f-144">CSS custom properties</span></span>

<span data-ttu-id="65e0f-145">`mgt-agenda`组件定义这些 CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="65e0f-145">The `mgt-agenda` component defines these CSS custom properties</span></span>

```css
mgt-agenda {
  --event-box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.092);
  --event-margin: 0px 10px 14px 10px;
  --event-padding: 8px 0px;
  --event-background: #ffffff;
  --event-border: solid 2px rgba(0, 0, 0, 0);

  --agenda-header-margin: 40px 10px 14px 10px;
  --agenda-header-font-size: 24px;
  --agenda-header-color: #333333;

  --event-time-font-size: 12px;
  --event-time-color: #000000;

  --event-subject-font-size: 19px;
  --event-subject-color: #333333;

  --event-location-font-size: 12px;
  --event-location-color: #000000;
}
```

<span data-ttu-id="65e0f-146">若要了解详细信息，请参阅[样式组件](../style.md)。</span><span class="sxs-lookup"><span data-stu-id="65e0f-146">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="65e0f-147">模板</span><span class="sxs-lookup"><span data-stu-id="65e0f-147">Templates</span></span>

<span data-ttu-id="65e0f-148">`mgt-agenda`组件支持多个[模板](../templates.md)，这些模板允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="65e0f-148">The `mgt-agenda` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="65e0f-149">若要指定模板，请在 `<template>` 组件内添加一个元素，并将 `data-type` 值设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="65e0f-149">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="65e0f-150">数据类型</span><span class="sxs-lookup"><span data-stu-id="65e0f-150">Data type</span></span> | <span data-ttu-id="65e0f-151">数据上下文</span><span class="sxs-lookup"><span data-stu-id="65e0f-151">Data context</span></span> | <span data-ttu-id="65e0f-152">说明</span><span class="sxs-lookup"><span data-stu-id="65e0f-152">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="65e0f-153">`events`：事件对象的列表</span><span class="sxs-lookup"><span data-stu-id="65e0f-153">`events`: list of event objects</span></span> | <span data-ttu-id="65e0f-154">默认模板会将整个组件替换为您自己的组件。</span><span class="sxs-lookup"><span data-stu-id="65e0f-154">The default template replaces the entire component with your own.</span></span> |
| `event` | <span data-ttu-id="65e0f-155">`event`： event 对象</span><span class="sxs-lookup"><span data-stu-id="65e0f-155">`event`: event object</span></span> | <span data-ttu-id="65e0f-156">用于呈现每个事件的模板。</span><span class="sxs-lookup"><span data-stu-id="65e0f-156">The template used to render each event.</span></span> |
| `event-other` | <span data-ttu-id="65e0f-157">`event`： event 对象</span><span class="sxs-lookup"><span data-stu-id="65e0f-157">`event`: event object</span></span> | <span data-ttu-id="65e0f-158">用于呈现每个事件的其他内容的模板。</span><span class="sxs-lookup"><span data-stu-id="65e0f-158">The template used to render additional content for each event.</span></span> |
| `header` | <span data-ttu-id="65e0f-159">`header`： string</span><span class="sxs-lookup"><span data-stu-id="65e0f-159">`header`: string</span></span> | <span data-ttu-id="65e0f-160">用于呈现每天的标题的模板。</span><span class="sxs-lookup"><span data-stu-id="65e0f-160">The template used to render the header for each day.</span></span> |
| `loading` | <span data-ttu-id="65e0f-161">不传递数据上下文</span><span class="sxs-lookup"><span data-stu-id="65e0f-161">No data context is passed</span></span> | <span data-ttu-id="65e0f-162">加载数据时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="65e0f-162">The template used when data is loading.</span></span> |
| `no-data` | <span data-ttu-id="65e0f-163">不传递数据上下文</span><span class="sxs-lookup"><span data-stu-id="65e0f-163">No data context is passed</span></span> | <span data-ttu-id="65e0f-164">没有可用事件时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="65e0f-164">The template used when no events are available.</span></span> |

<span data-ttu-id="65e0f-165">下面的示例演示如何使用 `event` 模板：</span><span class="sxs-lookup"><span data-stu-id="65e0f-165">The following examples illustrates how to use the `event` template:</span></span>

```html
<mgt-agenda>
  <template data-type="event">
    <button class="eventButton">
      <div class="event-subject">{{ event.subject }}</div>
      <div data-for="attendee in event.attendees">
        <mgt-person
          person-query="{{ attendee.emailAddress.name }}"
          show-name
          show-email>
        </mgt-person>
      </div>
    </button>
  </template>
  <template data-type="no-data">
    There are no events found!
  </template>
</mgt-agenda>
```

<span data-ttu-id="65e0f-166">若要了解详细信息，请参阅[模板](../templates.md)。</span><span class="sxs-lookup"><span data-stu-id="65e0f-166">To learn more, see [templates](../templates.md).</span></span>

## <a name="events"></a><span data-ttu-id="65e0f-167">活动</span><span class="sxs-lookup"><span data-stu-id="65e0f-167">Events</span></span>

<span data-ttu-id="65e0f-168">从控件触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="65e0f-168">The following events are fired from the control.</span></span>

| <span data-ttu-id="65e0f-169">事件</span><span class="sxs-lookup"><span data-stu-id="65e0f-169">Event</span></span> | <span data-ttu-id="65e0f-170">说明</span><span class="sxs-lookup"><span data-stu-id="65e0f-170">Description</span></span> |
| --- | --- |
| <span data-ttu-id="65e0f-171">eventClick</span><span class="sxs-lookup"><span data-stu-id="65e0f-171">eventClick</span></span> | <span data-ttu-id="65e0f-172">用户单击或点击事件。</span><span class="sxs-lookup"><span data-stu-id="65e0f-172">The user clicks or taps an event.</span></span>|

## <a name="permissions"></a><span data-ttu-id="65e0f-173">权限</span><span class="sxs-lookup"><span data-stu-id="65e0f-173">Permissions</span></span>

<span data-ttu-id="65e0f-174">此组件使用以下 Microsoft Graph Api 和权限：</span><span class="sxs-lookup"><span data-stu-id="65e0f-174">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="65e0f-175">资源</span><span class="sxs-lookup"><span data-stu-id="65e0f-175">Resource</span></span> | <span data-ttu-id="65e0f-176">权限</span><span class="sxs-lookup"><span data-stu-id="65e0f-176">Permission</span></span> |
| - | - |
| [<span data-ttu-id="65e0f-177">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="65e0f-177">/me/calendarview</span></span>](/graph/api/calendar-list-calendarview?view=graph-rest-1.0) | <span data-ttu-id="65e0f-178">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="65e0f-178">Calendars.Read</span></span> |

<span data-ttu-id="65e0f-179">组件允许您指定要调用的其他 Microsoft Graph 查询（例如 `/groups/{id}/calendar/calendarView` ）。</span><span class="sxs-lookup"><span data-stu-id="65e0f-179">The component allows you to specify a different Microsoft Graph query to call (such as `/groups/{id}/calendar/calendarView`).</span></span> <span data-ttu-id="65e0f-180">在这种情况下，将权限追加到字符串的末尾，并将其作为分隔符 `|` 。</span><span class="sxs-lookup"><span data-stu-id="65e0f-180">In this case, append the permission to the end of the string, delimited by `|`.</span></span>

<span data-ttu-id="65e0f-181">使用默认模板和默认模板时 `renderAttendees` ，需要其他 api 和权限。</span><span class="sxs-lookup"><span data-stu-id="65e0f-181">When using the default template and default `renderAttendees` template, additional APIs and permissions are required.</span></span> <span data-ttu-id="65e0f-182">此组件的默认模板对具有与会者的事件使用 "it 人员" 组件，这需要以下各[项](people.md)。</span><span class="sxs-lookup"><span data-stu-id="65e0f-182">The default template for this component uses a [mgt-people](people.md) component for events that have attendees, which requires the following.</span></span>

| <span data-ttu-id="65e0f-183">资源</span><span class="sxs-lookup"><span data-stu-id="65e0f-183">Resource</span></span> | <span data-ttu-id="65e0f-184">权限</span><span class="sxs-lookup"><span data-stu-id="65e0f-184">Permission</span></span> |
| - | - |
| [<span data-ttu-id="65e0f-185">/users</span><span class="sxs-lookup"><span data-stu-id="65e0f-185">/users</span></span>](/graph/api/user-list?view=graph-rest-1.0) | <span data-ttu-id="65e0f-186">User.readbasic.all</span><span class="sxs-lookup"><span data-stu-id="65e0f-186">Users.ReadBasic.All</span></span> |
| [<span data-ttu-id="65e0f-187">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="65e0f-187">/me/calendarview</span></span>](/graph/api/user-list-people?view=graph-rest-1.0) | <span data-ttu-id="65e0f-188">People.Read</span><span class="sxs-lookup"><span data-stu-id="65e0f-188">People.Read</span></span> |
| [<span data-ttu-id="65e0f-189">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="65e0f-189">/me/calendarview</span></span>](/graph/api/user-list-contacts?view=graph-rest-1.0) | <span data-ttu-id="65e0f-190">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="65e0f-190">Contacts.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="65e0f-191">身份验证</span><span class="sxs-lookup"><span data-stu-id="65e0f-191">Authentication</span></span>

<span data-ttu-id="65e0f-192">登录控件利用[身份验证文档](./../providers.md)中所述的全局验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="65e0f-192">The login control leverages the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="65e0f-193">扩展以实现更多控制</span><span class="sxs-lookup"><span data-stu-id="65e0f-193">Extend for more control</span></span>

<span data-ttu-id="65e0f-194">对于更复杂的方案或真正的自定义 UX，此组件 `protected` 在组件扩展中公开了几种用于覆盖的 render \* 方法。</span><span class="sxs-lookup"><span data-stu-id="65e0f-194">For more complex scenarios or a truly custom UX, this component exposes several `protected` render\* methods for override in component extensions.</span></span>

| <span data-ttu-id="65e0f-195">方法</span><span class="sxs-lookup"><span data-stu-id="65e0f-195">Method</span></span> | <span data-ttu-id="65e0f-196">说明</span><span class="sxs-lookup"><span data-stu-id="65e0f-196">Description</span></span> |
| - | - |
| <span data-ttu-id="65e0f-197">renderLoading</span><span class="sxs-lookup"><span data-stu-id="65e0f-197">renderLoading</span></span> | <span data-ttu-id="65e0f-198">在加载组件时呈现加载状态。</span><span class="sxs-lookup"><span data-stu-id="65e0f-198">Renders a loading state while the component loads.</span></span> |
| <span data-ttu-id="65e0f-199">renderNoData</span><span class="sxs-lookup"><span data-stu-id="65e0f-199">renderNoData</span></span> | <span data-ttu-id="65e0f-200">呈现空数据状态。</span><span class="sxs-lookup"><span data-stu-id="65e0f-200">Renders an empty data state.</span></span> |
| <span data-ttu-id="65e0f-201">renderGroups</span><span class="sxs-lookup"><span data-stu-id="65e0f-201">renderGroups</span></span> | <span data-ttu-id="65e0f-202">将事件数据分为组，并使用组标头进行呈现。</span><span class="sxs-lookup"><span data-stu-id="65e0f-202">Sorts event data into groups and renders them with group headers.</span></span> |
| <span data-ttu-id="65e0f-203">renderHeader</span><span class="sxs-lookup"><span data-stu-id="65e0f-203">renderHeader</span></span> | <span data-ttu-id="65e0f-204">呈现组标头。</span><span class="sxs-lookup"><span data-stu-id="65e0f-204">Renders a group header.</span></span> |
| <span data-ttu-id="65e0f-205">renderEvents</span><span class="sxs-lookup"><span data-stu-id="65e0f-205">renderEvents</span></span> | <span data-ttu-id="65e0f-206">呈现事件对象的列表。</span><span class="sxs-lookup"><span data-stu-id="65e0f-206">Renders a list of event objects.</span></span> |
| <span data-ttu-id="65e0f-207">renderEvent</span><span class="sxs-lookup"><span data-stu-id="65e0f-207">renderEvent</span></span> | <span data-ttu-id="65e0f-208">呈现单数事件及其所有部件。</span><span class="sxs-lookup"><span data-stu-id="65e0f-208">Renders a singular event and all of its parts.</span></span>
| <span data-ttu-id="65e0f-209">renderTitle</span><span class="sxs-lookup"><span data-stu-id="65e0f-209">renderTitle</span></span> | <span data-ttu-id="65e0f-210">呈现事件标题部分。</span><span class="sxs-lookup"><span data-stu-id="65e0f-210">Renders the event title part.</span></span> |
| <span data-ttu-id="65e0f-211">renderLocation</span><span class="sxs-lookup"><span data-stu-id="65e0f-211">renderLocation</span></span> | <span data-ttu-id="65e0f-212">呈现事件位置部分。</span><span class="sxs-lookup"><span data-stu-id="65e0f-212">Renders the event location part.</span></span> |
| <span data-ttu-id="65e0f-213">renderAttendees</span><span class="sxs-lookup"><span data-stu-id="65e0f-213">renderAttendees</span></span> | <span data-ttu-id="65e0f-214">呈现事件的与会者部件。</span><span class="sxs-lookup"><span data-stu-id="65e0f-214">Renders the event attendees part.</span></span> |
| <span data-ttu-id="65e0f-215">renderOther</span><span class="sxs-lookup"><span data-stu-id="65e0f-215">renderOther</span></span> | <span data-ttu-id="65e0f-216">呈现其他事件内容。</span><span class="sxs-lookup"><span data-stu-id="65e0f-216">Renders additional event content.</span></span> |
