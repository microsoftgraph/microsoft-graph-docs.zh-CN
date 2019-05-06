---
title: onenotePage 资源类型
description: OneNote 笔记本中的页面。
localization_priority: Normal
ms.openlocfilehash: 04e06fefd0b48a5d794f20733a4755e030cb7e0d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630795"
---
# <a name="onenotepage-resource-type"></a><span data-ttu-id="cc246-103">onenotePage 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc246-103">onenotePage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc246-104">OneNote 笔记本中的页面。</span><span class="sxs-lookup"><span data-stu-id="cc246-104">A page in a OneNote notebook.</span></span>

## <a name="properties"></a><span data-ttu-id="cc246-105">属性</span><span class="sxs-lookup"><span data-stu-id="cc246-105">Properties</span></span>
| <span data-ttu-id="cc246-106">属性</span><span class="sxs-lookup"><span data-stu-id="cc246-106">Property</span></span>     | <span data-ttu-id="cc246-107">类型</span><span class="sxs-lookup"><span data-stu-id="cc246-107">Type</span></span>   |<span data-ttu-id="cc246-108">说明</span><span class="sxs-lookup"><span data-stu-id="cc246-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc246-109">content</span><span class="sxs-lookup"><span data-stu-id="cc246-109">content</span></span>|<span data-ttu-id="cc246-110">流</span><span class="sxs-lookup"><span data-stu-id="cc246-110">Stream</span></span>|<span data-ttu-id="cc246-111">页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="cc246-111">The page's HTML content.</span></span>|
|<span data-ttu-id="cc246-112">contentUrl</span><span class="sxs-lookup"><span data-stu-id="cc246-112">contentUrl</span></span>|<span data-ttu-id="cc246-113">字符串</span><span class="sxs-lookup"><span data-stu-id="cc246-113">String</span></span>|<span data-ttu-id="cc246-114">页面的 HTML 内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="cc246-114">The URL for the page's HTML content.</span></span>  <span data-ttu-id="cc246-115">只读。</span><span class="sxs-lookup"><span data-stu-id="cc246-115">Read-only.</span></span>|
|<span data-ttu-id="cc246-116">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="cc246-116">createdByAppId</span></span>|<span data-ttu-id="cc246-117">字符串</span><span class="sxs-lookup"><span data-stu-id="cc246-117">String</span></span>|<span data-ttu-id="cc246-118">创建页面的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cc246-118">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="cc246-119">只读。</span><span class="sxs-lookup"><span data-stu-id="cc246-119">Read-only.</span></span>|
|<span data-ttu-id="cc246-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc246-120">createdDateTime</span></span>|<span data-ttu-id="cc246-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc246-121">DateTimeOffset</span></span>|<span data-ttu-id="cc246-122">页面的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cc246-122">The date and time when the page was created.</span></span> <span data-ttu-id="cc246-123">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="cc246-123">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cc246-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="cc246-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="cc246-125">只读。</span><span class="sxs-lookup"><span data-stu-id="cc246-125">Read-only.</span></span>|
|<span data-ttu-id="cc246-126">id</span><span class="sxs-lookup"><span data-stu-id="cc246-126">id</span></span>|<span data-ttu-id="cc246-127">字符串</span><span class="sxs-lookup"><span data-stu-id="cc246-127">String</span></span>|<span data-ttu-id="cc246-128">页面的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cc246-128">The unique identifier of the page.</span></span>  <span data-ttu-id="cc246-129">只读。</span><span class="sxs-lookup"><span data-stu-id="cc246-129">Read-only.</span></span>|
|<span data-ttu-id="cc246-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc246-130">lastModifiedDateTime</span></span>|<span data-ttu-id="cc246-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc246-131">DateTimeOffset</span></span>|<span data-ttu-id="cc246-132">上次修改页面的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cc246-132">The date and time when the page was last modified.</span></span> <span data-ttu-id="cc246-133">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="cc246-133">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cc246-134">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="cc246-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="cc246-135">只读。</span><span class="sxs-lookup"><span data-stu-id="cc246-135">Read-only.</span></span>|
|<span data-ttu-id="cc246-136">块级</span><span class="sxs-lookup"><span data-stu-id="cc246-136">level</span></span>|<span data-ttu-id="cc246-137">Int32</span><span class="sxs-lookup"><span data-stu-id="cc246-137">Int32</span></span>|<span data-ttu-id="cc246-138">页面的缩进级别。</span><span class="sxs-lookup"><span data-stu-id="cc246-138">The indentation level of the page.</span></span> <span data-ttu-id="cc246-139">只读。</span><span class="sxs-lookup"><span data-stu-id="cc246-139">Read-only.</span></span>|
|<span data-ttu-id="cc246-140">links</span><span class="sxs-lookup"><span data-stu-id="cc246-140">links</span></span>|[<span data-ttu-id="cc246-141">pageLinks</span><span class="sxs-lookup"><span data-stu-id="cc246-141">pageLinks</span></span>](pagelinks.md)|<span data-ttu-id="cc246-142">用于打开页面的链接。</span><span class="sxs-lookup"><span data-stu-id="cc246-142">Links for opening the page.</span></span> <span data-ttu-id="cc246-143">如果`oneNoteClientURL`安装了 OneNote 本机客户端, 则链接将在其中打开页面。</span><span class="sxs-lookup"><span data-stu-id="cc246-143">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="cc246-144">`oneNoteWebUrl`链接将在 OneNote Online 中打开页面。</span><span class="sxs-lookup"><span data-stu-id="cc246-144">The `oneNoteWebUrl` link opens the page in OneNote Online.</span></span> <span data-ttu-id="cc246-145">只读。</span><span class="sxs-lookup"><span data-stu-id="cc246-145">Read-only.</span></span>|
|<span data-ttu-id="cc246-146">顺序</span><span class="sxs-lookup"><span data-stu-id="cc246-146">order</span></span>|<span data-ttu-id="cc246-147">Int32</span><span class="sxs-lookup"><span data-stu-id="cc246-147">Int32</span></span>|<span data-ttu-id="cc246-148">页面在其父节中的顺序。</span><span class="sxs-lookup"><span data-stu-id="cc246-148">The order of the page within its parent section.</span></span> <span data-ttu-id="cc246-149">只读。</span><span class="sxs-lookup"><span data-stu-id="cc246-149">Read-only.</span></span>|
|<span data-ttu-id="cc246-150">自学</span><span class="sxs-lookup"><span data-stu-id="cc246-150">self</span></span>|<span data-ttu-id="cc246-151">字符串</span><span class="sxs-lookup"><span data-stu-id="cc246-151">String</span></span>|<span data-ttu-id="cc246-152">可在其中获取有关页面的详细信息的终结点。</span><span class="sxs-lookup"><span data-stu-id="cc246-152">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="cc246-153">只读。</span><span class="sxs-lookup"><span data-stu-id="cc246-153">Read-only.</span></span>|
|<span data-ttu-id="cc246-154">title</span><span class="sxs-lookup"><span data-stu-id="cc246-154">title</span></span>|<span data-ttu-id="cc246-155">String</span><span class="sxs-lookup"><span data-stu-id="cc246-155">String</span></span>|<span data-ttu-id="cc246-156">页面的标题。</span><span class="sxs-lookup"><span data-stu-id="cc246-156">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cc246-157">关系</span><span class="sxs-lookup"><span data-stu-id="cc246-157">Relationships</span></span>
| <span data-ttu-id="cc246-158">关系</span><span class="sxs-lookup"><span data-stu-id="cc246-158">Relationship</span></span> | <span data-ttu-id="cc246-159">类型</span><span class="sxs-lookup"><span data-stu-id="cc246-159">Type</span></span>   |<span data-ttu-id="cc246-160">说明</span><span class="sxs-lookup"><span data-stu-id="cc246-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc246-161">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="cc246-161">parentNotebook</span></span>|[<span data-ttu-id="cc246-162">笔记</span><span class="sxs-lookup"><span data-stu-id="cc246-162">notebook</span></span>](notebook.md)|<span data-ttu-id="cc246-163">包含页面的笔记本。</span><span class="sxs-lookup"><span data-stu-id="cc246-163">The notebook that contains the page.</span></span>  <span data-ttu-id="cc246-164">只读。</span><span class="sxs-lookup"><span data-stu-id="cc246-164">Read-only.</span></span>|
|<span data-ttu-id="cc246-165">parentSection</span><span class="sxs-lookup"><span data-stu-id="cc246-165">parentSection</span></span>|[<span data-ttu-id="cc246-166">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="cc246-166">onenoteSection</span></span>](onenotesection.md)|<span data-ttu-id="cc246-167">包含页面的部分。</span><span class="sxs-lookup"><span data-stu-id="cc246-167">The section that contains the page.</span></span> <span data-ttu-id="cc246-168">只读的。</span><span class="sxs-lookup"><span data-stu-id="cc246-168">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="cc246-169">方法</span><span class="sxs-lookup"><span data-stu-id="cc246-169">Methods</span></span>

