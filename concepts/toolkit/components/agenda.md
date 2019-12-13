---
title: Microsoft Graph 工具包中的 "议程" 组件
description: "\"管理中心议程\" web 组件用于表示用户或组日历中的事件。"
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 7f46602396ab794593101505d56c14b675db235f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955895"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="f4b17-103">Microsoft Graph 工具包中的 "议程" 组件</span><span class="sxs-lookup"><span data-stu-id="f4b17-103">Agenda component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="f4b17-104">`mgt-agenda` Web 组件表示用户或组日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="f4b17-104">The `mgt-agenda` web component represents events in a user or group calendar.</span></span> <span data-ttu-id="f4b17-105">默认情况下，日历会在当前日期的用户事件中显示当前登录的用户事件。</span><span class="sxs-lookup"><span data-stu-id="f4b17-105">By default, the calendar displays the current signed in user events for the current day.</span></span> <span data-ttu-id="f4b17-106">组件还可以使用从 Microsoft Graph 返回事件的任何终结点。</span><span class="sxs-lookup"><span data-stu-id="f4b17-106">The component can also use any endpoint that returns events from Microsoft Graph.</span></span> 

## <a name="example"></a><span data-ttu-id="f4b17-107">示例</span><span class="sxs-lookup"><span data-stu-id="f4b17-107">Example</span></span>

