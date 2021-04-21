---
title: 在 OneNote 页中使用笔记标记
description: " Microsoft 365 中的企业笔记本"
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 6fe0d1603e2cd5b94e753b4e8d6b1a7e47b5aacf
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921915"
---
# <a name="use-note-tags-in-onenote-pages"></a><span data-ttu-id="033bc-103">在 OneNote 页中使用笔记标记</span><span class="sxs-lookup"><span data-stu-id="033bc-103">Use note tags in OneNote pages</span></span>

<span data-ttu-id="033bc-104">**适用于** OneDrive 上的消费者笔记本 | Microsoft 365 上的企业级笔记本</span><span class="sxs-lookup"><span data-stu-id="033bc-104">**Applies to** Consumer notebooks on OneDrive | Enterprise notebooks on Microsoft 365</span></span>

<span data-ttu-id="033bc-105">使用 `data-tag` 属性在 OneNote 页面上添加并更新复选框、星标及其他内置笔记标记，如下图所示。</span><span class="sxs-lookup"><span data-stu-id="033bc-105">Use the `data-tag` attribute to add and update check boxes, stars, and other built-in note tags on a OneNote page, as shown in the following image.</span></span>

![显示在 OneNote 页面上的三个笔记标记。](images/note-tags-example.png)


<a name="attributes"></a>

## <a name="note-tag-attributes"></a><span data-ttu-id="033bc-107">笔记标记属性</span><span class="sxs-lookup"><span data-stu-id="033bc-107">Note tag attributes</span></span>

<span data-ttu-id="033bc-108">在 OneNote 页面的 HTML 中，笔记标记由 `data-tag` 属性来表示。</span><span class="sxs-lookup"><span data-stu-id="033bc-108">In the HTML of a OneNote page, a note tag is represented by the `data-tag` attribute.</span></span> <span data-ttu-id="033bc-109">例如：</span><span class="sxs-lookup"><span data-stu-id="033bc-109">For example:</span></span>

- <span data-ttu-id="033bc-110">未选中待办事项框：`<p data-tag="to-do">`</span><span class="sxs-lookup"><span data-stu-id="033bc-110">An unchecked to-do box:  `<p data-tag="to-do">`</span></span>

- <span data-ttu-id="033bc-111">已选中的待办事项框：`<p data-tag="to-do:completed">`</span><span class="sxs-lookup"><span data-stu-id="033bc-111">A checked to-do box:  `<p data-tag="to-do:completed">`</span></span>

- <span data-ttu-id="033bc-112">星标：`<h2 data-tag="important">`</span><span class="sxs-lookup"><span data-stu-id="033bc-112">A star:  `<h2 data-tag="important">`</span></span>

