---
title: 页面资源类型
description: OneNote 笔记本中的页面。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 69066585c575569da7b355a6c52263843510dcc3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447239"
---
# <a name="page-resource-type"></a><span data-ttu-id="0b076-103">页面资源类型</span><span class="sxs-lookup"><span data-stu-id="0b076-103">page resource type</span></span>

<span data-ttu-id="0b076-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0b076-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b076-105">OneNote 笔记本中的页面。</span><span class="sxs-lookup"><span data-stu-id="0b076-105">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b076-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b076-106">JSON representation</span></span>

<span data-ttu-id="0b076-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b076-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="0b076-108">属性</span><span class="sxs-lookup"><span data-stu-id="0b076-108">Properties</span></span>
| <span data-ttu-id="0b076-109">属性</span><span class="sxs-lookup"><span data-stu-id="0b076-109">Property</span></span>     | <span data-ttu-id="0b076-110">类型</span><span class="sxs-lookup"><span data-stu-id="0b076-110">Type</span></span>   |<span data-ttu-id="0b076-111">说明</span><span class="sxs-lookup"><span data-stu-id="0b076-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b076-112">content</span><span class="sxs-lookup"><span data-stu-id="0b076-112">content</span></span>|<span data-ttu-id="0b076-113">流</span><span class="sxs-lookup"><span data-stu-id="0b076-113">Stream</span></span>|<span data-ttu-id="0b076-114">页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="0b076-114">The page's HTML content.</span></span>|
|<span data-ttu-id="0b076-115">contentUrl</span><span class="sxs-lookup"><span data-stu-id="0b076-115">contentUrl</span></span>|<span data-ttu-id="0b076-116">String</span><span class="sxs-lookup"><span data-stu-id="0b076-116">String</span></span>|<span data-ttu-id="0b076-117">页面的 HTML 内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="0b076-117">The URL for the page's HTML content.</span></span>  <span data-ttu-id="0b076-118">只读。</span><span class="sxs-lookup"><span data-stu-id="0b076-118">Read-only.</span></span>|
|<span data-ttu-id="0b076-119">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="0b076-119">createdByAppId</span></span>|<span data-ttu-id="0b076-120">String</span><span class="sxs-lookup"><span data-stu-id="0b076-120">String</span></span>|<span data-ttu-id="0b076-121">创建页面的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0b076-121">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="0b076-122">只读。</span><span class="sxs-lookup"><span data-stu-id="0b076-122">Read-only.</span></span>|
|<span data-ttu-id="0b076-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b076-123">createdDateTime</span></span>|<span data-ttu-id="0b076-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b076-124">DateTimeOffset</span></span>|<span data-ttu-id="0b076-125">页面的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0b076-125">The date and time when the page was created.</span></span> <span data-ttu-id="0b076-126">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="0b076-126">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0b076-127">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="0b076-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0b076-128">只读。</span><span class="sxs-lookup"><span data-stu-id="0b076-128">Read-only.</span></span>|
|<span data-ttu-id="0b076-129">id</span><span class="sxs-lookup"><span data-stu-id="0b076-129">id</span></span>|<span data-ttu-id="0b076-130">字符串</span><span class="sxs-lookup"><span data-stu-id="0b076-130">String</span></span>|<span data-ttu-id="0b076-131">页面的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0b076-131">The unique identifier of the page.</span></span>  <span data-ttu-id="0b076-132">只读。</span><span class="sxs-lookup"><span data-stu-id="0b076-132">Read-only.</span></span>|
|<span data-ttu-id="0b076-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b076-133">lastModifiedDateTime</span></span>|<span data-ttu-id="0b076-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b076-134">DateTimeOffset</span></span>|<span data-ttu-id="0b076-135">上次修改页面的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0b076-135">The date and time when the page was last modified.</span></span> <span data-ttu-id="0b076-136">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="0b076-136">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0b076-137">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="0b076-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0b076-138">只读。</span><span class="sxs-lookup"><span data-stu-id="0b076-138">Read-only.</span></span>|
|<span data-ttu-id="0b076-139">块级</span><span class="sxs-lookup"><span data-stu-id="0b076-139">level</span></span>|<span data-ttu-id="0b076-140">Int32</span><span class="sxs-lookup"><span data-stu-id="0b076-140">Int32</span></span>|<span data-ttu-id="0b076-141">页面的缩进级别。</span><span class="sxs-lookup"><span data-stu-id="0b076-141">The indentation level of the page.</span></span> <span data-ttu-id="0b076-142">只读。</span><span class="sxs-lookup"><span data-stu-id="0b076-142">Read-only.</span></span>|
|<span data-ttu-id="0b076-143">links</span><span class="sxs-lookup"><span data-stu-id="0b076-143">links</span></span>|[<span data-ttu-id="0b076-144">PageLinks</span><span class="sxs-lookup"><span data-stu-id="0b076-144">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="0b076-145">用于打开页面的链接。</span><span class="sxs-lookup"><span data-stu-id="0b076-145">Links for opening the page.</span></span> <span data-ttu-id="0b076-146">如果`oneNoteClientURL`安装了 OneNote 本机客户端，则链接将在其中打开页面。</span><span class="sxs-lookup"><span data-stu-id="0b076-146">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="0b076-147">`oneNoteWebUrl`链接将在 web 上的 OneNote 中打开页面。</span><span class="sxs-lookup"><span data-stu-id="0b076-147">The `oneNoteWebUrl` link opens the page in OneNote on the web.</span></span> <span data-ttu-id="0b076-148">只读。</span><span class="sxs-lookup"><span data-stu-id="0b076-148">Read-only.</span></span>|
|<span data-ttu-id="0b076-149">顺序</span><span class="sxs-lookup"><span data-stu-id="0b076-149">order</span></span>|<span data-ttu-id="0b076-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0b076-150">Int32</span></span>|<span data-ttu-id="0b076-151">页面在其父节中的顺序。</span><span class="sxs-lookup"><span data-stu-id="0b076-151">The order of the page within its parent section.</span></span> <span data-ttu-id="0b076-152">只读。</span><span class="sxs-lookup"><span data-stu-id="0b076-152">Read-only.</span></span>|
|<span data-ttu-id="0b076-153">自学</span><span class="sxs-lookup"><span data-stu-id="0b076-153">self</span></span>|<span data-ttu-id="0b076-154">String</span><span class="sxs-lookup"><span data-stu-id="0b076-154">String</span></span>|<span data-ttu-id="0b076-155">可在其中获取有关页面的详细信息的终结点。</span><span class="sxs-lookup"><span data-stu-id="0b076-155">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="0b076-156">只读。</span><span class="sxs-lookup"><span data-stu-id="0b076-156">Read-only.</span></span>|
|<span data-ttu-id="0b076-157">title</span><span class="sxs-lookup"><span data-stu-id="0b076-157">title</span></span>|<span data-ttu-id="0b076-158">String</span><span class="sxs-lookup"><span data-stu-id="0b076-158">String</span></span>|<span data-ttu-id="0b076-159">页面的标题。</span><span class="sxs-lookup"><span data-stu-id="0b076-159">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0b076-160">关系</span><span class="sxs-lookup"><span data-stu-id="0b076-160">Relationships</span></span>
| <span data-ttu-id="0b076-161">关系</span><span class="sxs-lookup"><span data-stu-id="0b076-161">Relationship</span></span> | <span data-ttu-id="0b076-162">类型</span><span class="sxs-lookup"><span data-stu-id="0b076-162">Type</span></span>   |<span data-ttu-id="0b076-163">说明</span><span class="sxs-lookup"><span data-stu-id="0b076-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b076-164">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="0b076-164">parentNotebook</span></span>|[<span data-ttu-id="0b076-165">笔记本</span><span class="sxs-lookup"><span data-stu-id="0b076-165">Notebook</span></span>](notebook.md)|<span data-ttu-id="0b076-166">包含页面的笔记本。</span><span class="sxs-lookup"><span data-stu-id="0b076-166">The notebook that contains the page.</span></span>  <span data-ttu-id="0b076-167">只读。</span><span class="sxs-lookup"><span data-stu-id="0b076-167">Read-only.</span></span>|
|<span data-ttu-id="0b076-168">parentSection</span><span class="sxs-lookup"><span data-stu-id="0b076-168">parentSection</span></span>|[<span data-ttu-id="0b076-169">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="0b076-169">OnenoteSection</span></span>](section.md)|<span data-ttu-id="0b076-170">包含页面的部分。</span><span class="sxs-lookup"><span data-stu-id="0b076-170">The section that contains the page.</span></span> <span data-ttu-id="0b076-171">只读的。</span><span class="sxs-lookup"><span data-stu-id="0b076-171">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="0b076-172">方法</span><span class="sxs-lookup"><span data-stu-id="0b076-172">Methods</span></span>

| <span data-ttu-id="0b076-173">方法</span><span class="sxs-lookup"><span data-stu-id="0b076-173">Method</span></span>           | <span data-ttu-id="0b076-174">返回类型</span><span class="sxs-lookup"><span data-stu-id="0b076-174">Return Type</span></span>    |<span data-ttu-id="0b076-175">说明</span><span class="sxs-lookup"><span data-stu-id="0b076-175">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0b076-176">获取页面</span><span class="sxs-lookup"><span data-stu-id="0b076-176">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="0b076-177">Page</span><span class="sxs-lookup"><span data-stu-id="0b076-177">Page</span></span>](page.md) |<span data-ttu-id="0b076-178">读取页面的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0b076-178">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="0b076-179">更新页面内容</span><span class="sxs-lookup"><span data-stu-id="0b076-179">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="0b076-180">无</span><span class="sxs-lookup"><span data-stu-id="0b076-180">None</span></span> |<span data-ttu-id="0b076-181">更新页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="0b076-181">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="0b076-182">删除页面</span><span class="sxs-lookup"><span data-stu-id="0b076-182">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="0b076-183">无</span><span class="sxs-lookup"><span data-stu-id="0b076-183">None</span></span> |<span data-ttu-id="0b076-184">删除页面。</span><span class="sxs-lookup"><span data-stu-id="0b076-184">Delete the page.</span></span> |
|[<span data-ttu-id="0b076-185">copyToSection</span><span class="sxs-lookup"><span data-stu-id="0b076-185">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="0b076-186">无</span><span class="sxs-lookup"><span data-stu-id="0b076-186">None</span></span> |<span data-ttu-id="0b076-187">将页面复制到特定分区。</span><span class="sxs-lookup"><span data-stu-id="0b076-187">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
