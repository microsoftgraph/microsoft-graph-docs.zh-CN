---
title: 使用 OneNote API 获取 OneNote 内容和结构
description: 向目标终结点发送 GET 请求，获取 OneNote 内容和结构。 然后使用查询字符串选项筛选查询并提高性能。
author: jewan-microsoft
ms.localizationpriority: high
ms.prod: onenote
ms.openlocfilehash: 31bcfd207fca8e04f4d476f243752476c65d8a1e
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446173"
---
# <a name="get-onenote-content-and-structure"></a>获取 OneNote 内容和结构

**适用于**：OneDrive 上的消费者笔记本 | Microsoft 365 上的企业级笔记本

若要使用 Microsoft Graph OneNote API 获取 OneNote 内容和结构，请向目标终结点发送 GET 请求。 例如：

`GET ../onenote/pages/{id}`

如果请求成功，Microsoft Graph 会返回 `200 OK` HTTP 状态代码以及请求的实体或内容。 OneNote 实体作为符合 OData 版本 4.0 规范的 JSON 对象返回。

通过使用查询字符串选项，可以筛选查询并提高性能。

> [!NOTE]
> 如果正在构建支持以下方案之一的解决方案，则会达到 OneNote API 限制：
> - 备份/还原 OneNote 部分
> - 备份/还原 OneNote 笔记本
>
> 有关备份和还原操作，请参阅 [发现文件和检测大规模更改的最佳做法](/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online&preserve-view=true)。

<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a>构建请求 URI

若要构建请求 URI，请从服务根 URL 开始：

`https://graph.microsoft.com/v1.0/me/onenote`