<span data-ttu-id="033bc-113">`data-tag` 值由形状组成，有时由状态组成（查看所有[支持的值](#built-in-note-tags-for-onenote)）。</span><span class="sxs-lookup"><span data-stu-id="033bc-113">A `data-tag` value is composed of a shape, and sometimes a status (see all [supported values](#built-in-note-tags-for-onenote)).</span></span>

| <span data-ttu-id="033bc-114">属性</span><span class="sxs-lookup"><span data-stu-id="033bc-114">Property</span></span> | <span data-ttu-id="033bc-115">说明</span><span class="sxs-lookup"><span data-stu-id="033bc-115">Description</span></span> |
|:------|:------|
| <span data-ttu-id="033bc-116">shape</span><span class="sxs-lookup"><span data-stu-id="033bc-116">shape</span></span> | <span data-ttu-id="033bc-117">笔记标记的标识符（示例：`to-do` 或 `important`）。</span><span class="sxs-lookup"><span data-stu-id="033bc-117">The identifier of the note tag (example: `to-do` or `important`).</span></span> |
| <span data-ttu-id="033bc-118">status</span><span class="sxs-lookup"><span data-stu-id="033bc-118">status</span></span> | <span data-ttu-id="033bc-119">复选框笔记标记的状态。</span><span class="sxs-lookup"><span data-stu-id="033bc-119">The status of check box note tags.</span></span> <span data-ttu-id="033bc-120">这仅用于将复选框设置为“已完成”。</span><span class="sxs-lookup"><span data-stu-id="033bc-120">This is used only to set check boxes as completed.</span></span> |


<a name="note-tags"></a>

## <a name="add-or-update-note-tags"></a><span data-ttu-id="033bc-121">添加或更新笔记标记</span><span class="sxs-lookup"><span data-stu-id="033bc-121">Add or update note tags</span></span>

<span data-ttu-id="033bc-122">要添加或更新内置笔记标记，只需使用受支持元素上的 `data-tag` 属性。</span><span class="sxs-lookup"><span data-stu-id="033bc-122">To add or update a built-in note tag, just use the `data-tag` attribute on a supported element.</span></span> <span data-ttu-id="033bc-123">例如，下面是标记为“重要”的段落：</span><span class="sxs-lookup"><span data-stu-id="033bc-123">For example, here's a paragraph marked as important:</span></span>

```html
<p data-tag="important">...</p>
```

<span data-ttu-id="033bc-124">使用逗号分隔多个笔记标记：</span><span class="sxs-lookup"><span data-stu-id="033bc-124">Separate multiple note tags with commas:</span></span>

```html
<p data-tag="important, critical">...</p>
```

<span data-ttu-id="033bc-125">可以在以下元素上定义 `data-tag`：</span><span class="sxs-lookup"><span data-stu-id="033bc-125">You can define a `data-tag` on the following elements:</span></span>

- <span data-ttu-id="033bc-126">p</span><span class="sxs-lookup"><span data-stu-id="033bc-126">p</span></span>
- <span data-ttu-id="033bc-127">ul、ol、li（查看有关[列表上的笔记标记](#note-tags-on-lists)的详细信息）</span><span class="sxs-lookup"><span data-stu-id="033bc-127">ul, ol, li (see more about [note tags on lists](#note-tags-on-lists))</span></span>
- <span data-ttu-id="033bc-128">img</span><span class="sxs-lookup"><span data-stu-id="033bc-128">img</span></span>
- <span data-ttu-id="033bc-129">h1 - h6</span><span class="sxs-lookup"><span data-stu-id="033bc-129">h1 - h6</span></span>
- <span data-ttu-id="033bc-130">title</span><span class="sxs-lookup"><span data-stu-id="033bc-130">title</span></span>

<span data-ttu-id="033bc-131">请参阅[内置的笔记标记](#built-in-note-tags-for-onenote)，了解可与 Microsoft Graph 一起使用的笔记标记列表。</span><span class="sxs-lookup"><span data-stu-id="033bc-131">See [Built-in note tags](#built-in-note-tags-for-onenote) for a list of note tags that you can use with Microsoft Graph.</span></span> <span data-ttu-id="033bc-132">不支持使用 Microsoft Graph 添加或更新自定义标记。</span><span class="sxs-lookup"><span data-stu-id="033bc-132">Adding or updating custom tags using Microsoft Graph is not supported.</span></span>

### <a name="examples"></a><span data-ttu-id="033bc-133">示例</span><span class="sxs-lookup"><span data-stu-id="033bc-133">Examples</span></span>

<span data-ttu-id="033bc-134">下面是一个简单的待办事项列表，其第一项已完成。</span><span class="sxs-lookup"><span data-stu-id="033bc-134">Here's a simple to-do list with the first item completed.</span></span>

```html
<p data-tag="to-do:completed" data-id="prep">Till garden bed</p>
<p data-tag="to-do" data-id="spring">Plant peas and spinach</p>
<p data-tag="to-do" data-id="summer">Plant tomatoes and peppers</p>
```

<span data-ttu-id="033bc-135">请注意，上述 `<p>` 标签各包含一个 `data-id` 属性。</span><span class="sxs-lookup"><span data-stu-id="033bc-135">Note that the `<p>` tags above each include a `data-id` attribute.</span></span> <span data-ttu-id="033bc-136">这样，可以更容易地更新复选框笔记标记。</span><span class="sxs-lookup"><span data-stu-id="033bc-136">This makes it easier to update the check box note tags.</span></span> <span data-ttu-id="033bc-137">例如，以下请求将春耕待办事项标记为“已完成”。</span><span class="sxs-lookup"><span data-stu-id="033bc-137">For example, the following request marks the spring planting to-do item as completed.</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: application/json
Authorization: Bearer {token}

[
   {
    'target':'#spring',
    'action':'replace',
    'content':'<p data-tag="to-do:completed"  data-id="spring">Plant peas and spinach</p>'
  }
]
```

<span data-ttu-id="033bc-138">以下请求将创建包含所有[内置笔记标记](#built-in-note-tags-for-onenote)的页面。</span><span class="sxs-lookup"><span data-stu-id="033bc-138">The following request creates a page that contains all [built-in note tags](#built-in-note-tags-for-onenote).</span></span>

```html
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages

Content-Type: text/html
Authorization: Bearer {token}


<!DOCTYPE html>
<html>
  <head>
    <title data-tag="to-do:completed">All built-in note tags</title>
  </head>
  <body>
    <h1 data-tag="important">Paragraphs with built-in note tags</h1>
    <p data-tag="to-do">to-do</p>
    <p data-tag="important">important</p>
    <p data-tag="question">question</p>
    <p data-tag="definition">definition</p>
    <p data-tag="highlight">highlight</p>
    <p data-tag="contact">contact</p>
    <p data-tag="address">address</p>
    <p data-tag="phone-number">phone-number</p>
    <p data-tag="web-site-to-visit">web-site-to-visit</p>
    <p data-tag="idea">idea</p>
    <p data-tag="password">password</p>
    <p data-tag="critical">critical</p>
    <p data-tag="project-a">project-a</p>
    <p data-tag="project-b">project-b</p>
    <p data-tag="remember-for-later">remember-for-later</p>
    <p data-tag="movie-to-see">movie-to-see</p>
    <p data-tag="book-to-read">book-to-read</p>
    <p data-tag="music-to-listen-to">music-to-listen-to</p>
    <p data-tag="source-for-article">source-for-article</p>
    <p data-tag="remember-for-blog">remember-for-blog</p>
    <p data-tag="discuss-with-person-a">discuss-with-person-a</p>
    <p data-tag="discuss-with-person-b">discuss-with-person-b</p>
    <p data-tag="discuss-with-manager">discuss-with-manager</p>
    <p data-tag="send-in-email">send-in-email</p>
    <p data-tag="schedule-meeting">schedule-meeting</p>
    <p data-tag="call-back">call-back</p>
    <p data-tag="to-do-priority-1">to-do-priority-1</p>
    <p data-tag="to-do-priority-2">to-do-priority-2</p>
    <p data-tag="client-request">client-request</p>
    <h1 data-tag="important">Paragraphs with check boxes marked with "completed" status</h1>
    <p data-tag="to-do:completed">to-do:completed</p>
    <p data-tag="discuss-with-person-a:completed">discuss-with-person-a:completed</p>
    <p data-tag="discuss-with-person-b:completed">discuss-with-person-b:completed</p>
    <p data-tag="discuss-with-manager:completed">discuss-with-manager:completed</p>
    <p data-tag="schedule-meeting:completed">schedule-meeting:completed</p>
    <p data-tag="call-back:completed">call-back:completed</p>
    <p data-tag="to-do-priority-1:completed">to-do-priority-1:completed</p>
    <p data-tag="to-do-priority-2:completed">to-do-priority-2:completed</p>
    <p data-tag="client-request:completed">client-request:completed</p>
    <h1 data-tag="important">Multiple note tags</h1>
    <p data-tag="project-a,  client-request:completed">Two note tags:  project-a, client-request:completed</p>
    <p data-tag="idea, send-in-email, question">Three note tags:  idea, send-in-email, question</p>
    <h1 data-tag="important">Using note tags with other elements</h1>
    <p><b>Note tag on a list item:</b></p>
    <ul>
      <li data-tag="to-do-priority-1:completed">Make a to-do list</li>
    </ul>
    <p><b>Note tag on an image:</b></p>
    <img data-tag="source-for-article" src="https://placecorgi.com/200" />
    <p><b>Note tag with embedded style:</b></p>
    <p data-tag="important">Next time, <b>don't</b> forget to invite <span style="background-color:yellow">Dan</span>.</p>
  </body>
</html>
```

<span data-ttu-id="033bc-139">有关创建页面的详细信息，请参阅[创建 OneNote 页面](onenote-create-page.md)。</span><span class="sxs-lookup"><span data-stu-id="033bc-139">For more information about creating pages, see [Create OneNote pages](onenote-create-page.md).</span></span> <span data-ttu-id="033bc-140">有关更新页面的详细信息，请参阅[更新 OneNote 页面](onenote-update-page.md)。</span><span class="sxs-lookup"><span data-stu-id="033bc-140">For more about updating pages, see [Update OneNote pages](onenote-update-page.md).</span></span>


<a name="note-tags-lists"></a>

## <a name="note-tags-on-lists"></a><span data-ttu-id="033bc-141">列表上的笔记标记</span><span class="sxs-lookup"><span data-stu-id="033bc-141">Note tags on lists</span></span>

<span data-ttu-id="033bc-142">下面是一些使用列表中笔记标记的相关指南：</span><span class="sxs-lookup"><span data-stu-id="033bc-142">Here are some guidelines for working with note tags on lists:</span></span>

- <span data-ttu-id="033bc-143">使用待办事项列表的 `p` 元素。</span><span class="sxs-lookup"><span data-stu-id="033bc-143">Use `p` elements for to-do lists.</span></span> <span data-ttu-id="033bc-144">这些元素不会显示项目符号或编号，更加易于更新。</span><span class="sxs-lookup"><span data-stu-id="033bc-144">They don't display a bullet or number, and they're easier to update.</span></span>

- <span data-ttu-id="033bc-145">若要创建或更新为所有列表项显示 **相同** 笔记标记的列表，请在 `ul` 或 `ol` 上定义 `data-tag`。</span><span class="sxs-lookup"><span data-stu-id="033bc-145">To create or update lists that display the **same** note tag for all list items, define `data-tag` on the `ul` or `ol`.</span></span> <span data-ttu-id="033bc-146">若要更新完整列表，需要对 `ul` 或 `ol` 重新定义 `data-tag`。</span><span class="sxs-lookup"><span data-stu-id="033bc-146">To update the entire list, you'll need to redefine `data-tag` on the `ul` or `ol`.</span></span>

- <span data-ttu-id="033bc-147">若要创建或更新为某些或全部列表项显示 **唯一** 笔记标记的列表，请在 `li` 元素上定义 `data-tag`，并且不要在 `ul` 或 `ol` 中嵌套 `li` 元素。</span><span class="sxs-lookup"><span data-stu-id="033bc-147">To create or update lists that display a **unique** note tag for some or all list items, define `data-tag` on `li` elements, and don't nest the `li` elements in a `ul` or `ol`.</span></span> <span data-ttu-id="033bc-148">若要更新整个列表，将需要删除在输出 HTML 中返回的 `ul`，并仅提供非嵌套的 `li` 元素。</span><span class="sxs-lookup"><span data-stu-id="033bc-148">To update the entire list, you'll need to remove the `ul` that's returned in the output HTML and provide only the unnested `li` elements.</span></span>

- <span data-ttu-id="033bc-149">要更新特定的 `li` 元素，单独定位 `li` 元素并对 `li` 元素定义 `data-tag`。</span><span class="sxs-lookup"><span data-stu-id="033bc-149">To update specific `li` elements, target the `li` elements individually and define the `data-tag` on the `li` element.</span></span> <span data-ttu-id="033bc-150">任何单独处理的 `li` 元素都可以进行更新，以显示唯一笔记标记，而不考虑列表的最初定义方式。</span><span class="sxs-lookup"><span data-stu-id="033bc-150">Any individually addressed `li` element can be updated to display a unique note tag, no matter how the list was originally defined.</span></span>

  <span data-ttu-id="033bc-151">准则基于 Microsoft Graph 所应用的以下规则：</span><span class="sxs-lookup"><span data-stu-id="033bc-151">The guidelines are based on the following rules that are applied by Microsoft Graph:</span></span>

  - <span data-ttu-id="033bc-152">`ul` 或 `ol` 的 `data-tag` 设置会覆盖子 `li` 元素上的所有设置。</span><span class="sxs-lookup"><span data-stu-id="033bc-152">The `data-tag` setting for a `ul` or `ol` overrides all settings on child `li` elements.</span></span> <span data-ttu-id="033bc-153">这同样适用于 `ul` 或 `ol` 未指定 `data-tag` 但其子 `li` 元素执行了该操作的情况。</span><span class="sxs-lookup"><span data-stu-id="033bc-153">This applies even when the `ul` or `ol` doesn't specify a `data-tag` but its child `li` elements do.</span></span>

    <span data-ttu-id="033bc-154">例如，如果创建定义 `data-tag="project-a"` 的 `ul` 或 `ol`，其所有列表项将都显示 *项目 A* 笔记标记。</span><span class="sxs-lookup"><span data-stu-id="033bc-154">For example, if you create a `ul` or `ol` that defines `data-tag="project-a"`, all its list items will display the *Project A* note tag.</span></span> <span data-ttu-id="033bc-155">或者，如果 `ul` 或 `ol` 未定义 `data-tag`，则没有任何项会显示笔记标记。</span><span class="sxs-lookup"><span data-stu-id="033bc-155">Or if the `ul` or `ol` doesn't define a `data-tag`, none of its items will display a note tag.</span></span> <span data-ttu-id="033bc-156">无论子 `li` 元素有什么显式设置，都会发生这种覆盖。</span><span class="sxs-lookup"><span data-stu-id="033bc-156">This override happens regardless of any explicit settings on child `li` elements.</span></span>

- <span data-ttu-id="033bc-157">在下列情况下，唯一的 `data-tag` 设置被视为列表项：</span><span class="sxs-lookup"><span data-stu-id="033bc-157">Unique `data-tag` settings are honored for list items under the following conditions:</span></span>

  - <span data-ttu-id="033bc-158">在创建或更新请求中，`li` 元素不嵌套在 `ul` 或 `ol` 中。</span><span class="sxs-lookup"><span data-stu-id="033bc-158">The `li` elements are not nested in a `ul` or `ol` in a create or update request.</span></span>

  - <span data-ttu-id="033bc-159">对 `li` 元素在更新请求中单独处理。</span><span class="sxs-lookup"><span data-stu-id="033bc-159">An `li` element is individually addressed in an update request.</span></span>

- <span data-ttu-id="033bc-160">在输入 HTML 中发送的未嵌套 `li` 元素将在输出 HTML 的 `ul` 中返回。</span><span class="sxs-lookup"><span data-stu-id="033bc-160">Unnested `li` elements sent in input HTML are returned in a `ul` in the output HTML.</span></span>

- <span data-ttu-id="033bc-161">在输出 HTML 中，所有 `data-tag` 列表设置都在列表项的 `span` 元素上定义。</span><span class="sxs-lookup"><span data-stu-id="033bc-161">In output HTML, all `data-tag` list settings are defined on `span` elements on the list items.</span></span>


<span data-ttu-id="033bc-162">以下代码显示如何应用其中的某些规则。</span><span class="sxs-lookup"><span data-stu-id="033bc-162">The following code shows how some of these rules are applied.</span></span> <span data-ttu-id="033bc-163">输入 HTML 将使用笔记标记创建两个列表。</span><span class="sxs-lookup"><span data-stu-id="033bc-163">The input HTML creates two lists with note tags.</span></span> <span data-ttu-id="033bc-164">输出 HTML 是检索页面内容时针对列表所返回的内容。</span><span class="sxs-lookup"><span data-stu-id="033bc-164">The output HTML is what's returned for the lists when you retrieve page content.</span></span>

#### <a name="input-html"></a><span data-ttu-id="033bc-165">输入 HTML</span><span class="sxs-lookup"><span data-stu-id="033bc-165">Input HTML</span></span>

```html
<!--To display the same note tag on all list items, define note tags on the ul or ol.-->
<ul data-tag="project-a" data-id="agenda">
  <li>An item with a Project A note tag</li>
  <li>An item with a Project A note tag</li>
</ul>

<!--To display unique note tags on list items, don't nest li elements in a ul or ol.-->
<li data-tag="idea" data-id="my-idea">An item with an Idea note tag</li>
<li data-tag="question" data-id="my-question">An item with a Question note tag</li>
```

#### <a name="output-html"></a><span data-ttu-id="033bc-166">输出 HTML</span><span class="sxs-lookup"><span data-stu-id="033bc-166">Output HTML</span></span>

```html
<ul>
  <li><span data-tag="project-a">An item with a Project A note tag</span></li>
  <li><span data-tag="project-a">An item with a Project A note tag</span></li>
</ul>
<br />
<ul>
  <li style="..."><span data-tag="idea">An item with an Idea note tag</span></li>
  <li style="..."><span data-tag="question">An item with a Question note tag</span></li>
</ul>
```

<a name="output-html"></a>

## <a name="retrieve-note-tags"></a><span data-ttu-id="033bc-167">检索笔记标记</span><span class="sxs-lookup"><span data-stu-id="033bc-167">Retrieve note tags</span></span>

<span data-ttu-id="033bc-168">当访问页面内容时，内置笔记标记将包含在输出 HTML 中：</span><span class="sxs-lookup"><span data-stu-id="033bc-168">Built-in note tags are included in the output HTML when you get page content:</span></span>

`GET ../api/v1.0/pages/{page-id}/content`

<span data-ttu-id="033bc-169">输出 HTML 中的 `data-tag` 属性始终包含形状值，并且仅在它表示设置为“已完成”的复选框笔记标记时才包含状态。</span><span class="sxs-lookup"><span data-stu-id="033bc-169">A `data-tag` attribute in the output HTML always includes a shape value, and it only includes a status if it represents a check box note tag that's set to completed.</span></span> <span data-ttu-id="033bc-170">以下示例显示用于创建一些笔记标记的输入 HTML 和返回的输出 HTML。</span><span class="sxs-lookup"><span data-stu-id="033bc-170">The following examples show the input HTML used to create some note tags and the output HTML that's returned.</span></span>

#### <a name="input-html"></a><span data-ttu-id="033bc-171">输入 HTML</span><span class="sxs-lookup"><span data-stu-id="033bc-171">Input HTML</span></span>

```html
<h1>Status meeting</h1>
<p data-tag="important">Next week's meeting has been moved to <b>Wednesday</b>.</p>
<p data-tag="question">What are the exact dates for the conference?</p>
<p>Upcoming training opportunities. See Katie for more info.</p>
<p data-tag="project-a">Around the room updates.</p>
<ul data-tag="critical">
  <li>Design handouts</li>
  <li>Plan keynote</li>
</ul>
```

#### <a name="output-html"></a><span data-ttu-id="033bc-172">输出 HTML</span><span class="sxs-lookup"><span data-stu-id="033bc-172">Output HTML</span></span>

```html
<h1 style="...">Status meeting</h1>
<p data-tag="important">Next week's meeting has been moved to <span style="font-weight:bold">Wednesday</span>.</p>
<p data-tag="question">What are the exact dates for the conference?</p>
<p>Upcoming training opportunities. See Katie for more info.</p>
<p data-tag="project-a">Around the room updates.</p>
<ul>
  <li><span data-tag="critical">Design handouts</span></li>
  <li><span data-tag="critical">Plan keynote</span></li>
</ul>
```

<span data-ttu-id="033bc-173">请注意，在列表级别上定义的 `data-tag` 属性会被推送到它的列表项。</span><span class="sxs-lookup"><span data-stu-id="033bc-173">Note that the `data-tag` attribute defined at the list level is pushed to its list items.</span></span> <span data-ttu-id="033bc-174">有关将笔记标记与列表结合使用的详细信息，请参阅[列表上的笔记标记](#note-tags-on-lists)。</span><span class="sxs-lookup"><span data-stu-id="033bc-174">For more information about using note tags with lists, see [Note tags on lists](#note-tags-on-lists).</span></span>

> <span data-ttu-id="033bc-175">**注意：** 在输出 HTML 中，定义和后续工作笔记标记均作为 `data-tag="remember-for-later"` 返回。</span><span class="sxs-lookup"><span data-stu-id="033bc-175">**Note:** In the output HTML, the definition and remember-for-later note tags are both returned as `data-tag="remember-for-later"`.</span></span> <span data-ttu-id="033bc-176">`title` 元素不返回任何笔记标记信息。</span><span class="sxs-lookup"><span data-stu-id="033bc-176">The `title` element doesn't return any note tag information.</span></span>




<a name="built-in-tags"></a>

## <a name="built-in-note-tags-for-onenote"></a><span data-ttu-id="033bc-177">OneNote 的内置笔记标记</span><span class="sxs-lookup"><span data-stu-id="033bc-177">Built-in note tags for OneNote</span></span>

<span data-ttu-id="033bc-178">OneNote 包括以下内置笔记标记：</span><span class="sxs-lookup"><span data-stu-id="033bc-178">OneNote includes the following built-in note tags:</span></span>

![所有内置笔记标记。](images/note-tags-all.png)

<span data-ttu-id="033bc-180">可以为 `data-tag` 属性分配下列清单中显示的值。</span><span class="sxs-lookup"><span data-stu-id="033bc-180">The values you can assign to the `data-tag` attribute are shown in the following list.</span></span> <span data-ttu-id="033bc-181">不支持自定义标记。</span><span class="sxs-lookup"><span data-stu-id="033bc-181">Custom tags are not supported.</span></span>

- `shape[:status]`
- `to-do`
- `to-do:completed`
- `important`
- `question`
- `definition`
- `highlight`
- `contact`
- `address`
- `phone-number`
- `web-site-to-visit`
- `idea`
- `password`
- `critical`
- `project-a`
- `project-b`
- `remember-for-later`
- `movie-to-see`
- `book-to-read`
- `music-to-listen-to`
- `source-for-article`
- `remember-for-blog`
- `discuss-with-person-a`
- `discuss-with-person-a:completed`
- `discuss-with-person-b`
- `discuss-with-person-b:completed`
- `discuss-with-manager`
- `discuss-with-manager:completed`
- `send-in-email`
- `schedule-meeting`
- `schedule-meeting:completed`
- `call-back`
- `call-back:completed`
- `to-do-priority-1`
- `to-do-priority-1:completed`
- `to-do-priority-2`
- `to-do-priority-2:completed`
- `client-request`
- `client-request:completed`


<a name="request-response-info"></a>

## <a name="response-information"></a><span data-ttu-id="033bc-182">响应信息</span><span class="sxs-lookup"><span data-stu-id="033bc-182">Response information</span></span>

<span data-ttu-id="033bc-183">Microsoft Graph 在响应中返回以下信息。</span><span class="sxs-lookup"><span data-stu-id="033bc-183">Microsoft Graph returns the following information in the response.</span></span>

| <span data-ttu-id="033bc-184">响应数据</span><span class="sxs-lookup"><span data-stu-id="033bc-184">Response data</span></span> | <span data-ttu-id="033bc-185">说明</span><span class="sxs-lookup"><span data-stu-id="033bc-185">Description</span></span> |
|------|------|
| <span data-ttu-id="033bc-186">成功代码</span><span class="sxs-lookup"><span data-stu-id="033bc-186">Success code</span></span> | <span data-ttu-id="033bc-187">成功的 POST 请求的 HTTP 状态代码为 201，成功的 PATCH 请求的 HTTP 状态代码为 204。</span><span class="sxs-lookup"><span data-stu-id="033bc-187">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |
| <span data-ttu-id="033bc-188">错误</span><span class="sxs-lookup"><span data-stu-id="033bc-188">Errors</span></span> | <span data-ttu-id="033bc-189">请阅读 [Microsoft Graph 中 OneNote API 的错误代码](onenote-error-codes.md)，以了解 Microsoft Graph 可以返回的 OneNote 错误。</span><span class="sxs-lookup"><span data-stu-id="033bc-189">Read [Error codes for OneNote APIs in Microsoft Graph](onenote-error-codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="033bc-190">权限</span><span class="sxs-lookup"><span data-stu-id="033bc-190">Permissions</span></span>

<span data-ttu-id="033bc-191">若要创建或更新 OneNote 页面，需要请求相应的权限。</span><span class="sxs-lookup"><span data-stu-id="033bc-191">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="033bc-192">选择应用运行所需的最低级别的权限。</span><span class="sxs-lookup"><span data-stu-id="033bc-192">Choose the lowest level of permissions that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="033bc-193">POST 页面的权限</span><span class="sxs-lookup"><span data-stu-id="033bc-193">Permissions for POST pages</span></span>

- <span data-ttu-id="033bc-194">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="033bc-194">Notes.Create</span></span>
- <span data-ttu-id="033bc-195">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="033bc-195">Notes.ReadWrite</span></span>
- <span data-ttu-id="033bc-196">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="033bc-196">Notes.ReadWrite.All</span></span>

#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="033bc-197">PATCH 页面的权限</span><span class="sxs-lookup"><span data-stu-id="033bc-197">Permissions for PATCH pages</span></span>

- <span data-ttu-id="033bc-198">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="033bc-198">Notes.ReadWrite</span></span>
- <span data-ttu-id="033bc-199">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="033bc-199">Notes.ReadWrite.All</span></span>

<span data-ttu-id="033bc-200">有关权限范围及其工作方式的详细信息，请参阅 [OneNote 权限范围](permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="033bc-200">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions-reference.md).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="033bc-201">另请参阅</span><span class="sxs-lookup"><span data-stu-id="033bc-201">See also</span></span>

- [<span data-ttu-id="033bc-202">创建 OneNote 页</span><span class="sxs-lookup"><span data-stu-id="033bc-202">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="033bc-203">更新 OneNote 页内容</span><span class="sxs-lookup"><span data-stu-id="033bc-203">Update OneNote page content</span></span>](onenote-update-page.md)
- [<span data-ttu-id="033bc-204">与 OneNote 集成</span><span class="sxs-lookup"><span data-stu-id="033bc-204">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="033bc-205">OneNote 开发者博客</span><span class="sxs-lookup"><span data-stu-id="033bc-205">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="033bc-206">Microsoft Q&A 上的 OneNote 开发问题</span><span class="sxs-lookup"><span data-stu-id="033bc-206">OneNote development questions on Microsoft Q&A</span></span>](/answers/topics/microsoft-graph-notes.html)
- [<span data-ttu-id="033bc-207">OneNote GitHub 存储库</span><span class="sxs-lookup"><span data-stu-id="033bc-207">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)