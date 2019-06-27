---
title: Microsoft Graph 工具包中的 "议程" 组件
description: "\"管理中心议程\" web 组件用于表示用户或组日历中的事件。"
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 8a91b20a48c1646fafd8cd7a287f037615024a73
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242974"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="c6494-103">Microsoft Graph 工具包中的 "议程" 组件</span><span class="sxs-lookup"><span data-stu-id="c6494-103">Agenda component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="c6494-104">`mgt-agenda` Web 组件表示用户或组日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="c6494-104">The `mgt-agenda` web component represents events in a user or group calendar.</span></span> <span data-ttu-id="c6494-105">默认情况下, 日历会在当前日期的用户事件中显示当前登录的用户事件。</span><span class="sxs-lookup"><span data-stu-id="c6494-105">By default, the calendar displays the current signed in user events for the current day.</span></span> <span data-ttu-id="c6494-106">组件还可以使用从 Microsoft Graph 返回事件的任何终结点。</span><span class="sxs-lookup"><span data-stu-id="c6494-106">The component can also use any endpoint that returns events from Microsoft Graph.</span></span> 

## <a name="example"></a><span data-ttu-id="c6494-107">示例</span><span class="sxs-lookup"><span data-stu-id="c6494-107">Example</span></span>

[<span data-ttu-id="c6494-108">jsfiddle 示例</span><span class="sxs-lookup"><span data-stu-id="c6494-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/ojt2c7vp/)

```html
<mgt-agenda group-by-day></mgt-agenda>
```

![计划-议程](./images/mgt-agenda.png)

## <a name="properties"></a><span data-ttu-id="c6494-110">属性</span><span class="sxs-lookup"><span data-stu-id="c6494-110">Properties</span></span>

<span data-ttu-id="c6494-111">默认情况下, `mgt-agenda`组件从`/me/calendarview`终结点提取事件并显示当天的事件。</span><span class="sxs-lookup"><span data-stu-id="c6494-111">By default, the `mgt-agenda` component fetches events from the `/me/calendarview` endpoint and displays events for the current day.</span></span> <span data-ttu-id="c6494-112">有几个可用于更改此行为的属性。</span><span class="sxs-lookup"><span data-stu-id="c6494-112">There are several properties you can use to change this behavior.</span></span>

| <span data-ttu-id="c6494-113">属性</span><span class="sxs-lookup"><span data-stu-id="c6494-113">Property</span></span> | <span data-ttu-id="c6494-114">属性</span><span class="sxs-lookup"><span data-stu-id="c6494-114">Attribute</span></span> | <span data-ttu-id="c6494-115">说明</span><span class="sxs-lookup"><span data-stu-id="c6494-115">Description</span></span> |
| --- | --- | --- |
| `groupByDay` | `group-by-day` | <span data-ttu-id="c6494-116">按天对事件分组的布尔值不按默认事件进行分组。</span><span class="sxs-lookup"><span data-stu-id="c6494-116">A Boolean value to group events by day - by default events are not grouped.</span></span> |
| `date` | `date` | <span data-ttu-id="c6494-117">一个字符串, 表示要从 Microsoft Graph 中提取的事件的开始日期。</span><span class="sxs-lookup"><span data-stu-id="c6494-117">A string that represents the start date of the events to fetch from Microsoft Graph.</span></span> <span data-ttu-id="c6494-118">值应采用可由[日期构造函数](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)进行分析的格式, 如果`event-query`设置了属性, 则值不起作用。</span><span class="sxs-lookup"><span data-stu-id="c6494-118">Value should be in a format that can be parsed by the [Date constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) - value has no effect if `event-query` attribute is set.</span></span> |
| `days` | `days` | <span data-ttu-id="c6494-119">从 Microsoft Graph 提取的天数-默认值为3。如果`event-query`设置了属性, 则此值不起作用。</span><span class="sxs-lookup"><span data-stu-id="c6494-119">A number of days to fetch from Microsoft Graph - default is 3 - value has no effect if `event-query` attribute is set.</span></span> |
| `eventQuery` | `event-query` | <span data-ttu-id="c6494-120">一个字符串, 表示从 Microsoft Graph 提取事件时要使用的替代查询。</span><span class="sxs-lookup"><span data-stu-id="c6494-120">A string that represents an alternative query to be used when fetching events from Microsoft Graph.</span></span> <span data-ttu-id="c6494-121">(可选) 通过将委派作用域与`|` (`"/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all"`) 分隔来将其添加到字符串的末尾。</span><span class="sxs-lookup"><span data-stu-id="c6494-121">Optionally, add the delegated scope at the end of the string by delimiting it with `|` (`"/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all"`).</span></span> |
| `events` | `events` | <span data-ttu-id="c6494-122">一个事件数组, 用于获取或设置组件呈现的事件的列表-使用此属性可访问组件加载的事件。</span><span class="sxs-lookup"><span data-stu-id="c6494-122">An array of events to get or set the list of events rendered by the component - use this property to access the events loaded by the component.</span></span> <span data-ttu-id="c6494-123">将此值设置为加载您自己的事件-如果值是由开发人员`date`设置`days`的, `event-query`则、或属性不起作用。</span><span class="sxs-lookup"><span data-stu-id="c6494-123">Set this value to load your own events - if value is set by developer, the `date`, `days`, or `event-query` attributes have no effect.</span></span> |

<span data-ttu-id="c6494-124">下面的示例更改组件的行为, 以获取特定日期的数据, 最长为3天。</span><span class="sxs-lookup"><span data-stu-id="c6494-124">The following example changes the behavior of the component to fetch data for a specific date and up to 3 days.</span></span>

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

<span data-ttu-id="c6494-125">下面的示例将更改组件的行为, 以从特定查询中获取数据。</span><span class="sxs-lookup"><span data-stu-id="c6494-125">The following example changes the behavior of the component to fetch data from a specific query.</span></span>

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="css-custom-properties"></a><span data-ttu-id="c6494-126">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="c6494-126">CSS Custom properties</span></span>

<span data-ttu-id="c6494-127">`mgt-agenda`组件定义这些 CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="c6494-127">The `mgt-agenda` component defines these CSS custom properties</span></span>

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

<span data-ttu-id="c6494-128">若要了解详细信息, 请参阅[样式组件](../style.md)。</span><span class="sxs-lookup"><span data-stu-id="c6494-128">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="c6494-129">模板</span><span class="sxs-lookup"><span data-stu-id="c6494-129">Templates</span></span>

<span data-ttu-id="c6494-130">组件支持多个[模板](../templates.md), 这些模板允许您替换组件的某些部分。 `mgt-agenda`</span><span class="sxs-lookup"><span data-stu-id="c6494-130">The `mgt-agenda` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="c6494-131">若要指定模板, 请在`<template>`组件内添加一个元素, 并将`data-type`值设置为下列值之一:</span><span class="sxs-lookup"><span data-stu-id="c6494-131">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="c6494-132">数据类型</span><span class="sxs-lookup"><span data-stu-id="c6494-132">Data type</span></span> | <span data-ttu-id="c6494-133">数据上下文</span><span class="sxs-lookup"><span data-stu-id="c6494-133">Data context</span></span> | <span data-ttu-id="c6494-134">说明</span><span class="sxs-lookup"><span data-stu-id="c6494-134">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="c6494-135">`events`: 事件对象的列表</span><span class="sxs-lookup"><span data-stu-id="c6494-135">`events`: list of event objects</span></span> | <span data-ttu-id="c6494-136">默认模板会将整个组件替换为您自己的组件。</span><span class="sxs-lookup"><span data-stu-id="c6494-136">The default template replaces the entire component with your own.</span></span> |
| `event` | <span data-ttu-id="c6494-137">`event`: event 对象</span><span class="sxs-lookup"><span data-stu-id="c6494-137">`event`: event object</span></span> | <span data-ttu-id="c6494-138">用于呈现每个事件的模板。</span><span class="sxs-lookup"><span data-stu-id="c6494-138">The template used to render each event.</span></span> |
| `header` | <span data-ttu-id="c6494-139">`header`: string</span><span class="sxs-lookup"><span data-stu-id="c6494-139">`header`: string</span></span> | <span data-ttu-id="c6494-140">用于呈现每天的标题的模板。</span><span class="sxs-lookup"><span data-stu-id="c6494-140">The template used to render the header for each day.</span></span> |
| `other` | <span data-ttu-id="c6494-141">`event`: event 对象</span><span class="sxs-lookup"><span data-stu-id="c6494-141">`event`: event object</span></span> | <span data-ttu-id="c6494-142">用于呈现每个事件的其他内容的模板。</span><span class="sxs-lookup"><span data-stu-id="c6494-142">The template used to render additional content for each event.</span></span> |
| `no-data` | <span data-ttu-id="c6494-143">不传递数据上下文</span><span class="sxs-lookup"><span data-stu-id="c6494-143">No data context is passed</span></span> | <span data-ttu-id="c6494-144">没有可用事件时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="c6494-144">The template used when no events are available.</span></span> |
| `loading` | <span data-ttu-id="c6494-145">不传递数据上下文</span><span class="sxs-lookup"><span data-stu-id="c6494-145">No data context is passed</span></span> | <span data-ttu-id="c6494-146">加载数据时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="c6494-146">The template used when data is loading.</span></span> |

<span data-ttu-id="c6494-147">下面的示例演示如何使用`event`模板:</span><span class="sxs-lookup"><span data-stu-id="c6494-147">The following examples illustrates how to use the `event` template:</span></span>

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

<span data-ttu-id="c6494-148">若要了解详细信息, 请参阅[模板](../templates.md)。</span><span class="sxs-lookup"><span data-stu-id="c6494-148">To learn more, see [templates](../templates.md).</span></span>

## <a name="graph-scopes"></a><span data-ttu-id="c6494-149">图表范围</span><span class="sxs-lookup"><span data-stu-id="c6494-149">Graph scopes</span></span>

<span data-ttu-id="c6494-150">此组件使用以下 Microsoft Graph Api 和权限:</span><span class="sxs-lookup"><span data-stu-id="c6494-150">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="c6494-151">resource</span><span class="sxs-lookup"><span data-stu-id="c6494-151">resource</span></span> | <span data-ttu-id="c6494-152">权限/范围</span><span class="sxs-lookup"><span data-stu-id="c6494-152">permission/scope</span></span> |
| - | - |
| [<span data-ttu-id="c6494-153">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="c6494-153">/me/calendarview</span></span>](https://docs.microsoft.com/en-us/graph/api/calendar-list-calendarview?view=graph-rest-1.0) | `Calendars.Read` |

<span data-ttu-id="c6494-154">组件允许您指定要调用的其他 Microsoft Graph 查询 (例如`/groups/{id}/calendar/calendarView`)。</span><span class="sxs-lookup"><span data-stu-id="c6494-154">The component allows you to specify a different Microsoft Graph query to call (such as `/groups/{id}/calendar/calendarView`).</span></span> <span data-ttu-id="c6494-155">在这种情况下, 将作用域追加到字符串的末尾, 并将其分隔`|`</span><span class="sxs-lookup"><span data-stu-id="c6494-155">In this case, append the scope at the end of the string, delimited by `|`</span></span>

## <a name="authentication"></a><span data-ttu-id="c6494-156">身份验证</span><span class="sxs-lookup"><span data-stu-id="c6494-156">Authentication</span></span>

<span data-ttu-id="c6494-157">登录控件利用[身份验证文档](./../providers.md)中所述的全局验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="c6494-157">The login control leverages the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 

