---
title: Microsoft Graph 工具包中的 "议程" 组件
description: "\"管理中心议程\" web 组件用于表示用户或组日历中的事件。"
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 334da23db286c7243b9722cae443913219a97f7f
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639945"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="097cc-103">Microsoft Graph 工具包中的 "议程" 组件</span><span class="sxs-lookup"><span data-stu-id="097cc-103">Agenda component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="097cc-104">`mgt-agenda` Web 组件表示用户或组日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="097cc-104">The `mgt-agenda` web component represents events in a user or group calendar.</span></span> <span data-ttu-id="097cc-105">默认情况下，日历会在当前日期的用户事件中显示当前登录的用户事件。</span><span class="sxs-lookup"><span data-stu-id="097cc-105">By default, the calendar displays the current signed in user events for the current day.</span></span> <span data-ttu-id="097cc-106">组件还可以使用从 Microsoft Graph 返回事件的任何终结点。</span><span class="sxs-lookup"><span data-stu-id="097cc-106">The component can also use any endpoint that returns events from Microsoft Graph.</span></span>

## <a name="example"></a><span data-ttu-id="097cc-107">示例</span><span class="sxs-lookup"><span data-stu-id="097cc-107">Example</span></span>

<span data-ttu-id="097cc-108">以下示例显示使用`mgt-agenda`组件显示的已登录用户的日历事件。</span><span class="sxs-lookup"><span data-stu-id="097cc-108">The following example shows the signed-in user's calendar events displayed using the `mgt-agenda` component.</span></span> <span data-ttu-id="097cc-109">您可以使用代码编辑器来查看[属性](#properties)如何更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="097cc-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-agenda--simple&source=docs" height="500"></iframe>

