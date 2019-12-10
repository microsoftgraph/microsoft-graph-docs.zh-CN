---
title: 获取 Microsoft Graph 工具包中的组件
description: 通过获取组件，可以在 HTML 中直接在 Microsoft Graph 中进行任何 GET 查询。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 77beb3940eb29a2c9158fba88d78084639e433ed
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39921696"
---
# <a name="get-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="e9d7b-103">获取 Microsoft Graph 工具包中的组件</span><span class="sxs-lookup"><span data-stu-id="e9d7b-103">Get component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="e9d7b-104">您可以使用`mgt-get`从 Microsoft Graph 直接在 HTML 中进行任何 GET 查询。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-104">You can use `mgt-get` to make any GET query from Microsoft Graph directly in your HTML.</span></span> <span data-ttu-id="e9d7b-105">组件不提供默认 UI，需要您编写模板。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-105">The component does not provide a default UI and requires that you write a template.</span></span>

## <a name="example"></a><span data-ttu-id="e9d7b-106">示例</span><span class="sxs-lookup"><span data-stu-id="e9d7b-106">Example</span></span>

```html
<mgt-get resource="/me/messages" version="beta" scopes="mail.read" max-pages="2">
  <template>
    emails: {{value.length}}
  </template>
  <template data-type="loading">
    loading
  </template>
</mgt-get>
```

## <a name="properties-and-attributes"></a><span data-ttu-id="e9d7b-107">属性和属性</span><span class="sxs-lookup"><span data-stu-id="e9d7b-107">Properties and attributes</span></span>

<span data-ttu-id="e9d7b-108">您可以使用多个属性来更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-108">You can use several attributes to change the behavior of the component.</span></span> <span data-ttu-id="e9d7b-109">唯一的必需属性是`resource`。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-109">The only required attribute is `resource`.</span></span>

| <span data-ttu-id="e9d7b-110">属性</span><span class="sxs-lookup"><span data-stu-id="e9d7b-110">Attribute</span></span> | <span data-ttu-id="e9d7b-111">属性</span><span class="sxs-lookup"><span data-stu-id="e9d7b-111">Property</span></span>  | <span data-ttu-id="e9d7b-112">说明</span><span class="sxs-lookup"><span data-stu-id="e9d7b-112">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="e9d7b-113">资源</span><span class="sxs-lookup"><span data-stu-id="e9d7b-113">resource</span></span> | <span data-ttu-id="e9d7b-114">resource</span><span class="sxs-lookup"><span data-stu-id="e9d7b-114">resource</span></span> | <span data-ttu-id="e9d7b-115">要从 Microsoft Graph 中获取的资源（例如， `/me`）。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-115">The resource to get from Microsoft Graph (for example, `/me`).</span></span> |
| <span data-ttu-id="e9d7b-116">scopes</span><span class="sxs-lookup"><span data-stu-id="e9d7b-116">scopes</span></span> | <span data-ttu-id="e9d7b-117">scopes</span><span class="sxs-lookup"><span data-stu-id="e9d7b-117">scopes</span></span> | <span data-ttu-id="e9d7b-118">如果使用属性或以逗号分隔的范围（如果使用属性），则为可选的字符串数组。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-118">Optional array of strings if using the property or a comma delimited scope if using the attribute.</span></span> <span data-ttu-id="e9d7b-119">组件将使用这些作用域（使用受支持的提供程序），以确保用户已同意正确的权限。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-119">The component will use these scopes (with a supported provider) to ensure that the user has consented to the right permission.</span></span> |
| <span data-ttu-id="e9d7b-120">version</span><span class="sxs-lookup"><span data-stu-id="e9d7b-120">version</span></span> | <span data-ttu-id="e9d7b-121">version</span><span class="sxs-lookup"><span data-stu-id="e9d7b-121">version</span></span> | <span data-ttu-id="e9d7b-122">在发出 GET 请求时要使用的可选 API 版本。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-122">Optional API version to use when making the GET request.</span></span> <span data-ttu-id="e9d7b-123">默认值为 `v1.0`。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-123">Default is `v1.0`.</span></span>  |
| <span data-ttu-id="e9d7b-124">最大页数</span><span class="sxs-lookup"><span data-stu-id="e9d7b-124">max-pages</span></span> | <span data-ttu-id="e9d7b-125">maxPages</span><span class="sxs-lookup"><span data-stu-id="e9d7b-125">maxPages</span></span> | <span data-ttu-id="e9d7b-126">可选页数（针对支持分页的资源）。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-126">Optional number of pages (for resources that support paging).</span></span> <span data-ttu-id="e9d7b-127">默认值为3。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-127">Default is 3.</span></span> <span data-ttu-id="e9d7b-128">将此值设置为0将获取所有页面。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-128">Setting this value to 0 will get all pages.</span></span>  |
| <span data-ttu-id="e9d7b-129">不适用</span><span class="sxs-lookup"><span data-stu-id="e9d7b-129">N/A</span></span> | <span data-ttu-id="e9d7b-130">响应</span><span class="sxs-lookup"><span data-stu-id="e9d7b-130">response</span></span> | <span data-ttu-id="e9d7b-131">如果请求成功，则为来自 Microsoft Graph 的只读响应。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-131">Read-only response from Microsoft Graph if request was successful.</span></span>  |
| <span data-ttu-id="e9d7b-132">不适用</span><span class="sxs-lookup"><span data-stu-id="e9d7b-132">N/A</span></span> |<span data-ttu-id="e9d7b-133">error</span><span class="sxs-lookup"><span data-stu-id="e9d7b-133">error</span></span>| <span data-ttu-id="e9d7b-134">如果请求不成功，则为 Microsoft Graph 中的只读错误。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-134">Read-only error from Microsoft Graph if request was not successful.</span></span> |

