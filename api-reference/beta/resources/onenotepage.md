---
title: onenotePage 资源类型
description: OneNote 笔记本中的页面。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3d43f517ec028534e9b443c6e6c6e3e667a09e43
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966417"
---
# <a name="onenotepage-resource-type"></a><span data-ttu-id="7d061-103">onenotePage 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d061-103">onenotePage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d061-104">OneNote 笔记本中的页面。</span><span class="sxs-lookup"><span data-stu-id="7d061-104">A page in a OneNote notebook.</span></span>

## <a name="properties"></a><span data-ttu-id="7d061-105">属性</span><span class="sxs-lookup"><span data-stu-id="7d061-105">Properties</span></span>
| <span data-ttu-id="7d061-106">属性</span><span class="sxs-lookup"><span data-stu-id="7d061-106">Property</span></span>     | <span data-ttu-id="7d061-107">类型</span><span class="sxs-lookup"><span data-stu-id="7d061-107">Type</span></span>   |<span data-ttu-id="7d061-108">说明</span><span class="sxs-lookup"><span data-stu-id="7d061-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d061-109">content</span><span class="sxs-lookup"><span data-stu-id="7d061-109">content</span></span>|<span data-ttu-id="7d061-110">流</span><span class="sxs-lookup"><span data-stu-id="7d061-110">Stream</span></span>|<span data-ttu-id="7d061-111">页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="7d061-111">The page's HTML content.</span></span>|
|<span data-ttu-id="7d061-112">contentUrl</span><span class="sxs-lookup"><span data-stu-id="7d061-112">contentUrl</span></span>|<span data-ttu-id="7d061-113">String</span><span class="sxs-lookup"><span data-stu-id="7d061-113">String</span></span>|<span data-ttu-id="7d061-114">页面的 HTML 内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="7d061-114">The URL for the page's HTML content.</span></span>  <span data-ttu-id="7d061-115">只读。</span><span class="sxs-lookup"><span data-stu-id="7d061-115">Read-only.</span></span>|
|<span data-ttu-id="7d061-116">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="7d061-116">createdByAppId</span></span>|<span data-ttu-id="7d061-117">String</span><span class="sxs-lookup"><span data-stu-id="7d061-117">String</span></span>|<span data-ttu-id="7d061-118">创建页面的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7d061-118">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="7d061-119">只读。</span><span class="sxs-lookup"><span data-stu-id="7d061-119">Read-only.</span></span>|
|<span data-ttu-id="7d061-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d061-120">createdDateTime</span></span>|<span data-ttu-id="7d061-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d061-121">DateTimeOffset</span></span>|<span data-ttu-id="7d061-122">页面的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7d061-122">The date and time when the page was created.</span></span> <span data-ttu-id="7d061-123">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="7d061-123">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7d061-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="7d061-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="7d061-125">只读。</span><span class="sxs-lookup"><span data-stu-id="7d061-125">Read-only.</span></span>|
|<span data-ttu-id="7d061-126">id</span><span class="sxs-lookup"><span data-stu-id="7d061-126">id</span></span>|<span data-ttu-id="7d061-127">字符串</span><span class="sxs-lookup"><span data-stu-id="7d061-127">String</span></span>|<span data-ttu-id="7d061-128">页面的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7d061-128">The unique identifier of the page.</span></span>  <span data-ttu-id="7d061-129">只读。</span><span class="sxs-lookup"><span data-stu-id="7d061-129">Read-only.</span></span>|
|<span data-ttu-id="7d061-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d061-130">lastModifiedDateTime</span></span>|<span data-ttu-id="7d061-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d061-131">DateTimeOffset</span></span>|<span data-ttu-id="7d061-132">上次修改页面的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7d061-132">The date and time when the page was last modified.</span></span> <span data-ttu-id="7d061-133">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="7d061-133">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7d061-134">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="7d061-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="7d061-135">只读。</span><span class="sxs-lookup"><span data-stu-id="7d061-135">Read-only.</span></span>|
|<span data-ttu-id="7d061-136">块级</span><span class="sxs-lookup"><span data-stu-id="7d061-136">level</span></span>|<span data-ttu-id="7d061-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7d061-137">Int32</span></span>|<span data-ttu-id="7d061-138">页面的缩进级别。</span><span class="sxs-lookup"><span data-stu-id="7d061-138">The indentation level of the page.</span></span> <span data-ttu-id="7d061-139">只读。</span><span class="sxs-lookup"><span data-stu-id="7d061-139">Read-only.</span></span>|
|<span data-ttu-id="7d061-140">links</span><span class="sxs-lookup"><span data-stu-id="7d061-140">links</span></span>|[<span data-ttu-id="7d061-141">pageLinks</span><span class="sxs-lookup"><span data-stu-id="7d061-141">pageLinks</span></span>](pagelinks.md)|<span data-ttu-id="7d061-142">用于打开页面的链接。</span><span class="sxs-lookup"><span data-stu-id="7d061-142">Links for opening the page.</span></span> <span data-ttu-id="7d061-143">如果`oneNoteClientURL`安装了 OneNote 本机客户端, 则链接将在其中打开页面。</span><span class="sxs-lookup"><span data-stu-id="7d061-143">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="7d061-144">`oneNoteWebUrl`链接将在 web 上的 OneNote 中打开页面。</span><span class="sxs-lookup"><span data-stu-id="7d061-144">The `oneNoteWebUrl` link opens the page in OneNote on the web.</span></span> <span data-ttu-id="7d061-145">只读。</span><span class="sxs-lookup"><span data-stu-id="7d061-145">Read-only.</span></span>|
|<span data-ttu-id="7d061-146">顺序</span><span class="sxs-lookup"><span data-stu-id="7d061-146">order</span></span>|<span data-ttu-id="7d061-147">Int32</span><span class="sxs-lookup"><span data-stu-id="7d061-147">Int32</span></span>|<span data-ttu-id="7d061-148">页面在其父节中的顺序。</span><span class="sxs-lookup"><span data-stu-id="7d061-148">The order of the page within its parent section.</span></span> <span data-ttu-id="7d061-149">只读。</span><span class="sxs-lookup"><span data-stu-id="7d061-149">Read-only.</span></span>|
|<span data-ttu-id="7d061-150">自学</span><span class="sxs-lookup"><span data-stu-id="7d061-150">self</span></span>|<span data-ttu-id="7d061-151">String</span><span class="sxs-lookup"><span data-stu-id="7d061-151">String</span></span>|<span data-ttu-id="7d061-152">可在其中获取有关页面的详细信息的终结点。</span><span class="sxs-lookup"><span data-stu-id="7d061-152">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="7d061-153">只读。</span><span class="sxs-lookup"><span data-stu-id="7d061-153">Read-only.</span></span>|
|<span data-ttu-id="7d061-154">title</span><span class="sxs-lookup"><span data-stu-id="7d061-154">title</span></span>|<span data-ttu-id="7d061-155">String</span><span class="sxs-lookup"><span data-stu-id="7d061-155">String</span></span>|<span data-ttu-id="7d061-156">页面的标题。</span><span class="sxs-lookup"><span data-stu-id="7d061-156">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7d061-157">关系</span><span class="sxs-lookup"><span data-stu-id="7d061-157">Relationships</span></span>
| <span data-ttu-id="7d061-158">关系</span><span class="sxs-lookup"><span data-stu-id="7d061-158">Relationship</span></span> | <span data-ttu-id="7d061-159">类型</span><span class="sxs-lookup"><span data-stu-id="7d061-159">Type</span></span>   |<span data-ttu-id="7d061-160">说明</span><span class="sxs-lookup"><span data-stu-id="7d061-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d061-161">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="7d061-161">parentNotebook</span></span>|[<span data-ttu-id="7d061-162">笔记</span><span class="sxs-lookup"><span data-stu-id="7d061-162">notebook</span></span>](notebook.md)|<span data-ttu-id="7d061-163">包含页面的笔记本。</span><span class="sxs-lookup"><span data-stu-id="7d061-163">The notebook that contains the page.</span></span>  <span data-ttu-id="7d061-164">只读。</span><span class="sxs-lookup"><span data-stu-id="7d061-164">Read-only.</span></span>|
|<span data-ttu-id="7d061-165">parentSection</span><span class="sxs-lookup"><span data-stu-id="7d061-165">parentSection</span></span>|[<span data-ttu-id="7d061-166">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="7d061-166">onenoteSection</span></span>](onenotesection.md)|<span data-ttu-id="7d061-167">包含页面的部分。</span><span class="sxs-lookup"><span data-stu-id="7d061-167">The section that contains the page.</span></span> <span data-ttu-id="7d061-168">只读的。</span><span class="sxs-lookup"><span data-stu-id="7d061-168">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="7d061-169">方法</span><span class="sxs-lookup"><span data-stu-id="7d061-169">Methods</span></span>

