---
title: 更新 OneNote 页面内容
description: " Microsoft 365 中的企业笔记本"
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 8786bcf8a0aa3aafaca8406f11e6243b8dd7b49c
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920101"
---
# <a name="update-onenote-page-content"></a>更新 OneNote 页面内容

**适用于** OneDrive 上的消费者笔记本 | Microsoft 365 上的企业级笔记本


若要更新 OneNote 页面的内容，请向此页面的 *content* 终结点发送 PATCH 请求：

`PATCH ../notes/pages/{id}/content`</p>

在邮件正文中发送 JSON 更改对象。如果请求成功，Microsoft Graph 便会返回 204 HTTP 状态代码。


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a>构建请求 URI

若要构建请求 URI，请从服务根 URL 开始：

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

然后，追加页面的 *content* 终结点：

- **获取页面 HTML 和所有定义的 *data-id* 值**<br/><br/>`../pages/{id}/content`   

- **获取页面 HTML、所有定义的 *data-id* 值和所有生成的 *id* 值**<br/><br/>`../pages/{page-id}/content?includeIDs=true` 

**data-id** 和 **id** 值均用作要更新的元素的 **target** 标识符。

 
完整的请求 URI 将如下所示：<br/><br/>`https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content`


了解有关[服务根 URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url) 的详细信息。


<a name="message-body"></a>

## <a name="construct-the-message-body"></a>构造邮件正文

OneNote 页面的 HTML 包含文本、图像和组织到结构中的其他内容，如 **div**、**img** 和 **ol** 元素。 若要更新 OneNote 页面内容，请添加并替换页面上的 HTML 元素。

所做的更改将以 JSON 更改对象数组的形式在邮件正文中发送。 每个对象指定目标元素、新 HTML 内容以及使用内容可完成的操作。

以下数组定义了两个更改。第一个更改在段落上方插入一张图像作为同级对象，第二个更改向列表中附加一个项目作为最后一个子元素。

> [!NOTE]
> 在 OneNote 页面上更新图像时，你无法使用 www 链接。 该服务不会尝试下载随机资源。 相反，图像必须是请求的一部分，无论是通过 image-data-url 还是多部分请求的部件名称。

```json
[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-data-url-or-part-name" alt="Image above the target paragraph" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the end of the list</li>'
  }
]
```

