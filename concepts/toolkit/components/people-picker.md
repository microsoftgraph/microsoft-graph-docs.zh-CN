---
title: 人员-选取器组件
description: 您可以使用 "人员-选取器 web 组件" 搜索指定数量的人员，并通过 Microsoft Graph 呈现结果列表。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 2a0680a70ddfd5410e82911e5280c0b1a7e7dcaf
ms.sourcegitcommit: 3e7769ad097e9c34233fa5fea83afa23c34e14a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822793"
---
# <a name="people-picker-component"></a><span data-ttu-id="5b47f-103">人员-选取器组件</span><span class="sxs-lookup"><span data-stu-id="5b47f-103">People-Picker component</span></span>

<span data-ttu-id="5b47f-104">您可以使用`mgt-people-picker` web 组件搜索指定数量的人员，并通过 Microsoft Graph 呈现结果列表。</span><span class="sxs-lookup"><span data-stu-id="5b47f-104">You can use the `mgt-people-picker` web component search for a specified number of people and render the list of results via Microsoft Graph.</span></span> <span data-ttu-id="5b47f-105">默认情况下，组件将搜索所有人员;您还可以定义组属性以进一步筛选结果。</span><span class="sxs-lookup"><span data-stu-id="5b47f-105">By default, the component will search for all people; you can also define a group property to further filter the results.</span></span>

<span data-ttu-id="5b47f-106">如果要显示的用户数超过此`show-max`值，则不会在搜索列表中显示所有返回的人员数。</span><span class="sxs-lookup"><span data-stu-id="5b47f-106">If the number of people to display exceeds the `show-max` value, not all people returned will be displayed in the search list.</span></span>

## <a name="example"></a><span data-ttu-id="5b47f-107">示例</span><span class="sxs-lookup"><span data-stu-id="5b47f-107">Example</span></span>

[<span data-ttu-id="5b47f-108">jsfiddle 示例</span><span class="sxs-lookup"><span data-stu-id="5b47f-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/jdv38fg0/)

```html
<mgt-people-picker></mgt-people-picker>
```

![组织-人员-选取器](./images/mgt-people-picker-image.png)

## <a name="properties"></a><span data-ttu-id="5b47f-110">属性</span><span class="sxs-lookup"><span data-stu-id="5b47f-110">Properties</span></span>

<span data-ttu-id="5b47f-111">默认情况下， `mgt-people-picker`组件从`/me/people`终结点提取事件。</span><span class="sxs-lookup"><span data-stu-id="5b47f-111">By default, the `mgt-people-picker` component fetches events from the `/me/people` endpoint.</span></span> <span data-ttu-id="5b47f-112">使用以下属性来更改此行为。</span><span class="sxs-lookup"><span data-stu-id="5b47f-112">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="5b47f-113">属性</span><span class="sxs-lookup"><span data-stu-id="5b47f-113">Property</span></span> | <span data-ttu-id="5b47f-114">属性</span><span class="sxs-lookup"><span data-stu-id="5b47f-114">Attribute</span></span> | <span data-ttu-id="5b47f-115">说明</span><span class="sxs-lookup"><span data-stu-id="5b47f-115">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="5b47f-116">showMax</span><span class="sxs-lookup"><span data-stu-id="5b47f-116">showMax</span></span>  | <span data-ttu-id="5b47f-117">show-max</span><span class="sxs-lookup"><span data-stu-id="5b47f-117">show-max</span></span>  | <span data-ttu-id="5b47f-118">一个整数值，指示要显示的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="5b47f-118">An integer value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="5b47f-119">默认值为6。</span><span class="sxs-lookup"><span data-stu-id="5b47f-119">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="5b47f-120">people</span><span class="sxs-lookup"><span data-stu-id="5b47f-120">people</span></span>   | <span data-ttu-id="5b47f-121">people</span><span class="sxs-lookup"><span data-stu-id="5b47f-121">people</span></span>    | <span data-ttu-id="5b47f-122">获取或设置组件呈现的人员列表的人员数组。</span><span class="sxs-lookup"><span data-stu-id="5b47f-122">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="5b47f-123">使用此属性可访问组件加载的人员。</span><span class="sxs-lookup"><span data-stu-id="5b47f-123">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="5b47f-124">设置此值可加载自己的人员。</span><span class="sxs-lookup"><span data-stu-id="5b47f-124">Set this value to load your own people.</span></span> |
| <span data-ttu-id="5b47f-125">group</span><span class="sxs-lookup"><span data-stu-id="5b47f-125">group</span></span>    | <span data-ttu-id="5b47f-126">group</span><span class="sxs-lookup"><span data-stu-id="5b47f-126">group</span></span>     | <span data-ttu-id="5b47f-127">一个 string 值，属于 Microsoft Graph 定义的组，用于进一步筛选搜索结果。</span><span class="sxs-lookup"><span data-stu-id="5b47f-127">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |

<span data-ttu-id="5b47f-128">示例如下。</span><span class="sxs-lookup"><span data-stu-id="5b47f-128">The following is an example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="css-custom-properties"></a><span data-ttu-id="5b47f-129">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="5b47f-129">CSS custom properties</span></span>

<span data-ttu-id="5b47f-130">`mgt-people-picker`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="5b47f-130">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="5b47f-131">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="5b47f-131">Microsoft Graph permissions</span></span>

<span data-ttu-id="5b47f-132">此组件使用以下 Microsoft Graph Api 和权限。</span><span class="sxs-lookup"><span data-stu-id="5b47f-132">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="5b47f-133">API</span><span class="sxs-lookup"><span data-stu-id="5b47f-133">API</span></span>                                                                                                              | <span data-ttu-id="5b47f-134">权限</span><span class="sxs-lookup"><span data-stu-id="5b47f-134">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="5b47f-135">/me/people</span><span class="sxs-lookup"><span data-stu-id="5b47f-135">/me/people</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="5b47f-136">People.Read</span><span class="sxs-lookup"><span data-stu-id="5b47f-136">People.Read</span></span> |
| [<span data-ttu-id="5b47f-137">/groups/\${groupId}/members</span><span class="sxs-lookup"><span data-stu-id="5b47f-137">/groups/\${groupId}/members</span></span>](https://docs.microsoft.com/en-us/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="5b47f-138">People.Read</span><span class="sxs-lookup"><span data-stu-id="5b47f-138">People.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="5b47f-139">身份验证</span><span class="sxs-lookup"><span data-stu-id="5b47f-139">Authentication</span></span>

<span data-ttu-id="5b47f-140">该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="5b47f-140">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