[<span data-ttu-id="097cc-110">在 "dev" 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="097cc-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-agenda--simple&source=docs)

## <a name="properties"></a><span data-ttu-id="097cc-111">属性</span><span class="sxs-lookup"><span data-stu-id="097cc-111">Properties</span></span>

<span data-ttu-id="097cc-112">默认情况下， `mgt-agenda`组件从`/me/calendarview`终结点提取事件并显示当天的事件。</span><span class="sxs-lookup"><span data-stu-id="097cc-112">By default, the `mgt-agenda` component fetches events from the `/me/calendarview` endpoint and displays events for the current day.</span></span> <span data-ttu-id="097cc-113">有几个可用于更改此行为的属性。</span><span class="sxs-lookup"><span data-stu-id="097cc-113">There are several properties you can use to change this behavior.</span></span>

| <span data-ttu-id="097cc-114">属性</span><span class="sxs-lookup"><span data-stu-id="097cc-114">Attribute</span></span> | <span data-ttu-id="097cc-115">属性</span><span class="sxs-lookup"><span data-stu-id="097cc-115">Property</span></span> | <span data-ttu-id="097cc-116">说明</span><span class="sxs-lookup"><span data-stu-id="097cc-116">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="097cc-117">date</span><span class="sxs-lookup"><span data-stu-id="097cc-117">date</span></span> | <span data-ttu-id="097cc-118">date</span><span class="sxs-lookup"><span data-stu-id="097cc-118">date</span></span> | <span data-ttu-id="097cc-119">一个字符串，表示要从 Microsoft Graph 中提取的事件的开始日期。</span><span class="sxs-lookup"><span data-stu-id="097cc-119">A string that represents the start date of the events to fetch from Microsoft Graph.</span></span> <span data-ttu-id="097cc-120">值应采用可由[日期构造函数](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)进行分析的格式，如果`event-query`设置了属性，则值不起作用。</span><span class="sxs-lookup"><span data-stu-id="097cc-120">Value should be in a format that can be parsed by the [Date constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="097cc-121">之前</span><span class="sxs-lookup"><span data-stu-id="097cc-121">days</span></span> | <span data-ttu-id="097cc-122">之前</span><span class="sxs-lookup"><span data-stu-id="097cc-122">days</span></span> | <span data-ttu-id="097cc-123">从 Microsoft Graph 提取的天数-默认值为3。如果`event-query`设置了属性，则此值不起作用。</span><span class="sxs-lookup"><span data-stu-id="097cc-123">A number of days to fetch from Microsoft Graph - default is 3 - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="097cc-124">show-max</span><span class="sxs-lookup"><span data-stu-id="097cc-124">show-max</span></span> | <span data-ttu-id="097cc-125">showMax</span><span class="sxs-lookup"><span data-stu-id="097cc-125">showMax</span></span> | <span data-ttu-id="097cc-126">一个数字，用于指示要显示的最大事件数。</span><span class="sxs-lookup"><span data-stu-id="097cc-126">A number to indicate the maximum number of events to show.</span></span> <span data-ttu-id="097cc-127">未设置默认值（无最大值）。</span><span class="sxs-lookup"><span data-stu-id="097cc-127">The default value is not set (no maximum).</span></span> |
| <span data-ttu-id="097cc-128">组 id</span><span class="sxs-lookup"><span data-stu-id="097cc-128">group-id</span></span> | <span data-ttu-id="097cc-129">groupId</span><span class="sxs-lookup"><span data-stu-id="097cc-129">groupId</span></span> | <span data-ttu-id="097cc-130">要使用的组日历的字符串 ID，而不是当前登录的用户日历。</span><span class="sxs-lookup"><span data-stu-id="097cc-130">A string ID for a group calendar to use instead of the current signed in user's calendar.</span></span> |
| <span data-ttu-id="097cc-131">事件查询</span><span class="sxs-lookup"><span data-stu-id="097cc-131">event-query</span></span> | <span data-ttu-id="097cc-132">eventQuery</span><span class="sxs-lookup"><span data-stu-id="097cc-132">eventQuery</span></span> | <span data-ttu-id="097cc-133">一个字符串，表示从 Microsoft Graph 提取事件时要使用的替代查询。</span><span class="sxs-lookup"><span data-stu-id="097cc-133">A string that represents an alternative query to be used when fetching events from Microsoft Graph.</span></span> <span data-ttu-id="097cc-134">（可选）通过将委派作用域与`|` （`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`）分隔来将其添加到字符串的末尾。</span><span class="sxs-lookup"><span data-stu-id="097cc-134">Optionally, add the delegated scope at the end of the string by delimiting it with `|` (`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`).</span></span> |
| <span data-ttu-id="097cc-135">events</span><span class="sxs-lookup"><span data-stu-id="097cc-135">events</span></span> | <span data-ttu-id="097cc-136">events</span><span class="sxs-lookup"><span data-stu-id="097cc-136">events</span></span> | <span data-ttu-id="097cc-137">一个事件数组，用于获取或设置组件呈现的事件的列表-使用此属性可访问组件加载的事件。</span><span class="sxs-lookup"><span data-stu-id="097cc-137">An array of events to get or set the list of events rendered by the component - use this property to access the events loaded by the component.</span></span> <span data-ttu-id="097cc-138">将此值设置为加载您自己的事件-如果值是由开发人员`date`设置`days`的， `event-query`则、或属性不起作用。</span><span class="sxs-lookup"><span data-stu-id="097cc-138">Set this value to load your own events - if value is set by developer, the `date`, `days`, or `event-query` attributes have no effect.</span></span> |
| <span data-ttu-id="097cc-139">逐天分组</span><span class="sxs-lookup"><span data-stu-id="097cc-139">group-by-day</span></span> | <span data-ttu-id="097cc-140">groupByDay</span><span class="sxs-lookup"><span data-stu-id="097cc-140">groupByDay</span></span> | <span data-ttu-id="097cc-141">按天对事件分组的布尔值不按默认事件进行分组。</span><span class="sxs-lookup"><span data-stu-id="097cc-141">A Boolean value to group events by day - by default events are not grouped.</span></span> |

<span data-ttu-id="097cc-142">下面的示例更改组件的行为，以获取特定日期的数据，最长为三天。</span><span class="sxs-lookup"><span data-stu-id="097cc-142">The following example changes the behavior of the component to fetch data for a specific date and up to three days.</span></span>

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

<span data-ttu-id="097cc-143">下面的示例将更改组件的行为，以从特定查询中获取数据。</span><span class="sxs-lookup"><span data-stu-id="097cc-143">The following example changes the behavior of the component to fetch data from a specific query.</span></span>

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="css-custom-properties"></a><span data-ttu-id="097cc-144">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="097cc-144">CSS custom properties</span></span>

<span data-ttu-id="097cc-145">`mgt-agenda`组件定义这些 CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="097cc-145">The `mgt-agenda` component defines these CSS custom properties</span></span>

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

<span data-ttu-id="097cc-146">若要了解详细信息，请参阅[样式组件](../style.md)。</span><span class="sxs-lookup"><span data-stu-id="097cc-146">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="097cc-147">模板</span><span class="sxs-lookup"><span data-stu-id="097cc-147">Templates</span></span>

<span data-ttu-id="097cc-148">组件支持多个[模板](../templates.md)，这些模板允许您替换组件的某些部分。 `mgt-agenda`</span><span class="sxs-lookup"><span data-stu-id="097cc-148">The `mgt-agenda` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="097cc-149">若要指定模板，请在`<template>`组件内添加一个元素，并将`data-type`值设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="097cc-149">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="097cc-150">数据类型</span><span class="sxs-lookup"><span data-stu-id="097cc-150">Data type</span></span> | <span data-ttu-id="097cc-151">数据上下文</span><span class="sxs-lookup"><span data-stu-id="097cc-151">Data context</span></span> | <span data-ttu-id="097cc-152">说明</span><span class="sxs-lookup"><span data-stu-id="097cc-152">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="097cc-153">`events`：事件对象的列表</span><span class="sxs-lookup"><span data-stu-id="097cc-153">`events`: list of event objects</span></span> | <span data-ttu-id="097cc-154">默认模板会将整个组件替换为您自己的组件。</span><span class="sxs-lookup"><span data-stu-id="097cc-154">The default template replaces the entire component with your own.</span></span> |
| `event` | <span data-ttu-id="097cc-155">`event`： event 对象</span><span class="sxs-lookup"><span data-stu-id="097cc-155">`event`: event object</span></span> | <span data-ttu-id="097cc-156">用于呈现每个事件的模板。</span><span class="sxs-lookup"><span data-stu-id="097cc-156">The template used to render each event.</span></span> |
| `header` | <span data-ttu-id="097cc-157">`header`： string</span><span class="sxs-lookup"><span data-stu-id="097cc-157">`header`: string</span></span> | <span data-ttu-id="097cc-158">用于呈现每天的标题的模板。</span><span class="sxs-lookup"><span data-stu-id="097cc-158">The template used to render the header for each day.</span></span> |
| `other` | <span data-ttu-id="097cc-159">`event`： event 对象</span><span class="sxs-lookup"><span data-stu-id="097cc-159">`event`: event object</span></span> | <span data-ttu-id="097cc-160">用于呈现每个事件的其他内容的模板。</span><span class="sxs-lookup"><span data-stu-id="097cc-160">The template used to render additional content for each event.</span></span> |
| `no-data` | <span data-ttu-id="097cc-161">不传递数据上下文</span><span class="sxs-lookup"><span data-stu-id="097cc-161">No data context is passed</span></span> | <span data-ttu-id="097cc-162">没有可用事件时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="097cc-162">The template used when no events are available.</span></span> |
| `loading` | <span data-ttu-id="097cc-163">不传递数据上下文</span><span class="sxs-lookup"><span data-stu-id="097cc-163">No data context is passed</span></span> | <span data-ttu-id="097cc-164">加载数据时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="097cc-164">The template used when data is loading.</span></span> |

<span data-ttu-id="097cc-165">下面的示例演示如何使用`event`模板：</span><span class="sxs-lookup"><span data-stu-id="097cc-165">The following examples illustrates how to use the `event` template:</span></span>

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

<span data-ttu-id="097cc-166">若要了解详细信息，请参阅[模板](../templates.md)。</span><span class="sxs-lookup"><span data-stu-id="097cc-166">To learn more, see [templates](../templates.md).</span></span>

## <a name="events"></a><span data-ttu-id="097cc-167">活动</span><span class="sxs-lookup"><span data-stu-id="097cc-167">Events</span></span>

<span data-ttu-id="097cc-168">从控件触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="097cc-168">The following events are fired from the control.</span></span>

| <span data-ttu-id="097cc-169">事件</span><span class="sxs-lookup"><span data-stu-id="097cc-169">Event</span></span> | <span data-ttu-id="097cc-170">说明</span><span class="sxs-lookup"><span data-stu-id="097cc-170">Description</span></span> |
| --- | --- |
| <span data-ttu-id="097cc-171">eventClick</span><span class="sxs-lookup"><span data-stu-id="097cc-171">eventClick</span></span> | <span data-ttu-id="097cc-172">用户单击或点击事件。</span><span class="sxs-lookup"><span data-stu-id="097cc-172">The user clicks or taps on an event.</span></span>|


## <a name="graph-scopes"></a><span data-ttu-id="097cc-173">图表范围</span><span class="sxs-lookup"><span data-stu-id="097cc-173">Graph scopes</span></span>

<span data-ttu-id="097cc-174">此组件使用以下 Microsoft Graph Api 和权限：</span><span class="sxs-lookup"><span data-stu-id="097cc-174">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="097cc-175">resource</span><span class="sxs-lookup"><span data-stu-id="097cc-175">resource</span></span> | <span data-ttu-id="097cc-176">权限/范围</span><span class="sxs-lookup"><span data-stu-id="097cc-176">permission/scope</span></span> |
| - | - |
| [<span data-ttu-id="097cc-177">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="097cc-177">/me/calendarview</span></span>](/graph/api/calendar-list-calendarview?view=graph-rest-1.0) | `Calendars.Read` |

<span data-ttu-id="097cc-178">组件允许您指定要调用的其他 Microsoft Graph 查询（例如`/groups/{id}/calendar/calendarView`）。</span><span class="sxs-lookup"><span data-stu-id="097cc-178">The component allows you to specify a different Microsoft Graph query to call (such as `/groups/{id}/calendar/calendarView`).</span></span> <span data-ttu-id="097cc-179">在这种情况下，将作用域追加到字符串的末尾，并将其分隔`|`</span><span class="sxs-lookup"><span data-stu-id="097cc-179">In this case, append the scope at the end of the string, delimited by `|`</span></span>

## <a name="authentication"></a><span data-ttu-id="097cc-180">身份验证</span><span class="sxs-lookup"><span data-stu-id="097cc-180">Authentication</span></span>

<span data-ttu-id="097cc-181">登录控件利用[身份验证文档](./../providers.md)中所述的全局验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="097cc-181">The login control leverages the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