请参阅[更多示例](#example-requests)。


### <a name="attributes-for-json-change-objects"></a>JSON 更改对象的属性

使用 **target**、**action**、**position** 和 **content** 属性来定义用于 PATCH 请求的 JSON 对象。

#### <a name="target"></a>target

要更新的元素。值必须是下列标识符之一：

| 标示符 | 说明 |  
|------|------|  
| #{data-id} | <p>在[创建页面](onenote-create-page.md)或[更新页面](onenote-update-page.md)时，可以选择在输入 HTML 中的元素上定义此 ID。 将 # 用作此值的前缀。</p><p> 示例：<br/>`'target':'#intro'` 定位元素 `<div data-id="intro" ...>`</p> |  
| id | <p>这是从 Microsoft Graph [生成的 ID](#generated-ids)，对大多数替换操作所都是必需的值。 不要使用 # 作为前缀。</p><p> 示例：<br/>`'target':'div:{33f8a2...}{37}'` 定位元素 `<div id="div:{33f8a2...}{37}" ...>`</p><p>不要将其与 [输入 HTML](onenote-input-output-html.md) 中定义的任何 **id** 值混淆。 所有在输入 HTML 中发送的 **id** 值都将被丢弃。</p> |  
| body | 针对页面上第一个 div 的关键字。 不要使用 # 作为前缀。 |  
| title | 针对页标题的关键字。 不要使用 # 作为前缀。 |  
 
#### <a name="action"></a>action

要在目标元素上执行的操作。请参阅[元素的支持操作](#supported-elements-and-actions)。

| 操作 | 说明 |  
|------|------|  
| append | <p>将提供的内容作为第一个或最后一个子元素添加到由 **position** 属性所确定的目标。</p><p>仅适用于 **body**、**div**、**ol** 和 **ul** 元素。</p> |  
| insert | 将提供的内容作为同级元素添加到由 **position** 属性确定的目标之前或之后。 |  
| prepend | <p>将提供的内容作为第一个子元素添加到目标。 **append** + **before** 的快捷方式。</p><p>仅适用于 **body**、**div**、**ol** 和 **ul** 元素。</p> |  
| replace | <p>使用提供的内容替换目标。</p><p>大多数 **替换** 操作需要为目标使用 [生成的 ID](#generated-ids)（除 div 中的 **img** 和 **object** 元素之外，还支持使用 **data-id**）。</p> |  
 
#### <a name="position"></a>position

要添加所提供的内容的位置，与目标元素有关。如果省略，默认值为 **after**。

| 位置 | 说明 |  
|------|------|  
| after（默认） |<p>使用 **append**：目标元素的最后一个子元素。</p><p>使用 **insert**：目标元素的后续同级元素。</p> |
| before | <p>使用 **append**：目标元素的第一个子元素。</p><p>使用 **insert**：目标元素的前导同级元素。</p> |

#### <a name="content"></a>content

要添加到页面的格式标准的 HTML 字符串或任意图像或二进制文件数据。 如果内容包含二进制数据，则必须使用包含“Commands”部件的 `multipart/form-data` 内容类型发送请求（请参阅[示例](#multipart-request-with-binary-content)）。 
 

<a name="generated-ids"></a>

### <a name="generated-ids"></a>生成的 ID
Microsoft Graph 将为可更新页面上的元素生成 **id** 值。 若要获取生成的 ID，请在 GET 请求中使用 `includeIDs=true` 查询字符串表达式：

`GET ../notes/pages/{page-id}/content?includeIDs=true` 

> **注意：** API 会放弃在创建页面和更新页面请求的 [输入 HTML](onenote-input-output-html.md) 中定义的所有 **id** 值。

以下示例显示了段落的生成 ID，以及页面的[输出 HTML](onenote-input-output-html.md) 中的图像。

```html
<p id="p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}">Some text on the page</p>
<img id="img:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{45}" ... />
```

页面更新后，生成的 **id** 值可能会更改，因此您应该在构建使用当前值的 PATCH 请求之前获取当前值。
 
可以使用 **data-id** 或 **id** 值指定目标元素，如下所示：

- 对于 **append** 和 **insert** 操作，可以使用任一 ID 作为目标值。
- 对于 **replace** 操作，必须为除页标题及 div 中的图像和对象之外的所有元素使用生成的 ID。 
  - 若要替换标题，请使用 **title** 关键字。 
  - 若要替换 div 中的图像和对象，请使用 **data-id** 或 **id**。

以下示例为目标使用了 **id** 值。 不要将 # 前缀用于生成的 ID。

```json
[
   {
    'target':'p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}',
    'action':'insert',
    'position':'before',
    'content':'<p>This paragraph goes above the target paragraph.</p>'
  }
]
```

<a name="support-matrix"></a>

## <a name="supported-elements-and-actions"></a>受支持的元素和操作

可以更新页面上的许多元素，但每个元素类型支持特定操作。 下表显示了支持的目标元素和它们支持的更新操作。

| 元素 | 替换 | 附加子元素 | 插入同级元素 |  
|------|:------:|:------:|:------:|  
| body<br /> （目标为页面上的第一个 div） | 否 | **是** | 否 |  
| div<br /> （[绝对定位](onenote-abs-pos.md)） | 否 | **是** | 否 |  
| div<br /> （在 div 中） | **是**<br/>（仅 ID） | **是** | **是** |   
| img, object<br /> （在 div 中） | **是** | 否 | **是** |   
| ol, ul | **是**<br/>（仅 ID） | **是** | **是** |   
| table | **是**<br/>（仅 ID） | 否 | **是** |   
| p, li, h1-h6 | **是**<br/>（仅 ID） | 否 | **是** |   
| title | **是** | 否 | 否 |  
 
<br/>

以下元素不支持任何更新操作。

- img（[绝对定位](onenote-abs-pos.md)）
- object（[绝对定位](onenote-abs-pos.md)）
- tr, td
- meta
- head
- span
- a
- style tags


<a name="examples"></a>

## <a name="example-requests"></a>示例请求

更新请求包含表示为 JSON 更改对象的一个或多个更改。 这些对象可以定义页面上的不同目标，以及定义目标的不同操作和内容。

以下示例包括 PATCH 请求中使用的 JSON 对象和完整的 PATCH 请求：

- [追加子元素](#append-child-elements)
- [插入同级元素](#insert-sibling-elements)
- [替换元素](#replace-elements)
- [完整的 PATCH 请求](#complete-patch-request-examples)


<a name="append-examples"></a>

### <a name="append-child-elements"></a>追加子元素

**append** 操作向 **body**、**div**（分区内）、**ol** 或 **ul** 元素添加一个子元素。**position** 属性确定是在目标之前还是之后附加子元素。默认位置为 **after**。

#### <a name="append-to-a-div"></a>追加到 div

以下示例将两个子节点添加到 **div1** 元素。 它添加图像作为第一个子元素，添加段落作为最后一个子元素。 

```json
[
 {
    'target':'#div1',
    'action':'append',
    'position':'before',
    'content':'<img data-id="first-child" src="image-url-or-part-name" />'
  },
  {
    'target':'#div1',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph appended to the div</p>'
  }
]
```
 

#### <a name="append-to-the-body-element"></a>追加到 *body* 元素

可以使用 **body** 快捷方式来追加任何页面上的第一个 div 内的子元素。

以下示例将两个段落作为第一个子元素和最后一个子元素添加到页面上第一个 div。 不要将 # 用于 **body** 目标。 此示例使用 **prepend** 操作作为 **append** + **before** 的快捷方式。

```json
[
  {
    'target':'body',
    'action':'prepend',
    'content':'<p data-id="first-child">New paragraph as first child in the first div</p>'
  },
  {
    'target':'body',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph as last child in the first div</p>'
  }
]
```
 

#### <a name="append-to-a-list"></a>追加到列表

以下示例将一个列表项目作为最后一个子元素添加到目标列表。因为项目使用非默认的列表演示，因此应定义 **list-style-type** 属性。

```json
[
  {
    'target':'#circle-ul',
    'action':'append',
    'content':'<li style="list-style-type:circle">Item at the end of the list</li>'
  }
]
```
 

<a name="insert-examples"></a>

### <a name="insert-sibling-elements"></a>插入同级元素

**insert** 操作将同级元素添加到目标元素。 **position** 属性确定要将同级元素插入到目标之前还是之后。 默认位置是 **after**。 请参阅 [支持 **插入** 的元素](#supported-elements-and-actions)。

#### <a name="insert-siblings"></a>插入同级

以下示例向页面添加两个同级节点。它在 **para1** 元素上方添加一个图像，在 **para2** 元素下方添加一个段落。

```json
[
  {
     'target':'#para1',
     'action':'insert',
     'position':'before',
     'content':'<img src="image-data-url-or-part-name" alt="Image inserted above the target" />'
  },
  {
    'target':'#para2',
     'action':'insert',
     'content':'<p data-id="next-sibling">Paragraph inserted below the target</p>'
  }
]
```
 

<a name="replace-examples"></a>

### <a name="replace-elements"></a>替换元素

可以使用 **data-id** 或生成的 **id** 作为目标值来替换 div 中的 **img** 和 **object** 元素。 若要替换页标题，请使用 **title** 关键字。 对于所有其他 [支持 **替换**](#supported-elements-and-actions)的元素，必须使用生成的 ID。

#### <a name="replace-an-image"></a>替换图像

以下示例使用图像的 **data-id** 作为目标来替换 div 中的图像。 

```json
[
  {
    'target':'#img1',
    'action':'replace',
    'content':'<div data-id="new-div"><p>This div replaces the image</p></div>'
  }
]
```
 

#### <a name="update-a-table"></a>更新表格 

此示例显示如何使用生成的 ID 更新表格。不支持替换 **tr** 和 **td** 元素，但您可以替换整个表格。

```json
[
  {
    'target':'table:{de3e0977-94e4-4bb0-8fee-0379eaf47486}{11}',
    'action':'replace',
    'content':'<table data-id="football">
      <tr><td><p><b>Brazil</b></p></td><td><p>Germany</p></td></tr>
      <tr><td><p>France</p></td><td><p><b>Italy</b></p></td></tr>
      <tr><td><p>Netherlands</p></td><td><p><b>Spain</b></p></td></tr>
      <tr><td><p>Argentina</p></td><td><p><b>Germany</b></p></td></tr></table>'
  }
]
```
 

#### <a name="change-the-title"></a>更改标题 

此示例说明如何更改页面的标题。 若要更改标题，请使用 **title** 关键字作为目标值。 不要将 # 用于标题目标。

```json
[
  {
    'target':'title',
    'action':'replace',
    'content':'New title'
  }
]
```
 

#### <a name="update-a-to-do-item"></a>更新待办事项

以下示例使用替换操作将待办事项复选框项更改为完成状态。

```json
[
  {
    'target':'#task1',
    'action':'replace',
    'content':'<p data-tag="to-do:completed" data-id="task1">First task</p>'
  }
]
```

有关使用 **data-tag** 属性的详细信息，请参阅 [使用注释标记](onenote-note-tags.md)。


<a name="complete-requests"></a>

### <a name="complete-patch-request-examples"></a>完整的 PATCH 请求示例

以下示例显示了完整的 PATCH 请求。

#### <a name="request-with-text-content-only"></a>仅包含文本内容的请求

以下示例显示使用 **application/json** 内容类型的 PATCH 请求。 内容不包含二进制数据时，可使用此格式。

```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: application/json
Authorization: Bearer {token}

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-data-url" alt="New image from a URL" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]
```
 
<a name="multipart"></a>

#### <a name="multipart-request-with-binary-content"></a>包含二进制内容的多部分请求 

以下示例显示包含二进制数据的多部分 PATCH 请求。 多部分请求需要指定 **application/json** 内容类型并包含 JSON 更改对象数组的“Commands”部件。 其他数据部件可包含二进制数据。 部件名称通常是附加有毫秒为单位或随机 GUID 当前时间的字符串。

```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: multipart/form-data; boundary=PartBoundary123
Authorization: Bearer {token}

--PartBoundary123
Content-Disposition: form-data; name="Commands"
Content-Type: application/json

[
  {
    'target':'img:{2998967e-69b3-413f-a221-c1a3b5cbe0fc}{42}',
    'action':'replace',
    'content':'<img src="name:image-part-name" alt="New binary image" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]

--PartBoundary123
Content-Disposition: form-data; name="image-part-name"
Content-Type: image/png

... binary image data ...

--PartBoundary123--
```

<a name="request-response-info"></a>

## <a name="request-and-response-information-for-patch-requests"></a>PATCH 请求的请求和响应信息

| 请求数据 | 说明 |  
|------|------|  
| 协议 | 所有请求均使用 SSL/TLS HTTPS 协议。 |  
| 授权标头 | <p>`Bearer {token}`，其中 `{token}` 是已注册应用的一个有效 OAuth 2.0 访问令牌。</p><p>如果缺少或无效，则请求失败，并显示 401 状态代码。 请参阅[身份验证和权限](permissions-reference.md)。</p> |  
| Content-Type 标头 | <p>JSON 更改对象的数组的 `application/json`，确定是直接在邮件正文中发送还是在必须的[多部分请求](#multipart-request-with-binary-content)的“命令”部分中发送。</p><p>发送二进制数据时，多部分请求是必需的，并使用 `multipart/form-data; boundary=part-boundary` 内容类型，其中 `{part-boundary}` 是一个字符串，表示每个数据部件的开始和结束。</p> |  

<br/> 

| 响应数据 | 说明 |  
|------|------|  
| 成功代码 | 204 HTTP 状态代码。PATCH 请求未返回任何 JSON 数据。 |  
| 错误 | 请阅读 [Microsoft Graph 中 OneNote API 的错误代码](onenote-error-codes.md)，以了解 Microsoft Graph 可以返回的 OneNote 错误。 |  
 
 

<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a>构建 Microsoft Graph 服务根 URL

OneNote 服务根 URL 为 OneNote API 的所有调用使用以下格式：

`https://graph.microsoft.com/{version}/me/onenote/`

URL 中的 `version` 段表示想要使用的 Microsoft Graph 的版本。 `v1.0` 用于稳定的生产代码。 `beta` 用于试用正在开发的功能。 Beta 版中的特性和功能可能会有所更改，因此，不应将其用于生产代码。

`me` 用于为当前用户可以访问的 OneNote 内容（拥有和共享）。 `users/{id}` 用于指定用户已与当前用户共享的 OneNote 内容（此 URL 中）。 使用 [Azure AD 图形 API](/previous-versions/azure/ad/graph/api/api-catalog)。


> **注意：** 可以通过在 `https://graph.microsoft.com/v1.0/users` 上发出 GET 请求来获取用户 ID。



<a name="permissions"></a>

## <a name="permissions"></a>权限

若要更新 OneNote 页面，需要请求相应的权限。 选择应用运行所需的最低级别的权限。

- Notes.ReadWrite
- Notes.ReadWrite.All

有关权限范围及其工作方式的详细信息，请参阅 [OneNote 权限范围](permissions-reference.md)。
   

<a name="see-also"></a>

## <a name="see-also"></a>另请参阅

- [添加图像和文件](onenote-images-files.md)
- [与 OneNote 集成](integrate-with-onenote.md)
- [OneNote 开发者博客](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Microsoft Q&A 上的 OneNote 开发问题](/answers/topics/microsoft-graph-notes.html)
- [OneNote GitHub 存储库](https://go.microsoft.com/fwlink/?LinkID=390178)