[<span data-ttu-id="f4b17-108">jsfiddle 示例</span><span class="sxs-lookup"><span data-stu-id="f4b17-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/ojt2c7vp/)

```html
<mgt-agenda group-by-day></mgt-agenda>
```

![计划-议程](./images/mgt-agenda.png)

## <a name="properties"></a><span data-ttu-id="f4b17-110">属性</span><span class="sxs-lookup"><span data-stu-id="f4b17-110">Properties</span></span>

<span data-ttu-id="f4b17-111">默认情况下， `mgt-agenda`组件从`/me/calendarview`终结点提取事件并显示当天的事件。</span><span class="sxs-lookup"><span data-stu-id="f4b17-111">By default, the `mgt-agenda` component fetches events from the `/me/calendarview` endpoint and displays events for the current day.</span></span> <span data-ttu-id="f4b17-112">有几个可用于更改此行为的属性。</span><span class="sxs-lookup"><span data-stu-id="f4b17-112">There are several properties you can use to change this behavior.</span></span>

| <span data-ttu-id="f4b17-113">属性</span><span class="sxs-lookup"><span data-stu-id="f4b17-113">Attribute</span></span> | <span data-ttu-id="f4b17-114">属性</span><span class="sxs-lookup"><span data-stu-id="f4b17-114">Property</span></span> | <span data-ttu-id="f4b17-115">说明</span><span class="sxs-lookup"><span data-stu-id="f4b17-115">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="f4b17-116">date</span><span class="sxs-lookup"><span data-stu-id="f4b17-116">date</span></span> | <span data-ttu-id="f4b17-117">date</span><span class="sxs-lookup"><span data-stu-id="f4b17-117">date</span></span> | <span data-ttu-id="f4b17-118">一个字符串，表示要从 Microsoft Graph 中提取的事件的开始日期。</span><span class="sxs-lookup"><span data-stu-id="f4b17-118">A string that represents the start date of the events to fetch from Microsoft Graph.</span></span> <span data-ttu-id="f4b17-119">值应采用可由[日期构造函数](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)进行分析的格式，如果`event-query`设置了属性，则值不起作用。</span><span class="sxs-lookup"><span data-stu-id="f4b17-119">Value should be in a format that can be parsed by the [Date constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="f4b17-120">之前</span><span class="sxs-lookup"><span data-stu-id="f4b17-120">days</span></span> | <span data-ttu-id="f4b17-121">之前</span><span class="sxs-lookup"><span data-stu-id="f4b17-121">days</span></span> | <span data-ttu-id="f4b17-122">从 Microsoft Graph 提取的天数-默认值为3。如果`event-query`设置了属性，则此值不起作用。</span><span class="sxs-lookup"><span data-stu-id="f4b17-122">A number of days to fetch from Microsoft Graph - default is 3 - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="f4b17-123">show-max</span><span class="sxs-lookup"><span data-stu-id="f4b17-123">show-max</span></span> | <span data-ttu-id="f4b17-124">showMax</span><span class="sxs-lookup"><span data-stu-id="f4b17-124">showMax</span></span> | <span data-ttu-id="f4b17-125">一个数字，用于指示要显示的最大事件数。</span><span class="sxs-lookup"><span data-stu-id="f4b17-125">A number to indicate the maximum number of events to show.</span></span> <span data-ttu-id="f4b17-126">未设置默认值（无最大值）。</span><span class="sxs-lookup"><span data-stu-id="f4b17-126">The default value is not set (no maximum).</span></span> |
| <span data-ttu-id="f4b17-127">组 id</span><span class="sxs-lookup"><span data-stu-id="f4b17-127">group-id</span></span> | <span data-ttu-id="f4b17-128">groupId</span><span class="sxs-lookup"><span data-stu-id="f4b17-128">groupId</span></span> | <span data-ttu-id="f4b17-129">要使用的组日历的字符串 ID，而不是当前登录的用户日历。</span><span class="sxs-lookup"><span data-stu-id="f4b17-129">A string ID for a group calendar to use instead of the current signed in user's calendar.</span></span> |
| <span data-ttu-id="f4b17-130">事件查询</span><span class="sxs-lookup"><span data-stu-id="f4b17-130">event-query</span></span> | <span data-ttu-id="f4b17-131">eventQuery</span><span class="sxs-lookup"><span data-stu-id="f4b17-131">eventQuery</span></span> | <span data-ttu-id="f4b17-132">一个字符串，表示从 Microsoft Graph 提取事件时要使用的替代查询。</span><span class="sxs-lookup"><span data-stu-id="f4b17-132">A string that represents an alternative query to be used when fetching events from Microsoft Graph.</span></span> <span data-ttu-id="f4b17-133">（可选）通过将委派作用域与`|` （`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`）分隔来将其添加到字符串的末尾。</span><span class="sxs-lookup"><span data-stu-id="f4b17-133">Optionally, add the delegated scope at the end of the string by delimiting it with `|` (`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`).</span></span> |
| <span data-ttu-id="f4b17-134">活动</span><span class="sxs-lookup"><span data-stu-id="f4b17-134">events</span></span> | <span data-ttu-id="f4b17-135">活动</span><span class="sxs-lookup"><span data-stu-id="f4b17-135">events</span></span> | <span data-ttu-id="f4b17-136">一个事件数组，用于获取或设置组件呈现的事件的列表-使用此属性可访问组件加载的事件。</span><span class="sxs-lookup"><span data-stu-id="f4b17-136">An array of events to get or set the list of events rendered by the component - use this property to access the events loaded by the component.</span></span> <span data-ttu-id="f4b17-137">将此值设置为加载您自己的事件-如果值是由开发人员`date`设置`days`的， `event-query`则、或属性不起作用。</span><span class="sxs-lookup"><span data-stu-id="f4b17-137">Set this value to load your own events - if value is set by developer, the `date`, `days`, or `event-query` attributes have no effect.</span></span> |
| <span data-ttu-id="f4b17-138">逐天分组</span><span class="sxs-lookup"><span data-stu-id="f4b17-138">group-by-day</span></span> | <span data-ttu-id="f4b17-139">groupByDay</span><span class="sxs-lookup"><span data-stu-id="f4b17-139">groupByDay</span></span> | <span data-ttu-id="f4b17-140">按天对事件分组的布尔值不按默认事件进行分组。</span><span class="sxs-lookup"><span data-stu-id="f4b17-140">A Boolean value to group events by day - by default events are not grouped.</span></span> |

<span data-ttu-id="f4b17-141">下面的示例更改组件的行为，以获取特定日期的数据，最长为三天。</span><span class="sxs-lookup"><span data-stu-id="f4b17-141">The following example changes the behavior of the component to fetch data for a specific date and up to three days.</span></span>

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

<span data-ttu-id="f4b17-142">下面的示例将更改组件的行为，以从特定查询中获取数据。</span><span class="sxs-lookup"><span data-stu-id="f4b17-142">The following example changes the behavior of the component to fetch data from a specific query.</span></span>

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="css-custom-properties"></a><span data-ttu-id="f4b17-143">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="f4b17-143">CSS custom properties</span></span>

<span data-ttu-id="f4b17-144">`mgt-agenda`组件定义这些 CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="f4b17-144">The `mgt-agenda` component defines these CSS custom properties</span></span>

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

<span data-ttu-id="f4b17-145">若要了解详细信息，请参阅[样式组件](../style.md)。</span><span class="sxs-lookup"><span data-stu-id="f4b17-145">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="f4b17-146">模板</span><span class="sxs-lookup"><span data-stu-id="f4b17-146">Templates</span></span>

<span data-ttu-id="f4b17-147">组件支持多个[模板](../templates.md)，这些模板允许您替换组件的某些部分。 `mgt-agenda`</span><span class="sxs-lookup"><span data-stu-id="f4b17-147">The `mgt-agenda` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="f4b17-148">若要指定模板，请在`<template>`组件内添加一个元素，并将`data-type`值设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="f4b17-148">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="f4b17-149">数据类型</span><span class="sxs-lookup"><span data-stu-id="f4b17-149">Data type</span></span> | <span data-ttu-id="f4b17-150">数据上下文</span><span class="sxs-lookup"><span data-stu-id="f4b17-150">Data context</span></span> | <span data-ttu-id="f4b17-151">说明</span><span class="sxs-lookup"><span data-stu-id="f4b17-151">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="f4b17-152">`events`：事件对象的列表</span><span class="sxs-lookup"><span data-stu-id="f4b17-152">`events`: list of event objects</span></span> | <span data-ttu-id="f4b17-153">默认模板会将整个组件替换为您自己的组件。</span><span class="sxs-lookup"><span data-stu-id="f4b17-153">The default template replaces the entire component with your own.</span></span> |
| `event` | <span data-ttu-id="f4b17-154">`event`： event 对象</span><span class="sxs-lookup"><span data-stu-id="f4b17-154">`event`: event object</span></span> | <span data-ttu-id="f4b17-155">用于呈现每个事件的模板。</span><span class="sxs-lookup"><span data-stu-id="f4b17-155">The template used to render each event.</span></span> |
| `header` | <span data-ttu-id="f4b17-156">`header`： string</span><span class="sxs-lookup"><span data-stu-id="f4b17-156">`header`: string</span></span> | <span data-ttu-id="f4b17-157">用于呈现每天的标题的模板。</span><span class="sxs-lookup"><span data-stu-id="f4b17-157">The template used to render the header for each day.</span></span> |
| `other` | <span data-ttu-id="f4b17-158">`event`： event 对象</span><span class="sxs-lookup"><span data-stu-id="f4b17-158">`event`: event object</span></span> | <span data-ttu-id="f4b17-159">用于呈现每个事件的其他内容的模板。</span><span class="sxs-lookup"><span data-stu-id="f4b17-159">The template used to render additional content for each event.</span></span> |
| `no-data` | <span data-ttu-id="f4b17-160">不传递数据上下文</span><span class="sxs-lookup"><span data-stu-id="f4b17-160">No data context is passed</span></span> | <span data-ttu-id="f4b17-161">没有可用事件时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="f4b17-161">The template used when no events are available.</span></span> |
| `loading` | <span data-ttu-id="f4b17-162">不传递数据上下文</span><span class="sxs-lookup"><span data-stu-id="f4b17-162">No data context is passed</span></span> | <span data-ttu-id="f4b17-163">加载数据时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="f4b17-163">The template used when data is loading.</span></span> |

<span data-ttu-id="f4b17-164">下面的示例演示如何使用`event`模板：</span><span class="sxs-lookup"><span data-stu-id="f4b17-164">The following examples illustrates how to use the `event` template:</span></span>

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

<span data-ttu-id="f4b17-165">若要了解详细信息，请参阅[模板](../templates.md)。</span><span class="sxs-lookup"><span data-stu-id="f4b17-165">To learn more, see [templates](../templates.md).</span></span>

## <a name="events"></a><span data-ttu-id="f4b17-166">事件</span><span class="sxs-lookup"><span data-stu-id="f4b17-166">Events</span></span>

<span data-ttu-id="f4b17-167">从控件触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="f4b17-167">The following events are fired from the control.</span></span>

| <span data-ttu-id="f4b17-168">事件</span><span class="sxs-lookup"><span data-stu-id="f4b17-168">Event</span></span> | <span data-ttu-id="f4b17-169">说明</span><span class="sxs-lookup"><span data-stu-id="f4b17-169">Description</span></span> |
| --- | --- |
| <span data-ttu-id="f4b17-170">eventClick</span><span class="sxs-lookup"><span data-stu-id="f4b17-170">eventClick</span></span> | <span data-ttu-id="f4b17-171">用户单击或点击事件。</span><span class="sxs-lookup"><span data-stu-id="f4b17-171">The user clicks or taps on an event.</span></span>|


## <a name="graph-scopes"></a><span data-ttu-id="f4b17-172">图表范围</span><span class="sxs-lookup"><span data-stu-id="f4b17-172">Graph scopes</span></span>

<span data-ttu-id="f4b17-173">此组件使用以下 Microsoft Graph Api 和权限：</span><span class="sxs-lookup"><span data-stu-id="f4b17-173">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="f4b17-174">resource</span><span class="sxs-lookup"><span data-stu-id="f4b17-174">resource</span></span> | <span data-ttu-id="f4b17-175">权限/范围</span><span class="sxs-lookup"><span data-stu-id="f4b17-175">permission/scope</span></span> |
| - | - |
| [<span data-ttu-id="f4b17-176">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="f4b17-176">/me/calendarview</span></span>](https://docs.microsoft.com/graph/api/calendar-list-calendarview?view=graph-rest-1.0) | `Calendars.Read` |

<span data-ttu-id="f4b17-177">组件允许您指定要调用的其他 Microsoft Graph 查询（例如`/groups/{id}/calendar/calendarView`）。</span><span class="sxs-lookup"><span data-stu-id="f4b17-177">The component allows you to specify a different Microsoft Graph query to call (such as `/groups/{id}/calendar/calendarView`).</span></span> <span data-ttu-id="f4b17-178">在这种情况下，将作用域追加到字符串的末尾，并将其分隔`|`</span><span class="sxs-lookup"><span data-stu-id="f4b17-178">In this case, append the scope at the end of the string, delimited by `|`</span></span>

## <a name="authentication"></a><span data-ttu-id="f4b17-179">身份验证</span><span class="sxs-lookup"><span data-stu-id="f4b17-179">Authentication</span></span>

<span data-ttu-id="f4b17-180">登录控件利用[身份验证文档](./../providers.md)中所述的全局验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="f4b17-180">The login control leverages the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 

