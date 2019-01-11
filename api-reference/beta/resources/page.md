---
title: 页面资源类型
description: OneNote 笔记本中的页面。
localization_priority: Normal
ms.openlocfilehash: 5928f430fcbfe9f41c6aa83e99d7dfe737e8e1c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850132"
---
# <a name="page-resource-type"></a><span data-ttu-id="869a8-103">页面资源类型</span><span class="sxs-lookup"><span data-stu-id="869a8-103">page resource type</span></span>

> <span data-ttu-id="869a8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="869a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="869a8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="869a8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="869a8-106">OneNote 笔记本中的页面。</span><span class="sxs-lookup"><span data-stu-id="869a8-106">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="869a8-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="869a8-107">JSON representation</span></span>

<span data-ttu-id="869a8-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="869a8-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
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
## <a name="properties"></a><span data-ttu-id="869a8-109">属性</span><span class="sxs-lookup"><span data-stu-id="869a8-109">Properties</span></span>
| <span data-ttu-id="869a8-110">属性</span><span class="sxs-lookup"><span data-stu-id="869a8-110">Property</span></span>     | <span data-ttu-id="869a8-111">类型</span><span class="sxs-lookup"><span data-stu-id="869a8-111">Type</span></span>   |<span data-ttu-id="869a8-112">说明</span><span class="sxs-lookup"><span data-stu-id="869a8-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="869a8-113">内容</span><span class="sxs-lookup"><span data-stu-id="869a8-113">content</span></span>|<span data-ttu-id="869a8-114">Stream</span><span class="sxs-lookup"><span data-stu-id="869a8-114">Stream</span></span>|<span data-ttu-id="869a8-115">页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="869a8-115">The page's HTML content.</span></span>|
|<span data-ttu-id="869a8-116">contentUrl</span><span class="sxs-lookup"><span data-stu-id="869a8-116">contentUrl</span></span>|<span data-ttu-id="869a8-117">字符串</span><span class="sxs-lookup"><span data-stu-id="869a8-117">String</span></span>|<span data-ttu-id="869a8-p102">页面的 HTML 内容的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="869a8-p102">The URL for the page's HTML content.  Read-only.</span></span>|
|<span data-ttu-id="869a8-120">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="869a8-120">createdByAppId</span></span>|<span data-ttu-id="869a8-121">字符串</span><span class="sxs-lookup"><span data-stu-id="869a8-121">String</span></span>|<span data-ttu-id="869a8-p103">创建页面的应用程序的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="869a8-p103">The unique identifier of the application that created the page. Read-only.</span></span>|
|<span data-ttu-id="869a8-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="869a8-124">createdDateTime</span></span>|<span data-ttu-id="869a8-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="869a8-125">DateTimeOffset</span></span>|<span data-ttu-id="869a8-p104">页面的创建日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="869a8-p104">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="869a8-130">id</span><span class="sxs-lookup"><span data-stu-id="869a8-130">id</span></span>|<span data-ttu-id="869a8-131">字符串</span><span class="sxs-lookup"><span data-stu-id="869a8-131">String</span></span>|<span data-ttu-id="869a8-p105">页面的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="869a8-p105">The unique identifier of the page.  Read-only.</span></span>|
|<span data-ttu-id="869a8-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="869a8-134">lastModifiedDateTime</span></span>|<span data-ttu-id="869a8-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="869a8-135">DateTimeOffset</span></span>|<span data-ttu-id="869a8-p106">上次修改页面的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="869a8-p106">The date and time when the page was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="869a8-140">level</span><span class="sxs-lookup"><span data-stu-id="869a8-140">level</span></span>|<span data-ttu-id="869a8-141">Int32</span><span class="sxs-lookup"><span data-stu-id="869a8-141">Int32</span></span>|<span data-ttu-id="869a8-p107">页面的缩进级别。只读。</span><span class="sxs-lookup"><span data-stu-id="869a8-p107">The indentation level of the page. Read-only.</span></span>|
|<span data-ttu-id="869a8-144">links</span><span class="sxs-lookup"><span data-stu-id="869a8-144">links</span></span>|[<span data-ttu-id="869a8-145">PageLinks</span><span class="sxs-lookup"><span data-stu-id="869a8-145">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="869a8-p108">用于打开页面的链接。如果安装了 OneNote 本机客户端，则 `oneNoteClientURL` 链接将在其中打开页面。`oneNoteWebUrl` 链接将在 OneNote Online 中打开页面。只读。</span><span class="sxs-lookup"><span data-stu-id="869a8-p108">Links for opening the page. The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed. The `oneNoteWebUrl` link opens the page in OneNote Online. Read-only.</span></span>|
|<span data-ttu-id="869a8-150">order</span><span class="sxs-lookup"><span data-stu-id="869a8-150">order</span></span>|<span data-ttu-id="869a8-151">Int32</span><span class="sxs-lookup"><span data-stu-id="869a8-151">Int32</span></span>|<span data-ttu-id="869a8-p109">页面在其父分区中的顺序。只读。</span><span class="sxs-lookup"><span data-stu-id="869a8-p109">The order of the page within its parent section. Read-only.</span></span>|
|<span data-ttu-id="869a8-154">self</span><span class="sxs-lookup"><span data-stu-id="869a8-154">self</span></span>|<span data-ttu-id="869a8-155">字符串</span><span class="sxs-lookup"><span data-stu-id="869a8-155">String</span></span>|<span data-ttu-id="869a8-p110">可以在其中获取关于页面的详细信息的终结点。只读。</span><span class="sxs-lookup"><span data-stu-id="869a8-p110">The endpoint where you can get details about the page. Read-only.</span></span>|
|<span data-ttu-id="869a8-158">title</span><span class="sxs-lookup"><span data-stu-id="869a8-158">title</span></span>|<span data-ttu-id="869a8-159">String</span><span class="sxs-lookup"><span data-stu-id="869a8-159">String</span></span>|<span data-ttu-id="869a8-160">页面的标题。</span><span class="sxs-lookup"><span data-stu-id="869a8-160">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="869a8-161">关系</span><span class="sxs-lookup"><span data-stu-id="869a8-161">Relationships</span></span>
| <span data-ttu-id="869a8-162">关系</span><span class="sxs-lookup"><span data-stu-id="869a8-162">Relationship</span></span> | <span data-ttu-id="869a8-163">类型</span><span class="sxs-lookup"><span data-stu-id="869a8-163">Type</span></span>   |<span data-ttu-id="869a8-164">说明</span><span class="sxs-lookup"><span data-stu-id="869a8-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="869a8-165">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="869a8-165">parentNotebook</span></span>|[<span data-ttu-id="869a8-166">Notebook</span><span class="sxs-lookup"><span data-stu-id="869a8-166">Notebook</span></span>](notebook.md)|<span data-ttu-id="869a8-p111">包含页面的笔记本。只读。</span><span class="sxs-lookup"><span data-stu-id="869a8-p111">The notebook that contains the page.  Read-only.</span></span>|
|<span data-ttu-id="869a8-169">parentSection</span><span class="sxs-lookup"><span data-stu-id="869a8-169">parentSection</span></span>|[<span data-ttu-id="869a8-170">Section</span><span class="sxs-lookup"><span data-stu-id="869a8-170">Section</span></span>](section.md)|<span data-ttu-id="869a8-p112">包含页面的分区。只读。</span><span class="sxs-lookup"><span data-stu-id="869a8-p112">The section that contains the page. Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="869a8-173">方法</span><span class="sxs-lookup"><span data-stu-id="869a8-173">Methods</span></span>

| <span data-ttu-id="869a8-174">方法</span><span class="sxs-lookup"><span data-stu-id="869a8-174">Method</span></span>           | <span data-ttu-id="869a8-175">返回类型</span><span class="sxs-lookup"><span data-stu-id="869a8-175">Return Type</span></span>    |<span data-ttu-id="869a8-176">说明</span><span class="sxs-lookup"><span data-stu-id="869a8-176">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="869a8-177">Get page</span><span class="sxs-lookup"><span data-stu-id="869a8-177">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="869a8-178">Page</span><span class="sxs-lookup"><span data-stu-id="869a8-178">Page</span></span>](page.md) |<span data-ttu-id="869a8-179">读取页面的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="869a8-179">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="869a8-180">Update page content</span><span class="sxs-lookup"><span data-stu-id="869a8-180">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="869a8-181">无</span><span class="sxs-lookup"><span data-stu-id="869a8-181">None</span></span> |<span data-ttu-id="869a8-182">更新页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="869a8-182">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="869a8-183">Delete page</span><span class="sxs-lookup"><span data-stu-id="869a8-183">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="869a8-184">无</span><span class="sxs-lookup"><span data-stu-id="869a8-184">None</span></span> |<span data-ttu-id="869a8-185">删除页面。</span><span class="sxs-lookup"><span data-stu-id="869a8-185">Delete the page.</span></span> |
|[<span data-ttu-id="869a8-186">copyToSection</span><span class="sxs-lookup"><span data-stu-id="869a8-186">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="869a8-187">无</span><span class="sxs-lookup"><span data-stu-id="869a8-187">None</span></span> |<span data-ttu-id="869a8-188">将页面复制到特定分区。</span><span class="sxs-lookup"><span data-stu-id="869a8-188">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
