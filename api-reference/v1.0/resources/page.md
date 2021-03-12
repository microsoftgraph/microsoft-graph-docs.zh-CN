---
title: 页面资源类型
description: OneNote 笔记本中的页面。
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6adb0197b5e8fbcaa71e88f66481ca18a11bbfeb
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721528"
---
# <a name="page-resource-type"></a><span data-ttu-id="ce96d-103">页面资源类型</span><span class="sxs-lookup"><span data-stu-id="ce96d-103">page resource type</span></span>

<span data-ttu-id="ce96d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce96d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ce96d-105">OneNote 笔记本中的页面。</span><span class="sxs-lookup"><span data-stu-id="ce96d-105">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce96d-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ce96d-106">JSON representation</span></span>

<span data-ttu-id="ce96d-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce96d-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="ce96d-108">属性</span><span class="sxs-lookup"><span data-stu-id="ce96d-108">Properties</span></span>
| <span data-ttu-id="ce96d-109">属性</span><span class="sxs-lookup"><span data-stu-id="ce96d-109">Property</span></span>     | <span data-ttu-id="ce96d-110">类型</span><span class="sxs-lookup"><span data-stu-id="ce96d-110">Type</span></span>   |<span data-ttu-id="ce96d-111">说明</span><span class="sxs-lookup"><span data-stu-id="ce96d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce96d-112">content</span><span class="sxs-lookup"><span data-stu-id="ce96d-112">content</span></span>|<span data-ttu-id="ce96d-113">流</span><span class="sxs-lookup"><span data-stu-id="ce96d-113">Stream</span></span>|<span data-ttu-id="ce96d-114">页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="ce96d-114">The page's HTML content.</span></span>|
|<span data-ttu-id="ce96d-115">contentUrl</span><span class="sxs-lookup"><span data-stu-id="ce96d-115">contentUrl</span></span>|<span data-ttu-id="ce96d-116">字符串</span><span class="sxs-lookup"><span data-stu-id="ce96d-116">String</span></span>|<span data-ttu-id="ce96d-117">页面的 HTML 内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="ce96d-117">The URL for the page's HTML content.</span></span>  <span data-ttu-id="ce96d-118">只读。</span><span class="sxs-lookup"><span data-stu-id="ce96d-118">Read-only.</span></span>|
|<span data-ttu-id="ce96d-119">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="ce96d-119">createdByAppId</span></span>|<span data-ttu-id="ce96d-120">字符串</span><span class="sxs-lookup"><span data-stu-id="ce96d-120">String</span></span>|<span data-ttu-id="ce96d-121">创建页面的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ce96d-121">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="ce96d-122">只读。</span><span class="sxs-lookup"><span data-stu-id="ce96d-122">Read-only.</span></span>|
|<span data-ttu-id="ce96d-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce96d-123">createdDateTime</span></span>|<span data-ttu-id="ce96d-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce96d-124">DateTimeOffset</span></span>|<span data-ttu-id="ce96d-125">页面的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ce96d-125">The date and time when the page was created.</span></span> <span data-ttu-id="ce96d-126">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="ce96d-126">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ce96d-127">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="ce96d-127">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="ce96d-128">只读。</span><span class="sxs-lookup"><span data-stu-id="ce96d-128">Read-only.</span></span>|
|<span data-ttu-id="ce96d-129">id</span><span class="sxs-lookup"><span data-stu-id="ce96d-129">id</span></span>|<span data-ttu-id="ce96d-130">字符串</span><span class="sxs-lookup"><span data-stu-id="ce96d-130">String</span></span>|<span data-ttu-id="ce96d-131">页面的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ce96d-131">The unique identifier of the page.</span></span>  <span data-ttu-id="ce96d-132">只读。</span><span class="sxs-lookup"><span data-stu-id="ce96d-132">Read-only.</span></span>|
|<span data-ttu-id="ce96d-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce96d-133">lastModifiedDateTime</span></span>|<span data-ttu-id="ce96d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce96d-134">DateTimeOffset</span></span>|<span data-ttu-id="ce96d-135">上次修改页面的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ce96d-135">The date and time when the page was last modified.</span></span> <span data-ttu-id="ce96d-136">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="ce96d-136">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ce96d-137">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="ce96d-137">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="ce96d-138">只读。</span><span class="sxs-lookup"><span data-stu-id="ce96d-138">Read-only.</span></span>|
|<span data-ttu-id="ce96d-139">level</span><span class="sxs-lookup"><span data-stu-id="ce96d-139">level</span></span>|<span data-ttu-id="ce96d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ce96d-140">Int32</span></span>|<span data-ttu-id="ce96d-141">页面的缩进级别。</span><span class="sxs-lookup"><span data-stu-id="ce96d-141">The indentation level of the page.</span></span> <span data-ttu-id="ce96d-142">只读。</span><span class="sxs-lookup"><span data-stu-id="ce96d-142">Read-only.</span></span>|
|<span data-ttu-id="ce96d-143">links</span><span class="sxs-lookup"><span data-stu-id="ce96d-143">links</span></span>|[<span data-ttu-id="ce96d-144">PageLinks</span><span class="sxs-lookup"><span data-stu-id="ce96d-144">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="ce96d-145">用于打开页面的链接。</span><span class="sxs-lookup"><span data-stu-id="ce96d-145">Links for opening the page.</span></span> <span data-ttu-id="ce96d-146">如果 `oneNoteClientURL` 已安装，链接将在 OneNote 本机客户端中打开页面。</span><span class="sxs-lookup"><span data-stu-id="ce96d-146">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="ce96d-147">该 `oneNoteWebUrl` 链接在 OneNote 网页版中打开页面。</span><span class="sxs-lookup"><span data-stu-id="ce96d-147">The `oneNoteWebUrl` link opens the page in OneNote on the web.</span></span> <span data-ttu-id="ce96d-148">只读。</span><span class="sxs-lookup"><span data-stu-id="ce96d-148">Read-only.</span></span>|
|<span data-ttu-id="ce96d-149">order</span><span class="sxs-lookup"><span data-stu-id="ce96d-149">order</span></span>|<span data-ttu-id="ce96d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ce96d-150">Int32</span></span>|<span data-ttu-id="ce96d-151">页面在其父节中的顺序。</span><span class="sxs-lookup"><span data-stu-id="ce96d-151">The order of the page within its parent section.</span></span> <span data-ttu-id="ce96d-152">只读。</span><span class="sxs-lookup"><span data-stu-id="ce96d-152">Read-only.</span></span>|
|<span data-ttu-id="ce96d-153">self</span><span class="sxs-lookup"><span data-stu-id="ce96d-153">self</span></span>|<span data-ttu-id="ce96d-154">字符串</span><span class="sxs-lookup"><span data-stu-id="ce96d-154">String</span></span>|<span data-ttu-id="ce96d-155">可在其中获取页面详细信息的终结点。</span><span class="sxs-lookup"><span data-stu-id="ce96d-155">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="ce96d-156">只读。</span><span class="sxs-lookup"><span data-stu-id="ce96d-156">Read-only.</span></span>|
|<span data-ttu-id="ce96d-157">title</span><span class="sxs-lookup"><span data-stu-id="ce96d-157">title</span></span>|<span data-ttu-id="ce96d-158">String</span><span class="sxs-lookup"><span data-stu-id="ce96d-158">String</span></span>|<span data-ttu-id="ce96d-159">页面的标题。</span><span class="sxs-lookup"><span data-stu-id="ce96d-159">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ce96d-160">关系</span><span class="sxs-lookup"><span data-stu-id="ce96d-160">Relationships</span></span>
| <span data-ttu-id="ce96d-161">关系</span><span class="sxs-lookup"><span data-stu-id="ce96d-161">Relationship</span></span> | <span data-ttu-id="ce96d-162">类型</span><span class="sxs-lookup"><span data-stu-id="ce96d-162">Type</span></span>   |<span data-ttu-id="ce96d-163">说明</span><span class="sxs-lookup"><span data-stu-id="ce96d-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce96d-164">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="ce96d-164">parentNotebook</span></span>|[<span data-ttu-id="ce96d-165">笔记本</span><span class="sxs-lookup"><span data-stu-id="ce96d-165">Notebook</span></span>](notebook.md)|<span data-ttu-id="ce96d-166">包含页面的笔记本。</span><span class="sxs-lookup"><span data-stu-id="ce96d-166">The notebook that contains the page.</span></span>  <span data-ttu-id="ce96d-167">只读。</span><span class="sxs-lookup"><span data-stu-id="ce96d-167">Read-only.</span></span>|
|<span data-ttu-id="ce96d-168">parentSection</span><span class="sxs-lookup"><span data-stu-id="ce96d-168">parentSection</span></span>|[<span data-ttu-id="ce96d-169">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="ce96d-169">OnenoteSection</span></span>](section.md)|<span data-ttu-id="ce96d-170">包含页面的部分。</span><span class="sxs-lookup"><span data-stu-id="ce96d-170">The section that contains the page.</span></span> <span data-ttu-id="ce96d-171">只读的。</span><span class="sxs-lookup"><span data-stu-id="ce96d-171">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="ce96d-172">Methods</span><span class="sxs-lookup"><span data-stu-id="ce96d-172">Methods</span></span>

| <span data-ttu-id="ce96d-173">方法</span><span class="sxs-lookup"><span data-stu-id="ce96d-173">Method</span></span>           | <span data-ttu-id="ce96d-174">返回类型</span><span class="sxs-lookup"><span data-stu-id="ce96d-174">Return Type</span></span>    |<span data-ttu-id="ce96d-175">说明</span><span class="sxs-lookup"><span data-stu-id="ce96d-175">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ce96d-176">获取页面</span><span class="sxs-lookup"><span data-stu-id="ce96d-176">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="ce96d-177">Page</span><span class="sxs-lookup"><span data-stu-id="ce96d-177">Page</span></span>](page.md) |<span data-ttu-id="ce96d-178">读取页面的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ce96d-178">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="ce96d-179">更新页面内容</span><span class="sxs-lookup"><span data-stu-id="ce96d-179">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="ce96d-180">无</span><span class="sxs-lookup"><span data-stu-id="ce96d-180">None</span></span> |<span data-ttu-id="ce96d-181">更新页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="ce96d-181">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="ce96d-182">删除页面</span><span class="sxs-lookup"><span data-stu-id="ce96d-182">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="ce96d-183">无</span><span class="sxs-lookup"><span data-stu-id="ce96d-183">None</span></span> |<span data-ttu-id="ce96d-184">删除页面。</span><span class="sxs-lookup"><span data-stu-id="ce96d-184">Delete the page.</span></span> |
|[<span data-ttu-id="ce96d-185">copyToSection</span><span class="sxs-lookup"><span data-stu-id="ce96d-185">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="ce96d-186">无</span><span class="sxs-lookup"><span data-stu-id="ce96d-186">None</span></span> |<span data-ttu-id="ce96d-187">将页面复制到特定部分。</span><span class="sxs-lookup"><span data-stu-id="ce96d-187">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

