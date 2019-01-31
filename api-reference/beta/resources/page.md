---
title: 页面资源类型
description: OneNote 笔记本中的页面。
localization_priority: Normal
ms.openlocfilehash: d8c27cdc144e9b192bd0205f256653ff7f04df5f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649379"
---
# <a name="page-resource-type"></a><span data-ttu-id="7f197-103">页面资源类型</span><span class="sxs-lookup"><span data-stu-id="7f197-103">page resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f197-104">OneNote 笔记本中的页面。</span><span class="sxs-lookup"><span data-stu-id="7f197-104">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f197-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f197-105">JSON representation</span></span>

<span data-ttu-id="7f197-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f197-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="7f197-107">属性</span><span class="sxs-lookup"><span data-stu-id="7f197-107">Properties</span></span>
| <span data-ttu-id="7f197-108">属性</span><span class="sxs-lookup"><span data-stu-id="7f197-108">Property</span></span>     | <span data-ttu-id="7f197-109">类型</span><span class="sxs-lookup"><span data-stu-id="7f197-109">Type</span></span>   |<span data-ttu-id="7f197-110">说明</span><span class="sxs-lookup"><span data-stu-id="7f197-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f197-111">内容</span><span class="sxs-lookup"><span data-stu-id="7f197-111">content</span></span>|<span data-ttu-id="7f197-112">Stream</span><span class="sxs-lookup"><span data-stu-id="7f197-112">Stream</span></span>|<span data-ttu-id="7f197-113">页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="7f197-113">The page's HTML content.</span></span>|
|<span data-ttu-id="7f197-114">contentUrl</span><span class="sxs-lookup"><span data-stu-id="7f197-114">contentUrl</span></span>|<span data-ttu-id="7f197-115">String</span><span class="sxs-lookup"><span data-stu-id="7f197-115">String</span></span>|<span data-ttu-id="7f197-p101">页面的 HTML 内容的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="7f197-p101">The URL for the page's HTML content.  Read-only.</span></span>|
|<span data-ttu-id="7f197-118">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="7f197-118">createdByAppId</span></span>|<span data-ttu-id="7f197-119">String</span><span class="sxs-lookup"><span data-stu-id="7f197-119">String</span></span>|<span data-ttu-id="7f197-p102">创建页面的应用程序的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="7f197-p102">The unique identifier of the application that created the page. Read-only.</span></span>|
|<span data-ttu-id="7f197-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f197-122">createdDateTime</span></span>|<span data-ttu-id="7f197-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f197-123">DateTimeOffset</span></span>|<span data-ttu-id="7f197-p103">页面的创建日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="7f197-p103">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="7f197-128">id</span><span class="sxs-lookup"><span data-stu-id="7f197-128">id</span></span>|<span data-ttu-id="7f197-129">String</span><span class="sxs-lookup"><span data-stu-id="7f197-129">String</span></span>|<span data-ttu-id="7f197-p104">页面的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="7f197-p104">The unique identifier of the page.  Read-only.</span></span>|
|<span data-ttu-id="7f197-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f197-132">lastModifiedDateTime</span></span>|<span data-ttu-id="7f197-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f197-133">DateTimeOffset</span></span>|<span data-ttu-id="7f197-p105">上次修改页面的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="7f197-p105">The date and time when the page was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="7f197-138">level</span><span class="sxs-lookup"><span data-stu-id="7f197-138">level</span></span>|<span data-ttu-id="7f197-139">Int32</span><span class="sxs-lookup"><span data-stu-id="7f197-139">Int32</span></span>|<span data-ttu-id="7f197-p106">页面的缩进级别。只读。</span><span class="sxs-lookup"><span data-stu-id="7f197-p106">The indentation level of the page. Read-only.</span></span>|
|<span data-ttu-id="7f197-142">links</span><span class="sxs-lookup"><span data-stu-id="7f197-142">links</span></span>|[<span data-ttu-id="7f197-143">PageLinks</span><span class="sxs-lookup"><span data-stu-id="7f197-143">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="7f197-p107">用于打开页面的链接。如果安装了 OneNote 本机客户端，则 `oneNoteClientURL` 链接将在其中打开页面。`oneNoteWebUrl` 链接将在 OneNote Online 中打开页面。只读。</span><span class="sxs-lookup"><span data-stu-id="7f197-p107">Links for opening the page. The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed. The `oneNoteWebUrl` link opens the page in OneNote Online. Read-only.</span></span>|
|<span data-ttu-id="7f197-148">order</span><span class="sxs-lookup"><span data-stu-id="7f197-148">order</span></span>|<span data-ttu-id="7f197-149">Int32</span><span class="sxs-lookup"><span data-stu-id="7f197-149">Int32</span></span>|<span data-ttu-id="7f197-p108">页面在其父分区中的顺序。只读。</span><span class="sxs-lookup"><span data-stu-id="7f197-p108">The order of the page within its parent section. Read-only.</span></span>|
|<span data-ttu-id="7f197-152">self</span><span class="sxs-lookup"><span data-stu-id="7f197-152">self</span></span>|<span data-ttu-id="7f197-153">String</span><span class="sxs-lookup"><span data-stu-id="7f197-153">String</span></span>|<span data-ttu-id="7f197-p109">可以在其中获取关于页面的详细信息的终结点。只读。</span><span class="sxs-lookup"><span data-stu-id="7f197-p109">The endpoint where you can get details about the page. Read-only.</span></span>|
|<span data-ttu-id="7f197-156">title</span><span class="sxs-lookup"><span data-stu-id="7f197-156">title</span></span>|<span data-ttu-id="7f197-157">String</span><span class="sxs-lookup"><span data-stu-id="7f197-157">String</span></span>|<span data-ttu-id="7f197-158">页面的标题。</span><span class="sxs-lookup"><span data-stu-id="7f197-158">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7f197-159">关系</span><span class="sxs-lookup"><span data-stu-id="7f197-159">Relationships</span></span>
| <span data-ttu-id="7f197-160">关系</span><span class="sxs-lookup"><span data-stu-id="7f197-160">Relationship</span></span> | <span data-ttu-id="7f197-161">类型</span><span class="sxs-lookup"><span data-stu-id="7f197-161">Type</span></span>   |<span data-ttu-id="7f197-162">说明</span><span class="sxs-lookup"><span data-stu-id="7f197-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f197-163">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="7f197-163">parentNotebook</span></span>|[<span data-ttu-id="7f197-164">Notebook</span><span class="sxs-lookup"><span data-stu-id="7f197-164">Notebook</span></span>](notebook.md)|<span data-ttu-id="7f197-p110">包含页面的笔记本。只读。</span><span class="sxs-lookup"><span data-stu-id="7f197-p110">The notebook that contains the page.  Read-only.</span></span>|
|<span data-ttu-id="7f197-167">parentSection</span><span class="sxs-lookup"><span data-stu-id="7f197-167">parentSection</span></span>|[<span data-ttu-id="7f197-168">Section</span><span class="sxs-lookup"><span data-stu-id="7f197-168">Section</span></span>](section.md)|<span data-ttu-id="7f197-p111">包含页面的分区。只读。</span><span class="sxs-lookup"><span data-stu-id="7f197-p111">The section that contains the page. Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="7f197-171">方法</span><span class="sxs-lookup"><span data-stu-id="7f197-171">Methods</span></span>

| <span data-ttu-id="7f197-172">方法</span><span class="sxs-lookup"><span data-stu-id="7f197-172">Method</span></span>           | <span data-ttu-id="7f197-173">返回类型</span><span class="sxs-lookup"><span data-stu-id="7f197-173">Return Type</span></span>    |<span data-ttu-id="7f197-174">说明</span><span class="sxs-lookup"><span data-stu-id="7f197-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7f197-175">Get page</span><span class="sxs-lookup"><span data-stu-id="7f197-175">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="7f197-176">Page</span><span class="sxs-lookup"><span data-stu-id="7f197-176">Page</span></span>](page.md) |<span data-ttu-id="7f197-177">读取页面的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7f197-177">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="7f197-178">Update page content</span><span class="sxs-lookup"><span data-stu-id="7f197-178">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="7f197-179">无</span><span class="sxs-lookup"><span data-stu-id="7f197-179">None</span></span> |<span data-ttu-id="7f197-180">更新页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="7f197-180">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="7f197-181">Delete page</span><span class="sxs-lookup"><span data-stu-id="7f197-181">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="7f197-182">无</span><span class="sxs-lookup"><span data-stu-id="7f197-182">None</span></span> |<span data-ttu-id="7f197-183">删除页面。</span><span class="sxs-lookup"><span data-stu-id="7f197-183">Delete the page.</span></span> |
|[<span data-ttu-id="7f197-184">copyToSection</span><span class="sxs-lookup"><span data-stu-id="7f197-184">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="7f197-185">无</span><span class="sxs-lookup"><span data-stu-id="7f197-185">None</span></span> |<span data-ttu-id="7f197-186">将页面复制到特定分区。</span><span class="sxs-lookup"><span data-stu-id="7f197-186">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/page.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
