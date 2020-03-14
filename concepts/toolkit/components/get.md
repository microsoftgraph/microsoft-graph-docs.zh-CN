---
title: 获取 Microsoft Graph 工具包中的组件
description: 通过获取组件，可以在 HTML 中直接在 Microsoft Graph 中进行任何 GET 查询。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 7c9c3fcc804dd5ba8257a1140791fa2eb60ff4ce
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639966"
---
# <a name="get-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="bdb8d-103">获取 Microsoft Graph 工具包中的组件</span><span class="sxs-lookup"><span data-stu-id="bdb8d-103">Get component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="bdb8d-104">您可以使用`mgt-get`从 Microsoft Graph 直接在 HTML 中进行任何 GET 查询。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-104">You can use `mgt-get` to make any GET query from Microsoft Graph directly in your HTML.</span></span> <span data-ttu-id="bdb8d-105">组件不提供默认 UI，需要您编写模板。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-105">The component does not provide a default UI and requires that you write a template.</span></span>

## <a name="example"></a><span data-ttu-id="bdb8d-106">示例</span><span class="sxs-lookup"><span data-stu-id="bdb8d-106">Example</span></span>

<span data-ttu-id="bdb8d-107">下面的示例演示如何使用`mgt-get`组件来显示用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-107">The following example shows the use of the `mgt-get` component to display a user's emails.</span></span> <span data-ttu-id="bdb8d-108">您可以使用代码编辑器来查看[属性和属性](#properties-and-attributes)如何更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-108">You can use the code editor to see how [properties and attributes](#properties-and-attributes) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-get--get-email&source=docs" height="500"></iframe>

[<span data-ttu-id="bdb8d-109">在 "dev" 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="bdb8d-109">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-get--get-email&source=docs)

## <a name="properties-and-attributes"></a><span data-ttu-id="bdb8d-110">属性和属性</span><span class="sxs-lookup"><span data-stu-id="bdb8d-110">Properties and attributes</span></span>

<span data-ttu-id="bdb8d-111">您可以使用多个属性来更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-111">You can use several attributes to change the behavior of the component.</span></span> <span data-ttu-id="bdb8d-112">唯一的必需属性是`resource`。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-112">The only required attribute is `resource`.</span></span>

| <span data-ttu-id="bdb8d-113">属性</span><span class="sxs-lookup"><span data-stu-id="bdb8d-113">Attribute</span></span> | <span data-ttu-id="bdb8d-114">属性</span><span class="sxs-lookup"><span data-stu-id="bdb8d-114">Property</span></span>  | <span data-ttu-id="bdb8d-115">说明</span><span class="sxs-lookup"><span data-stu-id="bdb8d-115">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="bdb8d-116">资源</span><span class="sxs-lookup"><span data-stu-id="bdb8d-116">resource</span></span> | <span data-ttu-id="bdb8d-117">resource</span><span class="sxs-lookup"><span data-stu-id="bdb8d-117">resource</span></span> | <span data-ttu-id="bdb8d-118">要从 Microsoft Graph 中获取的资源（例如， `/me`）。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-118">The resource to get from Microsoft Graph (for example, `/me`).</span></span> |
| <span data-ttu-id="bdb8d-119">scopes</span><span class="sxs-lookup"><span data-stu-id="bdb8d-119">scopes</span></span> | <span data-ttu-id="bdb8d-120">scopes</span><span class="sxs-lookup"><span data-stu-id="bdb8d-120">scopes</span></span> | <span data-ttu-id="bdb8d-121">如果使用属性或以逗号分隔的范围（如果使用属性），则为可选的字符串数组。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-121">Optional array of strings if using the property or a comma delimited scope if using the attribute.</span></span> <span data-ttu-id="bdb8d-122">组件将使用这些作用域（使用受支持的提供程序），以确保用户已同意正确的权限。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-122">The component will use these scopes (with a supported provider) to ensure that the user has consented to the right permission.</span></span> |
| <span data-ttu-id="bdb8d-123">version</span><span class="sxs-lookup"><span data-stu-id="bdb8d-123">version</span></span> | <span data-ttu-id="bdb8d-124">version</span><span class="sxs-lookup"><span data-stu-id="bdb8d-124">version</span></span> | <span data-ttu-id="bdb8d-125">在发出 GET 请求时要使用的可选 API 版本。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-125">Optional API version to use when making the GET request.</span></span> <span data-ttu-id="bdb8d-126">默认值为 `v1.0`。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-126">Default is `v1.0`.</span></span>  |
| <span data-ttu-id="bdb8d-127">最大页数</span><span class="sxs-lookup"><span data-stu-id="bdb8d-127">max-pages</span></span> | <span data-ttu-id="bdb8d-128">maxPages</span><span class="sxs-lookup"><span data-stu-id="bdb8d-128">maxPages</span></span> | <span data-ttu-id="bdb8d-129">可选页数（针对支持分页的资源）。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-129">Optional number of pages (for resources that support paging).</span></span> <span data-ttu-id="bdb8d-130">默认值为3。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-130">Default is 3.</span></span> <span data-ttu-id="bdb8d-131">将此值设置为0将获取所有页面。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-131">Setting this value to 0 will get all pages.</span></span>  |
| <span data-ttu-id="bdb8d-132">不适用</span><span class="sxs-lookup"><span data-stu-id="bdb8d-132">N/A</span></span> | <span data-ttu-id="bdb8d-133">响应</span><span class="sxs-lookup"><span data-stu-id="bdb8d-133">response</span></span> | <span data-ttu-id="bdb8d-134">如果请求成功，则为来自 Microsoft Graph 的只读响应。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-134">Read-only response from Microsoft Graph if request was successful.</span></span>  |
| <span data-ttu-id="bdb8d-135">不适用</span><span class="sxs-lookup"><span data-stu-id="bdb8d-135">N/A</span></span> |<span data-ttu-id="bdb8d-136">error</span><span class="sxs-lookup"><span data-stu-id="bdb8d-136">error</span></span>| <span data-ttu-id="bdb8d-137">如果请求不成功，则为 Microsoft Graph 中的只读错误。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-137">Read-only error from Microsoft Graph if request was not successful.</span></span> |

## <a name="events"></a><span data-ttu-id="bdb8d-138">活动</span><span class="sxs-lookup"><span data-stu-id="bdb8d-138">Events</span></span>
| <span data-ttu-id="bdb8d-139">事件</span><span class="sxs-lookup"><span data-stu-id="bdb8d-139">Event</span></span> | <span data-ttu-id="bdb8d-140">详细信息</span><span class="sxs-lookup"><span data-stu-id="bdb8d-140">Detail</span></span> | <span data-ttu-id="bdb8d-141">说明</span><span class="sxs-lookup"><span data-stu-id="bdb8d-141">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="bdb8d-142">dataChange</span><span class="sxs-lookup"><span data-stu-id="bdb8d-142">dataChange</span></span> | <span data-ttu-id="bdb8d-143">详细信息包含`response`和`error`对象。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-143">The detail contains the `response` and `error` objects.</span></span> | <span data-ttu-id="bdb8d-144">在响应或错误发生更改时激发。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-144">Fired when the response or error change.</span></span> |

## <a name="templates"></a><span data-ttu-id="bdb8d-145">模板</span><span class="sxs-lookup"><span data-stu-id="bdb8d-145">Templates</span></span>

<span data-ttu-id="bdb8d-146">`mgt-get`组件支持几个可用于定义外观的[模板](../templates.md)。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-146">The `mgt-get` component supports several [templates](../templates.md) that you can use to define the look and feel.</span></span> <span data-ttu-id="bdb8d-147">若要指定模板，请在`<template>`组件内添加一个元素，并`data-type`将值设置为下列值之一。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-147">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="bdb8d-148">数据类型</span><span class="sxs-lookup"><span data-stu-id="bdb8d-148">Data type</span></span> | <span data-ttu-id="bdb8d-149">数据上下文</span><span class="sxs-lookup"><span data-stu-id="bdb8d-149">Data context</span></span> | <span data-ttu-id="bdb8d-150">说明</span><span class="sxs-lookup"><span data-stu-id="bdb8d-150">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="bdb8d-151">设置</span><span class="sxs-lookup"><span data-stu-id="bdb8d-151">default</span></span> | <span data-ttu-id="bdb8d-152">来自 Microsoft Graph 的响应。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-152">The response from Microsoft Graph.</span></span> | <span data-ttu-id="bdb8d-153">若要呈现来自 Microsoft Graph 的数据，则需要默认模板。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-153">The default template is required to render the data coming from Microsoft Graph.</span></span> |
| <span data-ttu-id="bdb8d-154">error</span><span class="sxs-lookup"><span data-stu-id="bdb8d-154">error</span></span> | <span data-ttu-id="bdb8d-155">Microsoft Graph 中的错误。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-155">The error from Microsoft Graph.</span></span> | <span data-ttu-id="bdb8d-156">如果发出请求时出错，将使用此模板。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-156">This template will be used if there is an error making the request.</span></span> |
| <span data-ttu-id="bdb8d-157">装载</span><span class="sxs-lookup"><span data-stu-id="bdb8d-157">loading</span></span> | <span data-ttu-id="bdb8d-158">不适用</span><span class="sxs-lookup"><span data-stu-id="bdb8d-158">N/A</span></span> | <span data-ttu-id="bdb8d-159">在发出请求时使用此模板。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-159">This template is used while the request is being made.</span></span> |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="bdb8d-160">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="bdb8d-160">Microsoft Graph permissions</span></span>

<span data-ttu-id="bdb8d-161">有关权限的详细信息，请参阅 Microsoft Graph[权限参考](https://docs.microsoft.com/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-161">For more information about permissions, see the Microsoft Graph [permissions reference](https://docs.microsoft.com/graph/permissions-reference).</span></span> 

## <a name="authentication"></a><span data-ttu-id="bdb8d-162">身份验证</span><span class="sxs-lookup"><span data-stu-id="bdb8d-162">Authentication</span></span>

<span data-ttu-id="bdb8d-163">该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序提取所需的数据。</span><span class="sxs-lookup"><span data-stu-id="bdb8d-163">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>
