# <a name="page-resource-type"></a><span data-ttu-id="0c723-101">页面资源类型</span><span class="sxs-lookup"><span data-stu-id="0c723-101">page resource type</span></span>

<span data-ttu-id="0c723-102">OneNote 笔记本中的页面。</span><span class="sxs-lookup"><span data-stu-id="0c723-102">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c723-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c723-103">JSON representation</span></span>

<span data-ttu-id="0c723-104">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c723-104">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="0c723-105">属性</span><span class="sxs-lookup"><span data-stu-id="0c723-105">Properties</span></span>
| <span data-ttu-id="0c723-106">属性</span><span class="sxs-lookup"><span data-stu-id="0c723-106">Property</span></span>     | <span data-ttu-id="0c723-107">类型</span><span class="sxs-lookup"><span data-stu-id="0c723-107">Type</span></span>   |<span data-ttu-id="0c723-108">说明</span><span class="sxs-lookup"><span data-stu-id="0c723-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c723-109">内容</span><span class="sxs-lookup"><span data-stu-id="0c723-109">content</span></span>|<span data-ttu-id="0c723-110">Stream</span><span class="sxs-lookup"><span data-stu-id="0c723-110">Stream</span></span>|<span data-ttu-id="0c723-111">页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="0c723-111">The page's HTML content.</span></span>|
|<span data-ttu-id="0c723-112">contentUrl</span><span class="sxs-lookup"><span data-stu-id="0c723-112">contentUrl</span></span>|<span data-ttu-id="0c723-113">字符串</span><span class="sxs-lookup"><span data-stu-id="0c723-113">String</span></span>|<span data-ttu-id="0c723-p101">页面的 HTML 内容的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="0c723-p101">The URL for the page's HTML content.  Read-only.</span></span>|
|<span data-ttu-id="0c723-116">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="0c723-116">createdByAppId</span></span>|<span data-ttu-id="0c723-117">字符串</span><span class="sxs-lookup"><span data-stu-id="0c723-117">String</span></span>|<span data-ttu-id="0c723-p102">创建页面的应用程序的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="0c723-p102">The unique identifier of the application that created the page. Read-only.</span></span>|
|<span data-ttu-id="0c723-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c723-120">createdDateTime</span></span>|<span data-ttu-id="0c723-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c723-121">DateTimeOffset</span></span>|<span data-ttu-id="0c723-p103">页面的创建日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="0c723-p103">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="0c723-126">id</span><span class="sxs-lookup"><span data-stu-id="0c723-126">id</span></span>|<span data-ttu-id="0c723-127">字符串</span><span class="sxs-lookup"><span data-stu-id="0c723-127">String</span></span>|<span data-ttu-id="0c723-p104">页面的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="0c723-p104">The unique identifier of the page.  Read-only.</span></span>|
|<span data-ttu-id="0c723-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c723-130">lastModifiedDateTime</span></span>|<span data-ttu-id="0c723-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c723-131">DateTimeOffset</span></span>|<span data-ttu-id="0c723-p105">上次修改页面的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="0c723-p105">The date and time when the page was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="0c723-136">level</span><span class="sxs-lookup"><span data-stu-id="0c723-136">level</span></span>|<span data-ttu-id="0c723-137">Int32</span><span class="sxs-lookup"><span data-stu-id="0c723-137">Int32</span></span>|<span data-ttu-id="0c723-p106">页面的缩进级别。只读。</span><span class="sxs-lookup"><span data-stu-id="0c723-p106">The indentation level of the page. Read-only.</span></span>|
|<span data-ttu-id="0c723-140">links</span><span class="sxs-lookup"><span data-stu-id="0c723-140">links</span></span>|[<span data-ttu-id="0c723-141">PageLinks</span><span class="sxs-lookup"><span data-stu-id="0c723-141">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="0c723-p107">用于打开页面的链接。如果安装了 OneNote 本机客户端，则 `oneNoteClientURL` 链接将在其中打开页面。`oneNoteWebUrl` 链接将在 OneNote Online 中打开页面。只读。</span><span class="sxs-lookup"><span data-stu-id="0c723-p107">Links for opening the page. The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed. The `oneNoteWebUrl` link opens the page in OneNote Online. Read-only.</span></span>|
|<span data-ttu-id="0c723-146">order</span><span class="sxs-lookup"><span data-stu-id="0c723-146">order</span></span>|<span data-ttu-id="0c723-147">Int32</span><span class="sxs-lookup"><span data-stu-id="0c723-147">Int32</span></span>|<span data-ttu-id="0c723-p108">页面在其父分区中的顺序。只读。</span><span class="sxs-lookup"><span data-stu-id="0c723-p108">The order of the page within its parent section. Read-only.</span></span>|
|<span data-ttu-id="0c723-150">self</span><span class="sxs-lookup"><span data-stu-id="0c723-150">self</span></span>|<span data-ttu-id="0c723-151">字符串</span><span class="sxs-lookup"><span data-stu-id="0c723-151">String</span></span>|<span data-ttu-id="0c723-p109">可以在其中获取关于页面的详细信息的终结点。只读。</span><span class="sxs-lookup"><span data-stu-id="0c723-p109">The endpoint where you can get details about the page. Read-only.</span></span>|
|<span data-ttu-id="0c723-154">title</span><span class="sxs-lookup"><span data-stu-id="0c723-154">title</span></span>|<span data-ttu-id="0c723-155">String</span><span class="sxs-lookup"><span data-stu-id="0c723-155">String</span></span>|<span data-ttu-id="0c723-156">页面的标题。</span><span class="sxs-lookup"><span data-stu-id="0c723-156">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0c723-157">关系</span><span class="sxs-lookup"><span data-stu-id="0c723-157">Relationships</span></span>
| <span data-ttu-id="0c723-158">关系</span><span class="sxs-lookup"><span data-stu-id="0c723-158">Relationship</span></span> | <span data-ttu-id="0c723-159">类型</span><span class="sxs-lookup"><span data-stu-id="0c723-159">Type</span></span>   |<span data-ttu-id="0c723-160">说明</span><span class="sxs-lookup"><span data-stu-id="0c723-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c723-161">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="0c723-161">parentNotebook</span></span>|[<span data-ttu-id="0c723-162">Notebook</span><span class="sxs-lookup"><span data-stu-id="0c723-162">Notebook</span></span>](notebook.md)|<span data-ttu-id="0c723-p110">包含页面的笔记本。只读。</span><span class="sxs-lookup"><span data-stu-id="0c723-p110">The notebook that contains the page.  Read-only.</span></span>|
|<span data-ttu-id="0c723-165">parentSection</span><span class="sxs-lookup"><span data-stu-id="0c723-165">parentSection</span></span>|[<span data-ttu-id="0c723-166">Section</span><span class="sxs-lookup"><span data-stu-id="0c723-166">Section</span></span>](section.md)|<span data-ttu-id="0c723-p111">包含页面的分区。只读。</span><span class="sxs-lookup"><span data-stu-id="0c723-p111">The section that contains the page. Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="0c723-169">方法</span><span class="sxs-lookup"><span data-stu-id="0c723-169">Methods</span></span>

| <span data-ttu-id="0c723-170">方法</span><span class="sxs-lookup"><span data-stu-id="0c723-170">Method</span></span>           | <span data-ttu-id="0c723-171">返回类型</span><span class="sxs-lookup"><span data-stu-id="0c723-171">Return Type</span></span>    |<span data-ttu-id="0c723-172">说明</span><span class="sxs-lookup"><span data-stu-id="0c723-172">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0c723-173">Get page</span><span class="sxs-lookup"><span data-stu-id="0c723-173">Get page</span></span>](../api/page_get.md) | [<span data-ttu-id="0c723-174">Page</span><span class="sxs-lookup"><span data-stu-id="0c723-174">Page</span></span>](page.md) |<span data-ttu-id="0c723-175">读取页面的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0c723-175">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="0c723-176">Update page content</span><span class="sxs-lookup"><span data-stu-id="0c723-176">Update page content</span></span>](../api/page_update.md) | <span data-ttu-id="0c723-177">无</span><span class="sxs-lookup"><span data-stu-id="0c723-177">None</span></span> |<span data-ttu-id="0c723-178">更新页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="0c723-178">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="0c723-179">Delete page</span><span class="sxs-lookup"><span data-stu-id="0c723-179">Delete page</span></span>](../api/page_delete.md) | <span data-ttu-id="0c723-180">无</span><span class="sxs-lookup"><span data-stu-id="0c723-180">None</span></span> |<span data-ttu-id="0c723-181">删除页面。</span><span class="sxs-lookup"><span data-stu-id="0c723-181">Delete the page.</span></span> |
|[<span data-ttu-id="0c723-182">copyToSection</span><span class="sxs-lookup"><span data-stu-id="0c723-182">copyToSection</span></span>](../api/page_copytosection.md)| <span data-ttu-id="0c723-183">无</span><span class="sxs-lookup"><span data-stu-id="0c723-183">None</span></span> |<span data-ttu-id="0c723-184">将页面复制到特定分区。</span><span class="sxs-lookup"><span data-stu-id="0c723-184">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->