然后追加要检索的资源的终结点。 （[资源路径](#resource-paths-for-get-requests)会显示在下一个节中。）

完整的请求 URI 类似于以下示例之一：

- `https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections`
- `https://graph.microsoft.com/v1.0/me/onenote/notes/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?select=title,self`

> [!NOTE]
> 了解有关[服务根 URL](/graph/api/resources/onenote-api-overview#root-url) 的详细信息。

<a name="resource-paths"></a>

## <a name="resource-paths-for-get-requests"></a>GET 请求的资源路径

使用以下资源路径获取页面、节、节组、笔记本和图像或文件资源。

- [页面集合](#page-collection)
- [页面实体](#page-entity)
- [页面预览](#page-preview)
- [页面 HTML 内容](#page-html-content)
- [节集合](#section-collection)
- [节实体](#section-entity)
- [SectionGroup 集合](#sectiongroup-collection)
- [SectionGroup 实体](#sectiongroup-entity)
- [笔记本集合](#notebook-collection)
- [笔记本实体](#notebook-entity)
- [图像或其他文件资源](#image-or-other-file-resource)

<a name="get-pages"></a>

### <a name="page-collection"></a>页面集合

获取所有笔记本的页面（元数据）。

`../pages[?filter,orderby,select,expand,top,skip,search,count]`

从特定节获取页面（元数据）。

`../sections/{section-id}/pages[?filter,orderby,select,expand,top,skip,search,count,pagelevel]`
 
`search` 查询字符串选项仅适用于消费者笔记本。

页面的默认排序顺序是 `lastModifiedTime desc`。

默认查询将展开父节并选择节的 `id`、`name` 和 `self` 属性。

默认情况下，为 *GET 页面* 请求返回仅前 20 个实体。 未指定 **top** 查询字符串选项的请求将在响应中返回 `@odata.nextLink` 链接，该链接可用于获取接下来的 20 个条目。

对于节中的页面集合，使用 **pagelevel** 返回页面的缩进级别及其在节中的顺序。 

#### <a name="example"></a>示例

`GET ../sections/{section-id}/pages?pagelevel=true`

<a name="get-page"></a> 

### <a name="page-entity"></a>页面实体

获取特定页面的元数据。 

`../pages/{page-id}[?select,expand,pagelevel]`

页面可以展开 **parentNotebook** 和 **parentSection** 属性。

默认查询将展开父节并选择节的 `id`、`name` 和 `self` 属性。

使用 **pagelevel** 返回页面的缩进级别及其在父节中的顺序。

#### <a name="example"></a>示例

`GET ../pages/{page-id}?pagelevel=true`

<a name="get-page-preview"></a> 

### <a name="page-preview"></a>页面预览

获取页面的文字和图像预览内容。

`../pages/{page-id}/preview`


JSON 响应包含预览内容，可用于帮助用户标识页面中的内容。

```json
{
  "@odata.context":"https://www.onenote.com/api/v1.0/$metadata#Microsoft.OneNote.Api.PagePreview",
  "previewText":"text-snippet",
  "links":{
    "previewImageUrl":{
      "href":"https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png"
    }
  }
}
```

**previewText** 属性包含来自页面的文本片段。 Microsoft Graph 返回完整短语，最多 300 个字符。 

如果页面具有可用于生成预览 UI 的图像，则 **previewImageUrl** 对象中的 **href** 属性包含指向公共 [映像资源](#image-or-other-file-resource) 的链接。可以在 HTML 中使用此链接。否则，**href** 返回 null。

#### <a name="example"></a>示例 

`<img src="https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png" />`

<a name="get-page-content"></a> 

### <a name="page-html-content"></a>页面 HTML 内容

获取页面的 HTML 内容。

`../pages/{page-id}/content[?includeIDs]`

（*了解有关 [返回的 HTML 内容](onenote-input-output-html.md)* 的详细信息） 


使用 **includeIDs=true** 查询字符串选项获取生成的 ID，用于 [更新页面](onenote-update-page.md)。

<a name="get-sections"></a>

### <a name="section-collection"></a>节集合

获取用户拥有的所有笔记本的所有节，包括嵌套节组中的节。

`../sections[?filter,orderby,select,top,skip,expand,count]`

获取直接位于特定节组下的所有节。

`../sectionGroups/{sectiongroup-id}/sections[?filter,orderby,select,top,skip,expand,count]`

获取直接位于特定笔记本下的所有节。

`../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]`

节可以展开 **parentNotebook** 和 **parentSectionGroup** 属性。

节的默认排序顺序是 `name asc`。

默认查询将展开父笔记本和父节组，并选择它们的 `id`、`name` 和 `self` 属性。

<a name="get-section"></a>

### <a name="section-entity"></a>节实体

获取特定节。

`../sections/{section-id}[?select,expand]`

节可以展开 **parentNotebook** 和 **parentSectionGroup** 属性。

默认查询将展开父笔记本和父节组，并选择它们的 `id`、`name` 和 `self` 属性。

<a name="get-section-groups"></a>

### <a name="sectiongroup-collection"></a>SectionGroup 集合

获取用户拥有的所有笔记本的所有节组，包括嵌套节组。

`../sectionGroups[?filter,orderby,select,top,skip,expand,count]`

获取直接位于特定笔记本下的所有节组。 

`../notebooks/{notebook-id}/sectionGroups[?filter,orderby,select,top,skip,expand,count]`

节组可以展开 **sections**、**sectionGroups**、**parentNotebook** 和 **parentSectionGroup** 属性。

节组的默认排序顺序是 `name asc`。

默认查询将展开父笔记本和父节组，并选择它们的 `id`、`name` 和 `self` 属性。

<a name="get-section-group"></a>

### <a name="sectiongroup-entity"></a>SectionGroup 实体

获取特定节组。

`../sectionGroups/{sectiongroup-id}[?select,expand]`

节组可以展开 **sections**、**sectionGroups**、**parentNotebook** 和 **parentSectionGroup** 属性。

默认查询将展开父笔记本和父节组，并选择它们的 `id`、`name` 和 `self` 属性。

<a name="get-notebooks"></a>

### <a name="notebook-collection"></a>笔记本集合

获取用户拥有的所有笔记本。 

`../notebooks[?filter,orderby,select,top,skip,expand,count]`

笔记本可以展开 **sections** 和 **sectionGroups** 属性。

笔记本的默认排序顺序是 `name asc`。 

<a name="get-notebook"></a>

### <a name="notebook-entity"></a>笔记本实体

获取特定笔记本。

`../notebooks/{notebook-id}[?select,expand]`

笔记本可以展开 **sections** 和 **sectionGroups** 属性。

<a name="get-resource"></a>

### <a name="image-or-other-file-resource"></a>图像或其他文件资源

获取特定资源的二进制数据。 

`../resources/{resource-id}/$value`

可以在页面的[输出 HTML](onenote-input-output-html.md) 中找到文件的资源 URI。

例如，**img** 标记包含 **data-fullres-src** 属性中原始图像的终结点和 **src** 属性中经优化图像的终结点。 

#### <a name="example"></a>示例

```html
<img 
    src="https://www.onenote.com/api/v1.0/me/notes/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://www.onenote.com/api/v1.0/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

**object** 标记包含 **data** 属性中文件资源的终结点。 

#### <a name="example"></a>示例

```html
<object
    data="https://www.onenote.com/api/v1.0/me/notes/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" ... />
```

> [!NOTE]
> 不支持获取资源的集合。 

在获取文件资源时，无需在请求中包含 **Accept** 内容类型。

有关 GET 请求的详细信息，请参阅 Microsoft Graph API REST 引用中的以下资源：

- [GET 页面](/graph/api/page-get)
- [GET 节](/graph/api/section-get)
- [GET 节组](/graph/api/sectiongroup-get)
- [GET 笔记本](/graph/api/notebook-get)




<a name="example"></a>

## <a name="example-get-requests"></a>示例 GET 请求

可以查询 OneNote 实体和搜索页面内容以仅获取所需的信息。 以下示例演示了一些方法，可以在对 Microsoft Graph 的 GET 请求中使用[支持的查询字符串选项](#supported-odata-query-string-options)。 

**请注意：**

- 所有的 GET 请求都以[服务根 URL](/graph/api/resources/onenote-api-overview#root-url) 开头。
  
  **示例**：`https://www.onenote.com/api/v1.0/me/notes` 和 `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`

- URL 查询字符串中的空格必须使用 %20 编码。

  **示例**：`filter=title%20eq%20'biology'`

- 属性名和 OData 字符串比较均区分大小写。 建议使用 OData **tolower** 函数进行字符串比较。

  **示例**：`filter=tolower(name) eq 'spring'`

### <a name="search--filter"></a>search & filter  

获取包含由特定应用创建的术语 *recipe* 的所有页面（`search` 仅适用于消费者笔记本）。

```
[GET] ../pages?search=recipe&filter=createdByAppId eq 'WLID-000000004C12821A'
```
 
### <a name="search--select"></a>search & select  

获取包含术语 *golgi app* 的所有页面的标题、OneNote 客户端链接和 **contentUrl** 链接（`search` 仅适用于消费者笔记本）。

```
[GET] ../pages?search=golgi app&select=title,links,contentUrl
```
 
### <a name="expand"></a>expand 

获取所有笔记本，并展开它的节和节组。  

```
[GET] ../notebooks?expand=sections,sectionGroups
```

<br/>

获取某个特定的节组，并展开它的节和节组。  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections,sectionGroups
```

<br/>

获取一个页面并展开其父节和父笔记本。

```
[GET] ../pages/{page-id}?expand=parentSection,parentNotebook
```

### <a name="expand-multiple-levels"></a>expand（多个级别）  

获取所有笔记本，展开其节和节组，并在每个节组中展开所有节。  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections)
```
 
> [!NOTE]
> 展开子实体的父项或展开父实体的子项来创建循环引用，这并不受支持。

 
### <a name="expand--select-multiple-levels"></a>expand & select（多个级别）  

获取特定节组的名称和 **self** 链接，并获取其所有节的名称和 **self** 链接。  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections(select=name,self)&select=name,self
```

<br/>

获取所有节的名称和 **self** 链接，并获取每个节的父笔记本的名称和创建时间。  

```
[GET] ../sections?expand=parentNotebook(select=name,createdTime)&select=name,self
```

<br/>
 
获取所有页面的标题和 ID，并获取父节和父笔记本的名称。

```
[GET] ../pages?select=id,title&expand=parentSection(select=name),parentNotebook(select=name)
```

### <a name="expand--levels-multiple-levels"></a>expand & levels（多个级别）  

获取所有笔记本、节和节组。  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections,sectionGroups(levels=max;expand=sections))
```
 
### <a name="filter"></a>filter

获取 2014 年 10 月创建的所有节。

```
[GET] ../sections?filter=createdTime ge 2014-10-01 and createdTime le 2014-10-31
```

<br/>

获取某个特定应用自 2015 年 1 月 1 日以来所创建的页面。

```
[GET] ../pages?filter=createdByAppId eq 'WLID-0000000048118631' and createdTime ge 2015-01-01
```

### <a name="filter--expand"></a>filter & expand  

获取特定笔记本中的所有页面。 默认情况下，API 返回 20 个条目。

```
[GET] ../pages?filter=parentNotebook/id eq '{notebook-id}'&expand=parentNotebook
```

<br/>

获取 *School* 笔记本的所有节的名称和 **pagesUrl** 链接。 OData 字符串比较区分大小写，因此，作为最佳做法将使用 **tolower** 函数。

```
[GET] ../notebooks?filter=tolower(name) eq 'school'&expand=sections(select=name,pagesUrl)
```

### <a name="filter--select--orderby"></a>filter & select & orderby   

获取节名称中包含术语 *spring* 的所有节的名称和 **pagesUrl** 链接。按最后修改的日期对节进行排序。

```
[GET] ../sections?filter=contains(tolower(name),'spring')&select=name,pagesUrl&orderby=lastModifiedTime desc
```
 
### <a name="orderby"></a>orderby

获取按 **createdByAppId** 属性排序的前 20 个页面，然后按最近创建时间排序。默认情况下，此 API 返回 20 个条目。

```
[GET] ../pages?orderby=createdByAppId,createdTime desc
```

### <a name="search--filter--top"></a>search & filter & top 

获取自 2015 年 1 月 1 日以来创建的包含短语 *cell division* 的 5 个最新页面。 默认情况下，此 API 返回 20 个条目，最多返回 100 个条目。 页面的默认排序顺序为 `lastModifiedTime desc`（`search` 仅适用于消费者笔记本）。

```
[GET] ../pages?search="cell division"&filter=createdTime ge 2015-01-01&top=5
```

### <a name="search--filter--top--skip"></a>search & filter & top & skip  

获取结果集中接下来的五个页面（`search` 仅适用于消费者笔记本）。

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=5
```

<br/>

以及接下来的五页（`search` 仅适用于消费者笔记本）。

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=10
```

> [!NOTE]
> 如果 **search** 和 **filter** 都应用于同一请求，则结果只包含与这两个条件都匹配的实体。
 
### <a name="select"></a>select

获取用户笔记本中所有节的名称、创建时间和 **self** 链接。

```
[GET] ../sections?select=name,createdTime,self
```

<br/>

获取特定页面的标题、创建时间和 OneNote 客户端链接。

```
[GET] ../pages/{page-id}?select=title,createdTime,links
```

### <a name="select--expand--filter-multiple-levels"></a>select & expand & filter（多个级别）  

获取用户的默认笔记本中所有节的名称和 **pagesUrl** 链接。

```
[GET] ../notebooks?select=name&expand=sections(select=name,pagesUrl)&filter=isDefault eq true
```

### <a name="top--select--orderby"></a>top & select & orderby 

获取按标题字母顺序排序的前 50 个页面的标题和 **self** 链接。 默认情况下，此 API 返回 20 个条目，最多返回 100 个条目。 页面的默认排序顺序是 `lastModifiedTime desc`。

```
[GET] ../pages?top=50&select=title,self&orderby=title
```

### <a name="skip--top--select--orderby"></a>skip & top & select & orderby  

获取第 51 至 100 页。默认情况下，此 API 返回 20 个条目，最多返回 100 个条目。

```
[GET] ../pages?skip=50&top=50&select=title,self&orderby=title
```

> [!NOTE]
> 对于检索默认条目数量（即它们不指定 **top** 表达式）的页面的 GET 请求，会在响应中返回一个 **\@odata.nextLink** 链接，可使用此链接获取接下来的 20 个条目。
 

<a name="supported-odata-query-string-options"></a>

## <a name="supported-odata-query-string-options"></a>受支持的 OData 查询字符串选项

在将 GET 请求发送到 Microsoft Graph 时，可以使用 OData 查询字符串选项来自定义查询并获取所需信息。它们还可以通过减少对服务的调用量和减少响应负载的大小来提高性能。

> [!NOTE]
> 为了增强可读性，本文中的示例不使用 URL 查询字符串中空格所需的 %20 百分比编码：`filter=isDefault%20eq%20true`
 
| 查询选项 | 示例和说明 |  
|------|------|  
| count | <p>`count=true`</p><p>集合中的实体计数。在响应的 **\@odata.count** 属性中返回此值。</p> |  
| expand | <p>`expand=sections,sectionGroups`</p><p>要在响应中内嵌返回的导航属性。**expand** 表达式支持以下属性:<br /> - 页面：**parentNotebook**、**parentSection**<br /> - 节：**parentNotebook**、**parentSectionGroup**<br /> - 节组：**sections**、**sectionGroups**、**parentNotebook**、**parentSectionGroup**<br /> - 笔记本：**sections**、**sectionGroups**</p><p>默认情况下，页面的 GET 请求同时展开 **parentSection** 并选择该节的 **id**、**name** 和 **self** 属性。节和节组的默认 GET 请求扩展 **parentNotebook** 和 **parentSectionGroup**，并选择父项的 **id**、**name** 和 **self** 属性。</p><p>可用于单个实体或集合。<br />使用逗号分隔多个属性。<br />属性名区分大小写。</p> |   
| filter | <p>`filter=isDefault eq true`</p><p>是否在结果集中包含条目的布尔表达式。 支持以下 OData 运算符和函数：<br /> - 比较运算符：**eq**、**ne**、**gt**、**ge**、**lt**、**le**<br /> - 逻辑运算符：**and**、**or**、**not**<br /> - 字符串函数：**contains**、**endswith**、**startswith**、**length**、**indexof**、**substring**、**tolower**、**toupper**、**trim**、**concat**</p><p>[属性](#onenote-entity-properties)名和 OData 字符串比较均区分大小写。 建议使用 OData **tolower** 函数进行字符串比较。<br /><br />**示例**：`filter=tolower(name) eq 'spring'`</p> |  
| orderby | <p>`orderby=title,createdTime desc`</p><p>作为排序依据的 [属性](#onenote-entity-properties)，具有可选的 **asc**（默认）或 **desc** 的排序顺序。您可以按请求集合中实体的任意属性进行排序。</p><p>笔记本、节组和节的默认排序顺序为 `name asc`，页面的默认排序顺序为 `lastModifiedTime desc`（最后修改的页面排第一）。</p><p>用逗号隔开多个属性，并按您想要应用属性的顺序列出它们。属性名称区分大小写。</p> |  
| search | <p>`search=cell div`</p><p>仅适用于消费者笔记本。</p><p>要在页面标题、页面正文、图像替换文字、图像 OCR 文本中搜索的术语或短语。默认情况下，搜索查询返回按相关性排序的结果。</p><p>OneNote 使用必应全文搜索来支持短语搜索、词干分解、拼写宽容、相关性和排名、断字、多语言以及其他全文搜索功能。搜索字符串不区分大小写。</p><p>仅适用于用户拥有的笔记本中的页面。 已编入索引的内容具有私密性，只有所有者才能访问。 受密码保护的页面未编入索引。 仅适用于 `pages` 终结点。</p> |  
| select | <p>`select=id,title`</p><p>要返回的[属性](#onenote-entity-properties)。 可用于单个实体或集合。 使用逗号分隔多个属性。 属性名区分大小写。</p> |  
| skip | <p>`skip=10`</p><p>结果集中要跳过的条目数量。通常用于分页结果。</p> |  
| top | <p>`top=50`</p><p>结果集中要返回的条目数量，最多可达 100 个条目。默认值为 20。</p> |  

Microsoft Graph 还提供 `pagelevel` 查询字符串选项，可使用该选项获取父节内页面的级别和顺序。 仅适用于特定节中页面的查询或特定页面中的查询。 

#### <a name="examples"></a>示例 

- `GET ../sections/{section-id}/pages?pagelevel=true` 
- `GET ../pages/{page-id}?pagelevel=true` 

### <a name="supported-odata-operators-and-functions"></a>受支持的 OData 运算符和函数

Microsoft Graph 支持 **filter** 表达式中的以下 OData 运算符和函数。 使用 OData 表达式时，请记住：

- 必须将 URL 查询字符串中的空格替换为 `%20` 编码。

  **示例：** `filter=isDefault%20eq%20true`

- 属性名和 OData 字符串比较均区分大小写。 建议使用 OData **tolower** 函数进行字符串比较。

  **示例：** `filter=tolower(name) eq 'spring'`


| 比较运算符 | 示例 |  
|------|------|  
| eq<br />（等于） | `createdByAppId eq '{app-id}'` |  
| ne<br />（不等于） | `userRole ne 'Owner'` |  
| gt<br />（大于） | `createdTime gt 2014-02-23` |  
| ge<br />（大于或等于） | `lastModifiedTime ge 2014-05-05T07:00:00Z` |  
| lt<br />（小于） | `createdTime lt 2014-02-23` |  
| le<br />（小于或等于） | `lastModifiedTime le 2014-02-23` |  

<br/>

| 逻辑运算符 | 示例 |  
|------|------|  
| 和 | `createdTime le 2014-01-30 and createdTime gt 2014-01-23` |  
| 或 | `createdByAppId eq '{app-id}' or createdByAppId eq '{app-id}'` |  
| 
not | `not contains(tolower(title),'school')` |  

<br/>

| 字符串函数 | 示例 |  
|------|------|   
| contains | `contains(tolower(title),'spring')` |  
| endswith | `endswith(tolower(title),'spring')` |  
| startswith | `startswith(tolower(title),'spring')` |  
| length | `length(title) eq 19` |  
| indexof | `indexof(tolower(title),'spring') eq 1` |  
| substring | `substring(tolower(title),1) eq 'spring'` |  
| tolower | `tolower(title) eq 'spring'` |  
| toupper | `toupper(title) eq 'SPRING'` |  
| trim | `trim(tolower(title)) eq 'spring'` |  
| concat | `concat(title,'- by MyRecipesApp') eq 'Carrot Cake Recipe - by MyRecipesApp'` |  
 

<a name="properties"></a>

## <a name="onenote-entity-properties"></a>OneNote 实体属性

**filter**、**select**、**expand** 和 **orderby** 查询表达式可以包含 OneNote 实体的属性。 

#### <a name="example"></a>示例

`../sections?filter=createdTime ge 2015-01-01&select=name,pagesUrl&orderby=lastModifiedTime desc` 

查询表达式中的属性名称区分大小写。

有关属性列表和属性类型，请参阅 Microsoft Graph API REST 引用中的以下资源：

- [GET 页面](/graph/api/page-get)
- [GET 节](/graph/api/section-get)
- [GET 节组](/graph/api/sectiongroup-get)
- [GET 笔记本](/graph/api/notebook-get)


**expand** 查询字符串选项可与以下导航属性一起使用：

- 页面：**parentNotebook**、**parentSection**
- 节：**parentNotebook**、**parentSectionGroup**
- 节组：**sections**、**sectionGroups**、**parentNotebook**、**parentSectionGroup**
- 笔记本：**sections**、**sectionGroups**


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-get-requests"></a>*GET* 请求的请求和响应信息

| 请求数据 | 说明 |  
|------|------|  
| 协议 | 所有请求均使用 SSL/TLS HTTPS 协议。 |  
| 授权标头 | <p>`Bearer {token}`，其中 `{token}` 是已注册应用的一个有效 OAuth 2.0 访问令牌。</p><p>如果丢失或无效，则请求将失败，并显示 401 状态代码。请参阅 [身份验证和权限](permissions-reference.md)。</p> |  
| 接受标头 | <p> `application/json` 适用于 OneNote 实体和实体集</p><p> `text/html` 适用于页面内容</p> | 

<br/>

| 响应数据 | 说明 |  
|------|------|  
| 成功代码 | 200 HTTP 状态代码。 |  
| 响应正文 | JSON 格式、页面 HTML 或文件资源二进制数据中的实体或实体集的 OData 表示形式。  |  
| 错误 | 如果请求失败，API 将在响应正文的 **\@api.diagnostics** 对象中返回 [错误](onenote-error-codes.md)。 |  
| X-CorrelationId 标头 | 唯一标识请求的 GUID。在与 Microsoft 支持部门协作来解决问题时，可以使用此值和日期标头值。 |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-notes-service-root-url"></a>构建 Microsoft Graph 笔记服务根 URL

Microsoft Graph 笔记根 URL 为 Microsoft Graph 笔记的所有调用使用以下格式：

`https://graph.microsoft.com/{version}/me/onenote/`  

URL 中的 `version` 段表示想要使用的 Microsoft Graph 的版本。 `v1.0` 用于稳定的生产代码。 `beta` 用于试用正在开发的功能。 Beta 版中的特性和功能可能会有所更改，因此，不应将其用于生产代码。 

为当前用户可以访问的 OneNote 内容（拥有和共享）使用 `me`。 为指定用户已与当前用户共享的 OneNote 内容（此 URL 中）使用 `users/{id}`。 使用 [Microsoft Graph](https://graph.microsoft.com/v1.0/users) 获取用户 ID。 


<a name="permissions"></a>

## <a name="permissions-for-get-requests"></a>GET 请求的权限

若要获取 OneNote 内容或结构，需要请求相应的权限。 

以下范围允许对 Microsoft Graph 执行 GET 请求。 选择应用运行所需的最低级别的权限。

从以下项中进行选择：

- Notes.read
- Notes.ReadWrite
- Notes.ReadWrite.All

有关权限范围及其工作方式的详细信息，请参阅 [Microsoft Graph 权限引用](permissions-reference.md)。

<a name="see-also"></a>

## <a name="see-also"></a>另请参阅

- [OneNote 页面的输入和输出 HTML](onenote-input-output-html.md)
- [与 OneNote 集成](integrate-with-onenote.md)
- [OneNote 开发者博客](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Microsoft Q&A 上的 OneNote 开发问题](/answers/topics/microsoft-graph-notes.html)
- [OneNote GitHub 存储库](https://go.microsoft.com/fwlink/?LinkID=390178)