| <span data-ttu-id="7d061-170">方法</span><span class="sxs-lookup"><span data-stu-id="7d061-170">Method</span></span>           | <span data-ttu-id="7d061-171">返回类型</span><span class="sxs-lookup"><span data-stu-id="7d061-171">Return Type</span></span>    |<span data-ttu-id="7d061-172">说明</span><span class="sxs-lookup"><span data-stu-id="7d061-172">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7d061-173">获取页面</span><span class="sxs-lookup"><span data-stu-id="7d061-173">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="7d061-174">onenotePage</span><span class="sxs-lookup"><span data-stu-id="7d061-174">onenotePage</span></span>](onenotepage.md) |<span data-ttu-id="7d061-175">读取页面的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7d061-175">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="7d061-176">更新页面内容</span><span class="sxs-lookup"><span data-stu-id="7d061-176">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="7d061-177">无</span><span class="sxs-lookup"><span data-stu-id="7d061-177">None</span></span> |<span data-ttu-id="7d061-178">更新页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="7d061-178">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="7d061-179">删除页面</span><span class="sxs-lookup"><span data-stu-id="7d061-179">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="7d061-180">无</span><span class="sxs-lookup"><span data-stu-id="7d061-180">None</span></span> |<span data-ttu-id="7d061-181">删除页面。</span><span class="sxs-lookup"><span data-stu-id="7d061-181">Delete the page.</span></span> |
|[<span data-ttu-id="7d061-182">copyToSection</span><span class="sxs-lookup"><span data-stu-id="7d061-182">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="7d061-183">无</span><span class="sxs-lookup"><span data-stu-id="7d061-183">None</span></span> |<span data-ttu-id="7d061-184">将页面复制到特定分区。</span><span class="sxs-lookup"><span data-stu-id="7d061-184">Copies the page to a specific section.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d061-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d061-185">JSON representation</span></span>

<span data-ttu-id="7d061-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d061-186">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
