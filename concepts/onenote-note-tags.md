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
# <a name="use-note-tags-in-onenote-pages"></a>在 OneNote 页中使用笔记标记

**适用于** OneDrive 上的消费者笔记本 | Microsoft 365 上的企业级笔记本

使用 `data-tag` 属性在 OneNote 页面上添加并更新复选框、星标及其他内置笔记标记，如下图所示。

![显示在 OneNote 页面上的三个笔记标记。](images/note-tags-example.png)


<a name="attributes"></a>

## <a name="note-tag-attributes"></a>笔记标记属性

在 OneNote 页面的 HTML 中，笔记标记由 `data-tag` 属性来表示。 例如：

- 未选中待办事项框：`<p data-tag="to-do">`

- 已选中的待办事项框：`<p data-tag="to-do:completed">`

- 星标：`<h2 data-tag="important">`

`data-tag` 值由形状组成，有时由状态组成（查看所有[支持的值](#built-in-note-tags-for-onenote)）。

| 属性 | 说明 |
|:------|:------|
| shape | 笔记标记的标识符（示例：`to-do` 或 `important`）。 |
| status | 复选框笔记标记的状态。 这仅用于将复选框设置为“已完成”。 |


<a name="note-tags"></a>

## <a name="add-or-update-note-tags"></a>添加或更新笔记标记

要添加或更新内置笔记标记，只需使用受支持元素上的 `data-tag` 属性。 例如，下面是标记为“重要”的段落：

```html
<p data-tag="important">...</p>
```

使用逗号分隔多个笔记标记：

```html
<p data-tag="important, critical">...</p>
```

可以在以下元素上定义 `data-tag`：

- p
- ul、ol、li（查看有关[列表上的笔记标记](#note-tags-on-lists)的详细信息）
- img
- h1 - h6
- title

请参阅[内置的笔记标记](#built-in-note-tags-for-onenote)，了解可与 Microsoft Graph 一起使用的笔记标记列表。 不支持使用 Microsoft Graph 添加或更新自定义标记。

### <a name="examples"></a>示例

下面是一个简单的待办事项列表，其第一项已完成。

```html
<p data-tag="to-do:completed" data-id="prep">Till garden bed</p>
<p data-tag="to-do" data-id="spring">Plant peas and spinach</p>
<p data-tag="to-do" data-id="summer">Plant tomatoes and peppers</p>
```

请注意，上述 `<p>` 标签各包含一个 `data-id` 属性。 这样，可以更容易地更新复选框笔记标记。 例如，以下请求将春耕待办事项标记为“已完成”。

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

以下请求将创建包含所有[内置笔记标记](#built-in-note-tags-for-onenote)的页面。

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

有关创建页面的详细信息，请参阅[创建 OneNote 页面](onenote-create-page.md)。 有关更新页面的详细信息，请参阅[更新 OneNote 页面](onenote-update-page.md)。


<a name="note-tags-lists"></a>

## <a name="note-tags-on-lists"></a>列表上的笔记标记

下面是一些使用列表中笔记标记的相关指南：

- 使用待办事项列表的 `p` 元素。 这些元素不会显示项目符号或编号，更加易于更新。

- 若要创建或更新为所有列表项显示 **相同** 笔记标记的列表，请在 `ul` 或 `ol` 上定义 `data-tag`。 若要更新完整列表，需要对 `ul` 或 `ol` 重新定义 `data-tag`。

- 若要创建或更新为某些或全部列表项显示 **唯一** 笔记标记的列表，请在 `li` 元素上定义 `data-tag`，并且不要在 `ul` 或 `ol` 中嵌套 `li` 元素。 若要更新整个列表，将需要删除在输出 HTML 中返回的 `ul`，并仅提供非嵌套的 `li` 元素。

- 要更新特定的 `li` 元素，单独定位 `li` 元素并对 `li` 元素定义 `data-tag`。 任何单独处理的 `li` 元素都可以进行更新，以显示唯一笔记标记，而不考虑列表的最初定义方式。

  准则基于 Microsoft Graph 所应用的以下规则：

  - `ul` 或 `ol` 的 `data-tag` 设置会覆盖子 `li` 元素上的所有设置。 这同样适用于 `ul` 或 `ol` 未指定 `data-tag` 但其子 `li` 元素执行了该操作的情况。

    例如，如果创建定义 `data-tag="project-a"` 的 `ul` 或 `ol`，其所有列表项将都显示 *项目 A* 笔记标记。 或者，如果 `ul` 或 `ol` 未定义 `data-tag`，则没有任何项会显示笔记标记。 无论子 `li` 元素有什么显式设置，都会发生这种覆盖。

- 在下列情况下，唯一的 `data-tag` 设置被视为列表项：

  - 在创建或更新请求中，`li` 元素不嵌套在 `ul` 或 `ol` 中。

  - 对 `li` 元素在更新请求中单独处理。

- 在输入 HTML 中发送的未嵌套 `li` 元素将在输出 HTML 的 `ul` 中返回。

- 在输出 HTML 中，所有 `data-tag` 列表设置都在列表项的 `span` 元素上定义。


以下代码显示如何应用其中的某些规则。 输入 HTML 将使用笔记标记创建两个列表。 输出 HTML 是检索页面内容时针对列表所返回的内容。

#### <a name="input-html"></a>输入 HTML

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

#### <a name="output-html"></a>输出 HTML

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

## <a name="retrieve-note-tags"></a>检索笔记标记

当访问页面内容时，内置笔记标记将包含在输出 HTML 中：

`GET ../api/v1.0/pages/{page-id}/content`

输出 HTML 中的 `data-tag` 属性始终包含形状值，并且仅在它表示设置为“已完成”的复选框笔记标记时才包含状态。 以下示例显示用于创建一些笔记标记的输入 HTML 和返回的输出 HTML。

#### <a name="input-html"></a>输入 HTML

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

#### <a name="output-html"></a>输出 HTML

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

请注意，在列表级别上定义的 `data-tag` 属性会被推送到它的列表项。 有关将笔记标记与列表结合使用的详细信息，请参阅[列表上的笔记标记](#note-tags-on-lists)。

> **注意：** 在输出 HTML 中，定义和后续工作笔记标记均作为 `data-tag="remember-for-later"` 返回。 `title` 元素不返回任何笔记标记信息。




<a name="built-in-tags"></a>

## <a name="built-in-note-tags-for-onenote"></a>OneNote 的内置笔记标记

OneNote 包括以下内置笔记标记：

![所有内置笔记标记。](images/note-tags-all.png)

可以为 `data-tag` 属性分配下列清单中显示的值。 不支持自定义标记。

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

## <a name="response-information"></a>响应信息

Microsoft Graph 在响应中返回以下信息。

| 响应数据 | 说明 |
|------|------|
| 成功代码 | 成功的 POST 请求的 HTTP 状态代码为 201，成功的 PATCH 请求的 HTTP 状态代码为 204。 |
| 错误 | 请阅读 [Microsoft Graph 中 OneNote API 的错误代码](onenote-error-codes.md)，以了解 Microsoft Graph 可以返回的 OneNote 错误。 |


<a name="permissions"></a>

## <a name="permissions"></a>权限

若要创建或更新 OneNote 页面，需要请求相应的权限。 选择应用运行所需的最低级别的权限。

#### <a name="permissions-for-post-pages"></a>POST 页面的权限

- Notes.Create
- Notes.ReadWrite
- Notes.ReadWrite.All

#### <a name="permissions-for-patch-pages"></a>PATCH 页面的权限

- Notes.ReadWrite
- Notes.ReadWrite.All

有关权限范围及其工作方式的详细信息，请参阅 [OneNote 权限范围](permissions-reference.md)。


<a name="see-also"></a>

## <a name="see-also"></a>另请参阅

- [创建 OneNote 页](onenote-create-page.md)
- [更新 OneNote 页内容](onenote-update-page.md)
- [与 OneNote 集成](integrate-with-onenote.md)
- [OneNote 开发者博客](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Microsoft Q&A 上的 OneNote 开发问题](/answers/topics/microsoft-graph-notes.html)
- [OneNote GitHub 存储库](https://go.microsoft.com/fwlink/?LinkID=390178)