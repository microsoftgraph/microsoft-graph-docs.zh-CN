---
title: Microsoft 计划中的议程Graph Toolkit
description: mgt-agenda Web 组件用于表示用户或组日历中的事件。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 7de172c514aea12e0f57541649b6e98ca1ded2df
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781098"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="44a14-103">Microsoft 计划中的议程Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="44a14-103">Agenda component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="44a14-104">Web `mgt-agenda` 组件表示用户或组日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="44a14-104">The `mgt-agenda` web component represents events in a user or group calendar.</span></span> <span data-ttu-id="44a14-105">默认情况下，日历显示当前日期的当前已登录用户事件。</span><span class="sxs-lookup"><span data-stu-id="44a14-105">By default, the calendar displays the current signed in user events for the current day.</span></span> <span data-ttu-id="44a14-106">该组件还可使用从 Microsoft Graph 返回事件的任何终结点。</span><span class="sxs-lookup"><span data-stu-id="44a14-106">The component can also use any endpoint that returns events from Microsoft Graph.</span></span>

## <a name="example"></a><span data-ttu-id="44a14-107">示例</span><span class="sxs-lookup"><span data-stu-id="44a14-107">Example</span></span>

<span data-ttu-id="44a14-108">以下示例显示使用 组件显示的已登录用户的日历 `mgt-agenda` 事件。</span><span class="sxs-lookup"><span data-stu-id="44a14-108">The following example shows the signed-in user's calendar events displayed using the `mgt-agenda` component.</span></span> <span data-ttu-id="44a14-109">可以使用代码编辑器查看 [属性如何](#properties) 更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="44a14-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-agenda--simple&source=docs" height="500"></iframe>

