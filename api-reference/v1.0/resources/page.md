---
title: 页面资源类型
description: OneNote 笔记本中的页面。
localization_priority: Normal
ms.openlocfilehash: b7c92aaae401e022a79f7c3b72cb15b3093d0b7d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462548"
---
# <a name="page-resource-type"></a><span data-ttu-id="30d9e-103">页面资源类型</span><span class="sxs-lookup"><span data-stu-id="30d9e-103">page resource type</span></span>

<span data-ttu-id="30d9e-104">OneNote 笔记本中的页面。</span><span class="sxs-lookup"><span data-stu-id="30d9e-104">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="30d9e-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30d9e-105">JSON representation</span></span>

<span data-ttu-id="30d9e-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30d9e-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="30d9e-107">属性</span><span class="sxs-lookup"><span data-stu-id="30d9e-107">Properties</span></span>
| <span data-ttu-id="30d9e-108">属性</span><span class="sxs-lookup"><span data-stu-id="30d9e-108">Property</span></span>     | <span data-ttu-id="30d9e-109">类型</span><span class="sxs-lookup"><span data-stu-id="30d9e-109">Type</span></span>   |<span data-ttu-id="30d9e-110">说明</span><span class="sxs-lookup"><span data-stu-id="30d9e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30d9e-111">content</span><span class="sxs-lookup"><span data-stu-id="30d9e-111">content</span></span>|<span data-ttu-id="30d9e-112">流</span><span class="sxs-lookup"><span data-stu-id="30d9e-112">Stream</span></span>|<span data-ttu-id="30d9e-113">页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="30d9e-113">The page's HTML content.</span></span>|
|<span data-ttu-id="30d9e-114">contentUrl</span><span class="sxs-lookup"><span data-stu-id="30d9e-114">contentUrl</span></span>|<span data-ttu-id="30d9e-115">字符串</span><span class="sxs-lookup"><span data-stu-id="30d9e-115">String</span></span>|<span data-ttu-id="30d9e-116">页面的 HTML 内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="30d9e-116">The URL for the page's HTML content.</span></span>  <span data-ttu-id="30d9e-117">只读。</span><span class="sxs-lookup"><span data-stu-id="30d9e-117">Read-only.</span></span>|
|<span data-ttu-id="30d9e-118">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="30d9e-118">createdByAppId</span></span>|<span data-ttu-id="30d9e-119">字符串</span><span class="sxs-lookup"><span data-stu-id="30d9e-119">String</span></span>|<span data-ttu-id="30d9e-120">创建页面的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="30d9e-120">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="30d9e-121">只读。</span><span class="sxs-lookup"><span data-stu-id="30d9e-121">Read-only.</span></span>|
|<span data-ttu-id="30d9e-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30d9e-122">createdDateTime</span></span>|<span data-ttu-id="30d9e-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30d9e-123">DateTimeOffset</span></span>|<span data-ttu-id="30d9e-124">页面的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="30d9e-124">The date and time when the page was created.</span></span> <span data-ttu-id="30d9e-125">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="30d9e-125">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="30d9e-126">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="30d9e-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="30d9e-127">只读。</span><span class="sxs-lookup"><span data-stu-id="30d9e-127">Read-only.</span></span>|
|<span data-ttu-id="30d9e-128">id</span><span class="sxs-lookup"><span data-stu-id="30d9e-128">id</span></span>|<span data-ttu-id="30d9e-129">String</span><span class="sxs-lookup"><span data-stu-id="30d9e-129">String</span></span>|<span data-ttu-id="30d9e-130">页面的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="30d9e-130">The unique identifier of the page.</span></span>  <span data-ttu-id="30d9e-131">只读。</span><span class="sxs-lookup"><span data-stu-id="30d9e-131">Read-only.</span></span>|
|<span data-ttu-id="30d9e-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30d9e-132">lastModifiedDateTime</span></span>|<span data-ttu-id="30d9e-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30d9e-133">DateTimeOffset</span></span>|<span data-ttu-id="30d9e-134">上次修改页面的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="30d9e-134">The date and time when the page was last modified.</span></span> <span data-ttu-id="30d9e-135">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="30d9e-135">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="30d9e-136">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="30d9e-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="30d9e-137">只读。</span><span class="sxs-lookup"><span data-stu-id="30d9e-137">Read-only.</span></span>|
|<span data-ttu-id="30d9e-138">level</span><span class="sxs-lookup"><span data-stu-id="30d9e-138">level</span></span>|<span data-ttu-id="30d9e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="30d9e-139">Int32</span></span>|<span data-ttu-id="30d9e-140">页面的缩进级别。</span><span class="sxs-lookup"><span data-stu-id="30d9e-140">The indentation level of the page.</span></span> <span data-ttu-id="30d9e-141">只读。</span><span class="sxs-lookup"><span data-stu-id="30d9e-141">Read-only.</span></span>|
|<span data-ttu-id="30d9e-142">links</span><span class="sxs-lookup"><span data-stu-id="30d9e-142">links</span></span>|[<span data-ttu-id="30d9e-143">PageLinks</span><span class="sxs-lookup"><span data-stu-id="30d9e-143">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="30d9e-144">用于打开页面的链接。</span><span class="sxs-lookup"><span data-stu-id="30d9e-144">Links for opening the page.</span></span> <span data-ttu-id="30d9e-145">如果`oneNoteClientURL`安装了 OneNote 本机客户端, 则链接将在其中打开页面。</span><span class="sxs-lookup"><span data-stu-id="30d9e-145">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="30d9e-146">`oneNoteWebUrl`链接将在 OneNote Online 中打开页面。</span><span class="sxs-lookup"><span data-stu-id="30d9e-146">The `oneNoteWebUrl` link opens the page in OneNote Online.</span></span> <span data-ttu-id="30d9e-147">只读。</span><span class="sxs-lookup"><span data-stu-id="30d9e-147">Read-only.</span></span>|
|<span data-ttu-id="30d9e-148">顺序</span><span class="sxs-lookup"><span data-stu-id="30d9e-148">order</span></span>|<span data-ttu-id="30d9e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="30d9e-149">Int32</span></span>|<span data-ttu-id="30d9e-150">页面在其父节中的顺序。</span><span class="sxs-lookup"><span data-stu-id="30d9e-150">The order of the page within its parent section.</span></span> <span data-ttu-id="30d9e-151">只读。</span><span class="sxs-lookup"><span data-stu-id="30d9e-151">Read-only.</span></span>|
|<span data-ttu-id="30d9e-152">自学</span><span class="sxs-lookup"><span data-stu-id="30d9e-152">self</span></span>|<span data-ttu-id="30d9e-153">字符串</span><span class="sxs-lookup"><span data-stu-id="30d9e-153">String</span></span>|<span data-ttu-id="30d9e-154">可在其中获取有关页面的详细信息的终结点。</span><span class="sxs-lookup"><span data-stu-id="30d9e-154">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="30d9e-155">只读。</span><span class="sxs-lookup"><span data-stu-id="30d9e-155">Read-only.</span></span>|
|<span data-ttu-id="30d9e-156">title</span><span class="sxs-lookup"><span data-stu-id="30d9e-156">title</span></span>|<span data-ttu-id="30d9e-157">String</span><span class="sxs-lookup"><span data-stu-id="30d9e-157">String</span></span>|<span data-ttu-id="30d9e-158">页面的标题。</span><span class="sxs-lookup"><span data-stu-id="30d9e-158">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="30d9e-159">关系</span><span class="sxs-lookup"><span data-stu-id="30d9e-159">Relationships</span></span>
| <span data-ttu-id="30d9e-160">关系</span><span class="sxs-lookup"><span data-stu-id="30d9e-160">Relationship</span></span> | <span data-ttu-id="30d9e-161">类型</span><span class="sxs-lookup"><span data-stu-id="30d9e-161">Type</span></span>   |<span data-ttu-id="30d9e-162">说明</span><span class="sxs-lookup"><span data-stu-id="30d9e-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30d9e-163">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="30d9e-163">parentNotebook</span></span>|[<span data-ttu-id="30d9e-164">Notebook</span><span class="sxs-lookup"><span data-stu-id="30d9e-164">Notebook</span></span>](notebook.md)|<span data-ttu-id="30d9e-165">包含页面的笔记本。</span><span class="sxs-lookup"><span data-stu-id="30d9e-165">The notebook that contains the page.</span></span>  <span data-ttu-id="30d9e-166">只读。</span><span class="sxs-lookup"><span data-stu-id="30d9e-166">Read-only.</span></span>|
|<span data-ttu-id="30d9e-167">parentSection</span><span class="sxs-lookup"><span data-stu-id="30d9e-167">parentSection</span></span>|[<span data-ttu-id="30d9e-168">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="30d9e-168">OnenoteSection</span></span>](section.md)|<span data-ttu-id="30d9e-169">包含页面的部分。</span><span class="sxs-lookup"><span data-stu-id="30d9e-169">The section that contains the page.</span></span> <span data-ttu-id="30d9e-170">只读的。</span><span class="sxs-lookup"><span data-stu-id="30d9e-170">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="30d9e-171">方法</span><span class="sxs-lookup"><span data-stu-id="30d9e-171">Methods</span></span>

| <span data-ttu-id="30d9e-172">方法</span><span class="sxs-lookup"><span data-stu-id="30d9e-172">Method</span></span>           | <span data-ttu-id="30d9e-173">返回类型</span><span class="sxs-lookup"><span data-stu-id="30d9e-173">Return Type</span></span>    |<span data-ttu-id="30d9e-174">说明</span><span class="sxs-lookup"><span data-stu-id="30d9e-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="30d9e-175">获取页面</span><span class="sxs-lookup"><span data-stu-id="30d9e-175">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="30d9e-176">Page</span><span class="sxs-lookup"><span data-stu-id="30d9e-176">Page</span></span>](page.md) |<span data-ttu-id="30d9e-177">读取页面的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="30d9e-177">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="30d9e-178">更新页面内容</span><span class="sxs-lookup"><span data-stu-id="30d9e-178">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="30d9e-179">无</span><span class="sxs-lookup"><span data-stu-id="30d9e-179">None</span></span> |<span data-ttu-id="30d9e-180">更新页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="30d9e-180">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="30d9e-181">删除页面</span><span class="sxs-lookup"><span data-stu-id="30d9e-181">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="30d9e-182">无</span><span class="sxs-lookup"><span data-stu-id="30d9e-182">None</span></span> |<span data-ttu-id="30d9e-183">删除页面。</span><span class="sxs-lookup"><span data-stu-id="30d9e-183">Delete the page.</span></span> |
|[<span data-ttu-id="30d9e-184">copyToSection</span><span class="sxs-lookup"><span data-stu-id="30d9e-184">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="30d9e-185">无</span><span class="sxs-lookup"><span data-stu-id="30d9e-185">None</span></span> |<span data-ttu-id="30d9e-186">将页面复制到特定分区。</span><span class="sxs-lookup"><span data-stu-id="30d9e-186">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