## <a name="events"></a><span data-ttu-id="e9d7b-135">事件</span><span class="sxs-lookup"><span data-stu-id="e9d7b-135">Events</span></span>
| <span data-ttu-id="e9d7b-136">事件</span><span class="sxs-lookup"><span data-stu-id="e9d7b-136">Event</span></span> | <span data-ttu-id="e9d7b-137">详细信息</span><span class="sxs-lookup"><span data-stu-id="e9d7b-137">Detail</span></span> | <span data-ttu-id="e9d7b-138">说明</span><span class="sxs-lookup"><span data-stu-id="e9d7b-138">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="e9d7b-139">dataChange</span><span class="sxs-lookup"><span data-stu-id="e9d7b-139">dataChange</span></span> | <span data-ttu-id="e9d7b-140">详细信息包含`response`和`error`对象。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-140">The detail contains the `response` and `error` objects.</span></span> | <span data-ttu-id="e9d7b-141">在响应或错误发生更改时激发。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-141">Fired when the response or error change.</span></span> |

## <a name="templates"></a><span data-ttu-id="e9d7b-142">模板</span><span class="sxs-lookup"><span data-stu-id="e9d7b-142">Templates</span></span>

<span data-ttu-id="e9d7b-143">`mgt-get`组件支持几个可用于定义外观的[模板](../templates.md)。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-143">The `mgt-get` component supports several [templates](../templates.md) that you can use to define the look and feel.</span></span> <span data-ttu-id="e9d7b-144">若要指定模板，请在`<template>`组件内添加一个元素，并`data-type`将值设置为下列值之一。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-144">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="e9d7b-145">数据类型</span><span class="sxs-lookup"><span data-stu-id="e9d7b-145">Data type</span></span> | <span data-ttu-id="e9d7b-146">数据上下文</span><span class="sxs-lookup"><span data-stu-id="e9d7b-146">Data context</span></span> | <span data-ttu-id="e9d7b-147">说明</span><span class="sxs-lookup"><span data-stu-id="e9d7b-147">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="e9d7b-148">设置</span><span class="sxs-lookup"><span data-stu-id="e9d7b-148">default</span></span> | <span data-ttu-id="e9d7b-149">来自 Microsoft Graph 的响应。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-149">The response from Microsoft Graph.</span></span> | <span data-ttu-id="e9d7b-150">若要呈现来自 Microsoft Graph 的数据，则需要默认模板。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-150">The default template is required to render the data coming from Microsoft Graph.</span></span> |
| <span data-ttu-id="e9d7b-151">error</span><span class="sxs-lookup"><span data-stu-id="e9d7b-151">error</span></span> | <span data-ttu-id="e9d7b-152">Microsoft Graph 中的错误。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-152">The error from Microsoft Graph.</span></span> | <span data-ttu-id="e9d7b-153">如果发出请求时出错，将使用此模板。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-153">This template will be used if there is an error making the request.</span></span> |
| <span data-ttu-id="e9d7b-154">装载</span><span class="sxs-lookup"><span data-stu-id="e9d7b-154">loading</span></span> | <span data-ttu-id="e9d7b-155">不适用</span><span class="sxs-lookup"><span data-stu-id="e9d7b-155">N/A</span></span> | <span data-ttu-id="e9d7b-156">在发出请求时使用此模板。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-156">This template is used while the request is being made.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="e9d7b-157">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="e9d7b-157">Microsoft Graph permissions</span></span>

<span data-ttu-id="e9d7b-158">有关权限的详细信息，请参阅 Microsoft Graph[权限参考](https://docs.microsoft.com/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-158">For more information about permissions, see the Microsoft Graph [permissions reference](https://docs.microsoft.com/graph/permissions-reference).</span></span> 

## <a name="authentication"></a><span data-ttu-id="e9d7b-159">身份验证</span><span class="sxs-lookup"><span data-stu-id="e9d7b-159">Authentication</span></span>

<span data-ttu-id="e9d7b-160">该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序提取所需的数据。</span><span class="sxs-lookup"><span data-stu-id="e9d7b-160">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>