[<span data-ttu-id="44a14-110">在"打开"mgt.dev</span><span class="sxs-lookup"><span data-stu-id="44a14-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-agenda--simple&source=docs)

## <a name="properties"></a><span data-ttu-id="44a14-111">属性</span><span class="sxs-lookup"><span data-stu-id="44a14-111">Properties</span></span>

<span data-ttu-id="44a14-112">默认情况下， `mgt-agenda` 组件从终结点提取事件 `/me/calendarview` 并显示当天的事件。</span><span class="sxs-lookup"><span data-stu-id="44a14-112">By default, the `mgt-agenda` component fetches events from the `/me/calendarview` endpoint and displays events for the current day.</span></span> <span data-ttu-id="44a14-113">有几种属性可用于更改此行为。</span><span class="sxs-lookup"><span data-stu-id="44a14-113">There are several properties you can use to change this behavior.</span></span>

| <span data-ttu-id="44a14-114">属性</span><span class="sxs-lookup"><span data-stu-id="44a14-114">Attribute</span></span> | <span data-ttu-id="44a14-115">属性</span><span class="sxs-lookup"><span data-stu-id="44a14-115">Property</span></span> | <span data-ttu-id="44a14-116">说明</span><span class="sxs-lookup"><span data-stu-id="44a14-116">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="44a14-117">date</span><span class="sxs-lookup"><span data-stu-id="44a14-117">date</span></span> | <span data-ttu-id="44a14-118">date</span><span class="sxs-lookup"><span data-stu-id="44a14-118">date</span></span> | <span data-ttu-id="44a14-119">一个字符串，表示从 Microsoft Graph 提取的事件的开始日期。</span><span class="sxs-lookup"><span data-stu-id="44a14-119">A string that represents the start date of the events to fetch from Microsoft Graph.</span></span> <span data-ttu-id="44a14-120">值应采用 Date 构造函数可以分析的格式 [-](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) 如果设置了属性，则值 `event-query` 无效。</span><span class="sxs-lookup"><span data-stu-id="44a14-120">Value should be in a format that can be parsed by the [Date constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="44a14-121">days</span><span class="sxs-lookup"><span data-stu-id="44a14-121">days</span></span> | <span data-ttu-id="44a14-122">days</span><span class="sxs-lookup"><span data-stu-id="44a14-122">days</span></span> | <span data-ttu-id="44a14-123">从 Microsoft Graph获取的天数 - 默认值为 3 - 如果设置了属性，则值 `event-query` 无效。</span><span class="sxs-lookup"><span data-stu-id="44a14-123">A number of days to fetch from Microsoft Graph - default is 3 - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="44a14-124">show-max</span><span class="sxs-lookup"><span data-stu-id="44a14-124">show-max</span></span> | <span data-ttu-id="44a14-125">showMax</span><span class="sxs-lookup"><span data-stu-id="44a14-125">showMax</span></span> | <span data-ttu-id="44a14-126">一个数字，指示要显示的最大事件数。</span><span class="sxs-lookup"><span data-stu-id="44a14-126">A number to indicate the maximum number of events to show.</span></span> <span data-ttu-id="44a14-127">默认值未设置为没有 (最大值) 。</span><span class="sxs-lookup"><span data-stu-id="44a14-127">The default value is not set (no maximum).</span></span> |
| <span data-ttu-id="44a14-128">group-id</span><span class="sxs-lookup"><span data-stu-id="44a14-128">group-id</span></span> | <span data-ttu-id="44a14-129">groupId</span><span class="sxs-lookup"><span data-stu-id="44a14-129">groupId</span></span> | <span data-ttu-id="44a14-130">使用组日历的字符串 ID，而不是当前登录用户的日历。</span><span class="sxs-lookup"><span data-stu-id="44a14-130">A string ID for a group calendar to use instead of the current signed in user's calendar.</span></span> |
| <span data-ttu-id="44a14-131">event-query</span><span class="sxs-lookup"><span data-stu-id="44a14-131">event-query</span></span> | <span data-ttu-id="44a14-132">eventQuery</span><span class="sxs-lookup"><span data-stu-id="44a14-132">eventQuery</span></span> | <span data-ttu-id="44a14-133">一个字符串，表示在从 Microsoft 网站提取事件时所使用的Graph。</span><span class="sxs-lookup"><span data-stu-id="44a14-133">A string that represents an alternative query to be used when fetching events from Microsoft Graph.</span></span> <span data-ttu-id="44a14-134">（可选）在字符串末尾添加委派作用域，用 `|` `/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all` () 。</span><span class="sxs-lookup"><span data-stu-id="44a14-134">Optionally, add the delegated scope at the end of the string by delimiting it with `|` (`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`).</span></span> |
| <span data-ttu-id="44a14-135">events</span><span class="sxs-lookup"><span data-stu-id="44a14-135">events</span></span> | <span data-ttu-id="44a14-136">events</span><span class="sxs-lookup"><span data-stu-id="44a14-136">events</span></span> | <span data-ttu-id="44a14-137">用于获取或设置组件呈现的事件列表的事件数组 - 使用此属性访问组件加载的事件。</span><span class="sxs-lookup"><span data-stu-id="44a14-137">An array of events to get or set the list of events rendered by the component - use this property to access the events loaded by the component.</span></span> <span data-ttu-id="44a14-138">设置此值以加载你自己的事件 - 如果值由开发人员设置，则 `date` 、 `days` 或 `event-query` 属性不起作用。</span><span class="sxs-lookup"><span data-stu-id="44a14-138">Set this value to load your own events - if value is set by developer, the `date`, `days`, or `event-query` attributes have no effect.</span></span> |
| <span data-ttu-id="44a14-139">按天分组</span><span class="sxs-lookup"><span data-stu-id="44a14-139">group-by-day</span></span> | <span data-ttu-id="44a14-140">groupByDay</span><span class="sxs-lookup"><span data-stu-id="44a14-140">groupByDay</span></span> | <span data-ttu-id="44a14-141">按天对事件进行分组的布尔值 - 默认情况下不对事件进行分组。</span><span class="sxs-lookup"><span data-stu-id="44a14-141">A Boolean value to group events by day - by default events are not grouped.</span></span> |
| <span data-ttu-id="44a14-142">preferred-timezone</span><span class="sxs-lookup"><span data-stu-id="44a14-142">preferred-timezone</span></span> | <span data-ttu-id="44a14-143">preferredTimezone</span><span class="sxs-lookup"><span data-stu-id="44a14-143">preferredTimezone</span></span> | <span data-ttu-id="44a14-144">从 Microsoft 网站检索事件时使用的首选时区Graph;例如， `Pacific Standard Time` 。</span><span class="sxs-lookup"><span data-stu-id="44a14-144">Name of the preferred time zone to use when retrieving events from Microsoft Graph; for example, `Pacific Standard Time`.</span></span> <span data-ttu-id="44a14-145">默认情况下，此属性使用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="44a14-145">By default, this attribute uses the UTC time zone.</span></span> <span data-ttu-id="44a14-146">通过调用 终结点并读取 timeZone 属性的值，可以检索当前 `me/mailboxSettings` **用户的首选** 时区。</span><span class="sxs-lookup"><span data-stu-id="44a14-146">The preferred time zone for the current user can be retrieved by calling the `me/mailboxSettings` endpoint and reading the value of the **timeZone** property.</span></span> |

<span data-ttu-id="44a14-147">以下示例将组件的行为更改为获取特定日期的数据，最多三天。</span><span class="sxs-lookup"><span data-stu-id="44a14-147">The following example changes the behavior of the component to fetch data for a specific date and up to three days.</span></span>

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

<span data-ttu-id="44a14-148">以下示例将组件的行为更改为从特定查询提取数据。</span><span class="sxs-lookup"><span data-stu-id="44a14-148">The following example changes the behavior of the component to fetch data from a specific query.</span></span>

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="methods"></a><span data-ttu-id="44a14-149">方法</span><span class="sxs-lookup"><span data-stu-id="44a14-149">Methods</span></span>
| <span data-ttu-id="44a14-150">方法</span><span class="sxs-lookup"><span data-stu-id="44a14-150">Method</span></span> | <span data-ttu-id="44a14-151">说明</span><span class="sxs-lookup"><span data-stu-id="44a14-151">Description</span></span> |
| --- | --- |
| <span data-ttu-id="44a14-152">重新加载 () </span><span class="sxs-lookup"><span data-stu-id="44a14-152">reload()</span></span> | <span data-ttu-id="44a14-153">调用 方法，根据组件的属性使用潜在的新数据重新加载组件。</span><span class="sxs-lookup"><span data-stu-id="44a14-153">Call the method to reload the component with potential new data based on its properties.</span></span> |

## <a name="css-custom-properties"></a><span data-ttu-id="44a14-154">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="44a14-154">CSS custom properties</span></span>

<span data-ttu-id="44a14-155">组件 `mgt-agenda` 定义这些 CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="44a14-155">The `mgt-agenda` component defines these CSS custom properties</span></span>

```css
mgt-agenda {
  --event-box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.092);
  --event-margin: 0px 10px 14px 10px;
  --event-padding: 8px 0px;
  --event-background-color: #ffffff;
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

<span data-ttu-id="44a14-156">若要了解更多信息，请参阅 [设置组件样式](../customize-components/style.md)。</span><span class="sxs-lookup"><span data-stu-id="44a14-156">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="44a14-157">模板</span><span class="sxs-lookup"><span data-stu-id="44a14-157">Templates</span></span>

<span data-ttu-id="44a14-158">组件 `mgt-agenda` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="44a14-158">The `mgt-agenda` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="44a14-159">若要指定模板，请包含组件 `<template>` 内的元素，将值 `data-type` 设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="44a14-159">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="44a14-160">数据类型</span><span class="sxs-lookup"><span data-stu-id="44a14-160">Data type</span></span> | <span data-ttu-id="44a14-161">数据上下文</span><span class="sxs-lookup"><span data-stu-id="44a14-161">Data context</span></span> | <span data-ttu-id="44a14-162">说明</span><span class="sxs-lookup"><span data-stu-id="44a14-162">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="44a14-163">`events`：event 对象列表</span><span class="sxs-lookup"><span data-stu-id="44a14-163">`events`: list of event objects</span></span> | <span data-ttu-id="44a14-164">默认模板将整个组件替换为你自己的组件。</span><span class="sxs-lookup"><span data-stu-id="44a14-164">The default template replaces the entire component with your own.</span></span> |
| `event` | <span data-ttu-id="44a14-165">`event`： event 对象</span><span class="sxs-lookup"><span data-stu-id="44a14-165">`event`: event object</span></span> | <span data-ttu-id="44a14-166">用于呈现每个事件的模板。</span><span class="sxs-lookup"><span data-stu-id="44a14-166">The template used to render each event.</span></span> |
| `event-other` | <span data-ttu-id="44a14-167">`event`： event 对象</span><span class="sxs-lookup"><span data-stu-id="44a14-167">`event`: event object</span></span> | <span data-ttu-id="44a14-168">用于呈现每个事件的其他内容的模板。</span><span class="sxs-lookup"><span data-stu-id="44a14-168">The template used to render additional content for each event.</span></span> |
| `header` | <span data-ttu-id="44a14-169">`header`： string</span><span class="sxs-lookup"><span data-stu-id="44a14-169">`header`: string</span></span> | <span data-ttu-id="44a14-170">用于呈现每天的标题的模板。</span><span class="sxs-lookup"><span data-stu-id="44a14-170">The template used to render the header for each day.</span></span> |
| `loading` | <span data-ttu-id="44a14-171">不传递任何数据上下文</span><span class="sxs-lookup"><span data-stu-id="44a14-171">No data context is passed</span></span> | <span data-ttu-id="44a14-172">加载数据时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="44a14-172">The template used when data is loading.</span></span> |
| `no-data` | <span data-ttu-id="44a14-173">不传递任何数据上下文</span><span class="sxs-lookup"><span data-stu-id="44a14-173">No data context is passed</span></span> | <span data-ttu-id="44a14-174">没有可用事件时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="44a14-174">The template used when no events are available.</span></span> |

<span data-ttu-id="44a14-175">以下示例演示如何使用 `event` 模板：</span><span class="sxs-lookup"><span data-stu-id="44a14-175">The following examples illustrates how to use the `event` template:</span></span>

```html
<mgt-agenda>
  <template data-type="event">
    <button class="eventButton">
      <div class="event-subject">{{ event.subject }}</div>
      <div data-for="attendee in event.attendees">
        <mgt-person
          person-query="{{ attendee.emailAddress.name }}"
          view="twolines">
        </mgt-person>
      </div>
    </button>
  </template>
  <template data-type="no-data">
    There are no events found!
  </template>
</mgt-agenda>
```

<span data-ttu-id="44a14-176">若要了解更多信息，请参阅 [模板](../customize-components/templates.md)。</span><span class="sxs-lookup"><span data-stu-id="44a14-176">To learn more, see [templates](../customize-components/templates.md).</span></span>

## <a name="events"></a><span data-ttu-id="44a14-177">活动</span><span class="sxs-lookup"><span data-stu-id="44a14-177">Events</span></span>

<span data-ttu-id="44a14-178">从控件中触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="44a14-178">The following events are fired from the control.</span></span>

| <span data-ttu-id="44a14-179">事件</span><span class="sxs-lookup"><span data-stu-id="44a14-179">Event</span></span> | <span data-ttu-id="44a14-180">说明</span><span class="sxs-lookup"><span data-stu-id="44a14-180">Description</span></span> |
| --- | --- |
| <span data-ttu-id="44a14-181">eventClick</span><span class="sxs-lookup"><span data-stu-id="44a14-181">eventClick</span></span> | <span data-ttu-id="44a14-182">用户单击或点击事件。</span><span class="sxs-lookup"><span data-stu-id="44a14-182">The user clicks or taps an event.</span></span>|

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="44a14-183">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="44a14-183">Microsoft Graph permissions</span></span>

<span data-ttu-id="44a14-184">此组件使用以下 Microsoft Graph API 和权限：</span><span class="sxs-lookup"><span data-stu-id="44a14-184">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="44a14-185">配置</span><span class="sxs-lookup"><span data-stu-id="44a14-185">Configuration</span></span> | <span data-ttu-id="44a14-186">权限</span><span class="sxs-lookup"><span data-stu-id="44a14-186">Permission</span></span> | <span data-ttu-id="44a14-187">API</span><span class="sxs-lookup"><span data-stu-id="44a14-187">API</span></span>
| - | - | - |
| <span data-ttu-id="44a14-188">default</span><span class="sxs-lookup"><span data-stu-id="44a14-188">default</span></span> | <span data-ttu-id="44a14-189">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="44a14-189">Calendars.Read</span></span> | [<span data-ttu-id="44a14-190">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="44a14-190">/me/calendarview</span></span>](/graph/api/calendar-list-calendarview) |

<span data-ttu-id="44a14-191">该组件允许你指定不同的 Microsoft Graph查询来调用 (，如 `/groups/{id}/calendar/calendarView`) 。</span><span class="sxs-lookup"><span data-stu-id="44a14-191">The component allows you to specify a different Microsoft Graph query to call (such as `/groups/{id}/calendar/calendarView`).</span></span> <span data-ttu-id="44a14-192">在这种情况下，将权限追加到字符串的末尾，以 分隔 `|` 。</span><span class="sxs-lookup"><span data-stu-id="44a14-192">In this case, append the permission to the end of the string, delimited by `|`.</span></span>

<span data-ttu-id="44a14-193">使用默认模板和默认 `renderAttendees` 模板时，需要其他 API 和权限。</span><span class="sxs-lookup"><span data-stu-id="44a14-193">When using the default template and default `renderAttendees` template, additional APIs and permissions are required.</span></span> <span data-ttu-id="44a14-194">此组件的默认模板对具有与会者的事件使用 [mgt-people](people.md) 组件，并继承所有权限。</span><span class="sxs-lookup"><span data-stu-id="44a14-194">The default template for this component uses a [mgt-people](people.md) component for events that have attendees, and inherits all permissions.</span></span>

## <a name="authentication"></a><span data-ttu-id="44a14-195">身份验证</span><span class="sxs-lookup"><span data-stu-id="44a14-195">Authentication</span></span>

<span data-ttu-id="44a14-196">登录控件使用身份验证文档 中所述的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="44a14-196">The login control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="44a14-197">缓存</span><span class="sxs-lookup"><span data-stu-id="44a14-197">Cache</span></span>

<span data-ttu-id="44a14-198">`mgt-agenda`组件不缓存任何数据。</span><span class="sxs-lookup"><span data-stu-id="44a14-198">The `mgt-agenda` component doesn't cache any data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="44a14-199">扩展以了解更多控件</span><span class="sxs-lookup"><span data-stu-id="44a14-199">Extend for more control</span></span>

<span data-ttu-id="44a14-200">对于更复杂的方案或真正自定义的 UX，此组件公开多个 `protected` render\* 方法以在组件扩展中替代。</span><span class="sxs-lookup"><span data-stu-id="44a14-200">For more complex scenarios or a truly custom UX, this component exposes several `protected` render\* methods for override in component extensions.</span></span>

| <span data-ttu-id="44a14-201">方法</span><span class="sxs-lookup"><span data-stu-id="44a14-201">Method</span></span> | <span data-ttu-id="44a14-202">说明</span><span class="sxs-lookup"><span data-stu-id="44a14-202">Description</span></span> |
| - | - |
| <span data-ttu-id="44a14-203">renderLoading</span><span class="sxs-lookup"><span data-stu-id="44a14-203">renderLoading</span></span> | <span data-ttu-id="44a14-204">在组件加载时呈现加载状态。</span><span class="sxs-lookup"><span data-stu-id="44a14-204">Renders a loading state while the component loads.</span></span> |
| <span data-ttu-id="44a14-205">renderNoData</span><span class="sxs-lookup"><span data-stu-id="44a14-205">renderNoData</span></span> | <span data-ttu-id="44a14-206">呈现空数据状态。</span><span class="sxs-lookup"><span data-stu-id="44a14-206">Renders an empty data state.</span></span> |
| <span data-ttu-id="44a14-207">renderGroups</span><span class="sxs-lookup"><span data-stu-id="44a14-207">renderGroups</span></span> | <span data-ttu-id="44a14-208">将事件数据按组排序，然后使用组标头呈现它们。</span><span class="sxs-lookup"><span data-stu-id="44a14-208">Sorts event data into groups and renders them with group headers.</span></span> |
| <span data-ttu-id="44a14-209">renderHeader</span><span class="sxs-lookup"><span data-stu-id="44a14-209">renderHeader</span></span> | <span data-ttu-id="44a14-210">呈现组标头。</span><span class="sxs-lookup"><span data-stu-id="44a14-210">Renders a group header.</span></span> |
| <span data-ttu-id="44a14-211">renderEvents</span><span class="sxs-lookup"><span data-stu-id="44a14-211">renderEvents</span></span> | <span data-ttu-id="44a14-212">呈现 event 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="44a14-212">Renders a list of event objects.</span></span> |
| <span data-ttu-id="44a14-213">renderEvent</span><span class="sxs-lookup"><span data-stu-id="44a14-213">renderEvent</span></span> | <span data-ttu-id="44a14-214">呈现单数事件及其所有部分。</span><span class="sxs-lookup"><span data-stu-id="44a14-214">Renders a singular event and all of its parts.</span></span>
| <span data-ttu-id="44a14-215">renderTitle</span><span class="sxs-lookup"><span data-stu-id="44a14-215">renderTitle</span></span> | <span data-ttu-id="44a14-216">呈现事件标题部件。</span><span class="sxs-lookup"><span data-stu-id="44a14-216">Renders the event title part.</span></span> |
| <span data-ttu-id="44a14-217">renderLocation</span><span class="sxs-lookup"><span data-stu-id="44a14-217">renderLocation</span></span> | <span data-ttu-id="44a14-218">呈现事件位置部分。</span><span class="sxs-lookup"><span data-stu-id="44a14-218">Renders the event location part.</span></span> |
| <span data-ttu-id="44a14-219">renderAttendees</span><span class="sxs-lookup"><span data-stu-id="44a14-219">renderAttendees</span></span> | <span data-ttu-id="44a14-220">呈现事件参与者部分。</span><span class="sxs-lookup"><span data-stu-id="44a14-220">Renders the event attendees part.</span></span> |
| <span data-ttu-id="44a14-221">renderOther</span><span class="sxs-lookup"><span data-stu-id="44a14-221">renderOther</span></span> | <span data-ttu-id="44a14-222">呈现其他事件内容。</span><span class="sxs-lookup"><span data-stu-id="44a14-222">Renders additional event content.</span></span> |
