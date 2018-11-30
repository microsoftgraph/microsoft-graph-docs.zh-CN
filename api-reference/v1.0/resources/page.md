---
title: 页面资源类型
description: OneNote 笔记本中的页面。
ms.openlocfilehash: 19380f06ad4706f623397681a020054e65eba029
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010947"
---
# <a name="page-resource-type"></a><span data-ttu-id="c8a46-103">页面资源类型</span><span class="sxs-lookup"><span data-stu-id="c8a46-103">page resource type</span></span>

<span data-ttu-id="c8a46-104">OneNote 笔记本中的页面。</span><span class="sxs-lookup"><span data-stu-id="c8a46-104">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8a46-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8a46-105">JSON representation</span></span>

<span data-ttu-id="c8a46-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8a46-106">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenotePage"
}-->

```json
{
  "content": "stream",
  "contentUrl": "string",
  "createdByAppId": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "level": 1024,
  "links": {"@odata.type": "microsoft.graph.pageLinks"},
  "order": 1024,
  "self": "string",
  "title": "string"
}

```
## <a name="properties"></a><span data-ttu-id="c8a46-107">属性</span><span class="sxs-lookup"><span data-stu-id="c8a46-107">Properties</span></span>
| <span data-ttu-id="c8a46-108">属性</span><span class="sxs-lookup"><span data-stu-id="c8a46-108">Property</span></span>     | <span data-ttu-id="c8a46-109">类型</span><span class="sxs-lookup"><span data-stu-id="c8a46-109">Type</span></span>   |<span data-ttu-id="c8a46-110">说明</span><span class="sxs-lookup"><span data-stu-id="c8a46-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8a46-111">内容</span><span class="sxs-lookup"><span data-stu-id="c8a46-111">content</span></span>|<span data-ttu-id="c8a46-112">Stream</span><span class="sxs-lookup"><span data-stu-id="c8a46-112">Stream</span></span>|<span data-ttu-id="c8a46-113">页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="c8a46-113">The page's HTML content.</span></span>|
|<span data-ttu-id="c8a46-114">contentUrl</span><span class="sxs-lookup"><span data-stu-id="c8a46-114">contentUrl</span></span>|<span data-ttu-id="c8a46-115">字符串</span><span class="sxs-lookup"><span data-stu-id="c8a46-115">String</span></span>|<span data-ttu-id="c8a46-p101">页面的 HTML 内容的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="c8a46-p101">The URL for the page's HTML content.  Read-only.</span></span>|
|<span data-ttu-id="c8a46-118">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="c8a46-118">createdByAppId</span></span>|<span data-ttu-id="c8a46-119">字符串</span><span class="sxs-lookup"><span data-stu-id="c8a46-119">String</span></span>|<span data-ttu-id="c8a46-p102">创建页面的应用程序的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="c8a46-p102">The unique identifier of the application that created the page. Read-only.</span></span>|
|<span data-ttu-id="c8a46-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8a46-122">createdDateTime</span></span>|<span data-ttu-id="c8a46-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8a46-123">DateTimeOffset</span></span>|<span data-ttu-id="c8a46-p103">页面的创建日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="c8a46-p103">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="c8a46-128">id</span><span class="sxs-lookup"><span data-stu-id="c8a46-128">id</span></span>|<span data-ttu-id="c8a46-129">字符串</span><span class="sxs-lookup"><span data-stu-id="c8a46-129">String</span></span>|<span data-ttu-id="c8a46-p104">页面的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="c8a46-p104">The unique identifier of the page.  Read-only.</span></span>|
|<span data-ttu-id="c8a46-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8a46-132">lastModifiedDateTime</span></span>|<span data-ttu-id="c8a46-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8a46-133">DateTimeOffset</span></span>|<span data-ttu-id="c8a46-p105">上次修改页面的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="c8a46-p105">The date and time when the page was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="c8a46-138">level</span><span class="sxs-lookup"><span data-stu-id="c8a46-138">level</span></span>|<span data-ttu-id="c8a46-139">Int32</span><span class="sxs-lookup"><span data-stu-id="c8a46-139">Int32</span></span>|<span data-ttu-id="c8a46-p106">页面的缩进级别。只读。</span><span class="sxs-lookup"><span data-stu-id="c8a46-p106">The indentation level of the page. Read-only.</span></span>|
|<span data-ttu-id="c8a46-142">links</span><span class="sxs-lookup"><span data-stu-id="c8a46-142">links</span></span>|[<span data-ttu-id="c8a46-143">PageLinks</span><span class="sxs-lookup"><span data-stu-id="c8a46-143">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="c8a46-p107">用于打开页面的链接。如果安装了 OneNote 本机客户端，则 `oneNoteClientURL` 链接将在其中打开页面。`oneNoteWebUrl` 链接将在 OneNote Online 中打开页面。只读。</span><span class="sxs-lookup"><span data-stu-id="c8a46-p107">Links for opening the page. The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed. The `oneNoteWebUrl` link opens the page in OneNote Online. Read-only.</span></span>|
|<span data-ttu-id="c8a46-148">order</span><span class="sxs-lookup"><span data-stu-id="c8a46-148">order</span></span>|<span data-ttu-id="c8a46-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c8a46-149">Int32</span></span>|<span data-ttu-id="c8a46-p108">页面在其父分区中的顺序。只读。</span><span class="sxs-lookup"><span data-stu-id="c8a46-p108">The order of the page within its parent section. Read-only.</span></span>|
|<span data-ttu-id="c8a46-152">self</span><span class="sxs-lookup"><span data-stu-id="c8a46-152">self</span></span>|<span data-ttu-id="c8a46-153">字符串</span><span class="sxs-lookup"><span data-stu-id="c8a46-153">String</span></span>|<span data-ttu-id="c8a46-p109">可以在其中获取关于页面的详细信息的终结点。只读。</span><span class="sxs-lookup"><span data-stu-id="c8a46-p109">The endpoint where you can get details about the page. Read-only.</span></span>|
|<span data-ttu-id="c8a46-156">title</span><span class="sxs-lookup"><span data-stu-id="c8a46-156">title</span></span>|<span data-ttu-id="c8a46-157">String</span><span class="sxs-lookup"><span data-stu-id="c8a46-157">String</span></span>|<span data-ttu-id="c8a46-158">页面的标题。</span><span class="sxs-lookup"><span data-stu-id="c8a46-158">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c8a46-159">关系</span><span class="sxs-lookup"><span data-stu-id="c8a46-159">Relationships</span></span>
| <span data-ttu-id="c8a46-160">关系</span><span class="sxs-lookup"><span data-stu-id="c8a46-160">Relationship</span></span> | <span data-ttu-id="c8a46-161">类型</span><span class="sxs-lookup"><span data-stu-id="c8a46-161">Type</span></span>   |<span data-ttu-id="c8a46-162">说明</span><span class="sxs-lookup"><span data-stu-id="c8a46-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8a46-163">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="c8a46-163">parentNotebook</span></span>|[<span data-ttu-id="c8a46-164">Notebook</span><span class="sxs-lookup"><span data-stu-id="c8a46-164">Notebook</span></span>](notebook.md)|<span data-ttu-id="c8a46-p110">包含页面的笔记本。只读。</span><span class="sxs-lookup"><span data-stu-id="c8a46-p110">The notebook that contains the page.  Read-only.</span></span>|
|<span data-ttu-id="c8a46-167">parentSection</span><span class="sxs-lookup"><span data-stu-id="c8a46-167">parentSection</span></span>|[<span data-ttu-id="c8a46-168">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="c8a46-168">OnenoteSection</span></span>](section.md)|<span data-ttu-id="c8a46-p111">包含页面的分区。只读。</span><span class="sxs-lookup"><span data-stu-id="c8a46-p111">The section that contains the page. Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="c8a46-171">方法</span><span class="sxs-lookup"><span data-stu-id="c8a46-171">Methods</span></span>

| <span data-ttu-id="c8a46-172">方法</span><span class="sxs-lookup"><span data-stu-id="c8a46-172">Method</span></span>           | <span data-ttu-id="c8a46-173">返回类型</span><span class="sxs-lookup"><span data-stu-id="c8a46-173">Return Type</span></span>    |<span data-ttu-id="c8a46-174">说明</span><span class="sxs-lookup"><span data-stu-id="c8a46-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c8a46-175">Get page</span><span class="sxs-lookup"><span data-stu-id="c8a46-175">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="c8a46-176">Page</span><span class="sxs-lookup"><span data-stu-id="c8a46-176">Page</span></span>](page.md) |<span data-ttu-id="c8a46-177">读取页面的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c8a46-177">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="c8a46-178">Update page content</span><span class="sxs-lookup"><span data-stu-id="c8a46-178">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="c8a46-179">无</span><span class="sxs-lookup"><span data-stu-id="c8a46-179">None</span></span> |<span data-ttu-id="c8a46-180">更新页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="c8a46-180">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="c8a46-181">Delete page</span><span class="sxs-lookup"><span data-stu-id="c8a46-181">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="c8a46-182">无</span><span class="sxs-lookup"><span data-stu-id="c8a46-182">None</span></span> |<span data-ttu-id="c8a46-183">删除页面。</span><span class="sxs-lookup"><span data-stu-id="c8a46-183">Delete the page.</span></span> |
|[<span data-ttu-id="c8a46-184">copyToSection</span><span class="sxs-lookup"><span data-stu-id="c8a46-184">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="c8a46-185">无</span><span class="sxs-lookup"><span data-stu-id="c8a46-185">None</span></span> |<span data-ttu-id="c8a46-186">将页面复制到特定分区。</span><span class="sxs-lookup"><span data-stu-id="c8a46-186">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->