| <span data-ttu-id="cc246-170">方法</span><span class="sxs-lookup"><span data-stu-id="cc246-170">Method</span></span>           | <span data-ttu-id="cc246-171">返回类型</span><span class="sxs-lookup"><span data-stu-id="cc246-171">Return Type</span></span>    |<span data-ttu-id="cc246-172">说明</span><span class="sxs-lookup"><span data-stu-id="cc246-172">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cc246-173">获取页面</span><span class="sxs-lookup"><span data-stu-id="cc246-173">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="cc246-174">onenotePage</span><span class="sxs-lookup"><span data-stu-id="cc246-174">onenotePage</span></span>](onenotepage.md) |<span data-ttu-id="cc246-175">读取页面的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cc246-175">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="cc246-176">更新页面内容</span><span class="sxs-lookup"><span data-stu-id="cc246-176">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="cc246-177">无</span><span class="sxs-lookup"><span data-stu-id="cc246-177">None</span></span> |<span data-ttu-id="cc246-178">更新页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="cc246-178">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="cc246-179">删除页面</span><span class="sxs-lookup"><span data-stu-id="cc246-179">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="cc246-180">无</span><span class="sxs-lookup"><span data-stu-id="cc246-180">None</span></span> |<span data-ttu-id="cc246-181">删除页面。</span><span class="sxs-lookup"><span data-stu-id="cc246-181">Delete the page.</span></span> |
|[<span data-ttu-id="cc246-182">copyToSection</span><span class="sxs-lookup"><span data-stu-id="cc246-182">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="cc246-183">无</span><span class="sxs-lookup"><span data-stu-id="cc246-183">None</span></span> |<span data-ttu-id="cc246-184">将页面复制到特定分区。</span><span class="sxs-lookup"><span data-stu-id="cc246-184">Copies the page to a specific section.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc246-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc246-185">JSON representation</span></span>

<span data-ttu-id="cc246-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc246-186">Here is a JSON representation of the resource.</span></span>

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
