---
title: onenotePage 资源类型
description: OneNote 笔记本中的页面。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: 2f8a93080b3eaa58be95e8721307cdde31b359ea
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719449"
---
# <a name="onenotepage-resource-type"></a><span data-ttu-id="24822-103">onenotePage 资源类型</span><span class="sxs-lookup"><span data-stu-id="24822-103">onenotePage resource type</span></span>

<span data-ttu-id="24822-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24822-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24822-105">OneNote 笔记本中的页面。</span><span class="sxs-lookup"><span data-stu-id="24822-105">A page in a OneNote notebook.</span></span>

## <a name="properties"></a><span data-ttu-id="24822-106">属性</span><span class="sxs-lookup"><span data-stu-id="24822-106">Properties</span></span>
| <span data-ttu-id="24822-107">属性</span><span class="sxs-lookup"><span data-stu-id="24822-107">Property</span></span>     | <span data-ttu-id="24822-108">类型</span><span class="sxs-lookup"><span data-stu-id="24822-108">Type</span></span>   |<span data-ttu-id="24822-109">说明</span><span class="sxs-lookup"><span data-stu-id="24822-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24822-110">content</span><span class="sxs-lookup"><span data-stu-id="24822-110">content</span></span>|<span data-ttu-id="24822-111">流</span><span class="sxs-lookup"><span data-stu-id="24822-111">Stream</span></span>|<span data-ttu-id="24822-112">页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="24822-112">The page's HTML content.</span></span>|
|<span data-ttu-id="24822-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="24822-113">contentUrl</span></span>|<span data-ttu-id="24822-114">String</span><span class="sxs-lookup"><span data-stu-id="24822-114">String</span></span>|<span data-ttu-id="24822-115">页面的 HTML 内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="24822-115">The URL for the page's HTML content.</span></span>  <span data-ttu-id="24822-116">只读。</span><span class="sxs-lookup"><span data-stu-id="24822-116">Read-only.</span></span>|
|<span data-ttu-id="24822-117">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="24822-117">createdByAppId</span></span>|<span data-ttu-id="24822-118">字符串</span><span class="sxs-lookup"><span data-stu-id="24822-118">String</span></span>|<span data-ttu-id="24822-119">创建页面的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="24822-119">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="24822-120">只读。</span><span class="sxs-lookup"><span data-stu-id="24822-120">Read-only.</span></span>|
|<span data-ttu-id="24822-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24822-121">createdDateTime</span></span>|<span data-ttu-id="24822-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24822-122">DateTimeOffset</span></span>|<span data-ttu-id="24822-123">页面的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="24822-123">The date and time when the page was created.</span></span> <span data-ttu-id="24822-124">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="24822-124">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="24822-125">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="24822-125">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="24822-126">只读。</span><span class="sxs-lookup"><span data-stu-id="24822-126">Read-only.</span></span>|
|<span data-ttu-id="24822-127">id</span><span class="sxs-lookup"><span data-stu-id="24822-127">id</span></span>|<span data-ttu-id="24822-128">String</span><span class="sxs-lookup"><span data-stu-id="24822-128">String</span></span>|<span data-ttu-id="24822-129">页面的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="24822-129">The unique identifier of the page.</span></span>  <span data-ttu-id="24822-130">只读。</span><span class="sxs-lookup"><span data-stu-id="24822-130">Read-only.</span></span>|
|<span data-ttu-id="24822-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24822-131">lastModifiedDateTime</span></span>|<span data-ttu-id="24822-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24822-132">DateTimeOffset</span></span>|<span data-ttu-id="24822-133">上次修改页面的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="24822-133">The date and time when the page was last modified.</span></span> <span data-ttu-id="24822-134">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="24822-134">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="24822-135">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="24822-135">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="24822-136">只读。</span><span class="sxs-lookup"><span data-stu-id="24822-136">Read-only.</span></span>|
|<span data-ttu-id="24822-137">level</span><span class="sxs-lookup"><span data-stu-id="24822-137">level</span></span>|<span data-ttu-id="24822-138">Int32</span><span class="sxs-lookup"><span data-stu-id="24822-138">Int32</span></span>|<span data-ttu-id="24822-139">页面的缩进级别。</span><span class="sxs-lookup"><span data-stu-id="24822-139">The indentation level of the page.</span></span> <span data-ttu-id="24822-140">只读。</span><span class="sxs-lookup"><span data-stu-id="24822-140">Read-only.</span></span>|
|<span data-ttu-id="24822-141">links</span><span class="sxs-lookup"><span data-stu-id="24822-141">links</span></span>|[<span data-ttu-id="24822-142">pageLinks</span><span class="sxs-lookup"><span data-stu-id="24822-142">pageLinks</span></span>](pagelinks.md)|<span data-ttu-id="24822-143">用于打开页面的链接。</span><span class="sxs-lookup"><span data-stu-id="24822-143">Links for opening the page.</span></span> <span data-ttu-id="24822-144">如果 `oneNoteClientURL` 已安装，链接将在 OneNote 本机客户端中打开页面。</span><span class="sxs-lookup"><span data-stu-id="24822-144">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="24822-145">该 `oneNoteWebUrl` 链接在 Web 上的 OneNote 中打开页面。</span><span class="sxs-lookup"><span data-stu-id="24822-145">The `oneNoteWebUrl` link opens the page in OneNote on the web.</span></span> <span data-ttu-id="24822-146">只读。</span><span class="sxs-lookup"><span data-stu-id="24822-146">Read-only.</span></span>|
|<span data-ttu-id="24822-147">order</span><span class="sxs-lookup"><span data-stu-id="24822-147">order</span></span>|<span data-ttu-id="24822-148">Int32</span><span class="sxs-lookup"><span data-stu-id="24822-148">Int32</span></span>|<span data-ttu-id="24822-149">页面在其父节内的顺序。</span><span class="sxs-lookup"><span data-stu-id="24822-149">The order of the page within its parent section.</span></span> <span data-ttu-id="24822-150">只读。</span><span class="sxs-lookup"><span data-stu-id="24822-150">Read-only.</span></span>|
|<span data-ttu-id="24822-151">self</span><span class="sxs-lookup"><span data-stu-id="24822-151">self</span></span>|<span data-ttu-id="24822-152">String</span><span class="sxs-lookup"><span data-stu-id="24822-152">String</span></span>|<span data-ttu-id="24822-153">可在其中获取页面详细信息的终结点。</span><span class="sxs-lookup"><span data-stu-id="24822-153">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="24822-154">只读。</span><span class="sxs-lookup"><span data-stu-id="24822-154">Read-only.</span></span>|
|<span data-ttu-id="24822-155">title</span><span class="sxs-lookup"><span data-stu-id="24822-155">title</span></span>|<span data-ttu-id="24822-156">String</span><span class="sxs-lookup"><span data-stu-id="24822-156">String</span></span>|<span data-ttu-id="24822-157">页面的标题。</span><span class="sxs-lookup"><span data-stu-id="24822-157">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="24822-158">关系</span><span class="sxs-lookup"><span data-stu-id="24822-158">Relationships</span></span>
| <span data-ttu-id="24822-159">关系</span><span class="sxs-lookup"><span data-stu-id="24822-159">Relationship</span></span> | <span data-ttu-id="24822-160">类型</span><span class="sxs-lookup"><span data-stu-id="24822-160">Type</span></span>   |<span data-ttu-id="24822-161">说明</span><span class="sxs-lookup"><span data-stu-id="24822-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24822-162">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="24822-162">parentNotebook</span></span>|[<span data-ttu-id="24822-163">笔记本</span><span class="sxs-lookup"><span data-stu-id="24822-163">notebook</span></span>](notebook.md)|<span data-ttu-id="24822-164">包含页面的笔记本。</span><span class="sxs-lookup"><span data-stu-id="24822-164">The notebook that contains the page.</span></span>  <span data-ttu-id="24822-165">只读。</span><span class="sxs-lookup"><span data-stu-id="24822-165">Read-only.</span></span>|
|<span data-ttu-id="24822-166">parentSection</span><span class="sxs-lookup"><span data-stu-id="24822-166">parentSection</span></span>|[<span data-ttu-id="24822-167">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="24822-167">onenoteSection</span></span>](onenotesection.md)|<span data-ttu-id="24822-168">包含页面的部分。</span><span class="sxs-lookup"><span data-stu-id="24822-168">The section that contains the page.</span></span> <span data-ttu-id="24822-169">只读的。</span><span class="sxs-lookup"><span data-stu-id="24822-169">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="24822-170">方法</span><span class="sxs-lookup"><span data-stu-id="24822-170">Methods</span></span>

| <span data-ttu-id="24822-171">方法</span><span class="sxs-lookup"><span data-stu-id="24822-171">Method</span></span>           | <span data-ttu-id="24822-172">返回类型</span><span class="sxs-lookup"><span data-stu-id="24822-172">Return Type</span></span>    |<span data-ttu-id="24822-173">说明</span><span class="sxs-lookup"><span data-stu-id="24822-173">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="24822-174">获取页面</span><span class="sxs-lookup"><span data-stu-id="24822-174">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="24822-175">onenotePage</span><span class="sxs-lookup"><span data-stu-id="24822-175">onenotePage</span></span>](onenotepage.md) |<span data-ttu-id="24822-176">读取页面的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="24822-176">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="24822-177">更新页面内容</span><span class="sxs-lookup"><span data-stu-id="24822-177">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="24822-178">无</span><span class="sxs-lookup"><span data-stu-id="24822-178">None</span></span> |<span data-ttu-id="24822-179">更新页面的 HTML 内容。</span><span class="sxs-lookup"><span data-stu-id="24822-179">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="24822-180">删除页面</span><span class="sxs-lookup"><span data-stu-id="24822-180">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="24822-181">无</span><span class="sxs-lookup"><span data-stu-id="24822-181">None</span></span> |<span data-ttu-id="24822-182">删除页面。</span><span class="sxs-lookup"><span data-stu-id="24822-182">Delete the page.</span></span> |
|[<span data-ttu-id="24822-183">copyToSection</span><span class="sxs-lookup"><span data-stu-id="24822-183">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="24822-184">无</span><span class="sxs-lookup"><span data-stu-id="24822-184">None</span></span> |<span data-ttu-id="24822-185">将页面复制到特定节。</span><span class="sxs-lookup"><span data-stu-id="24822-185">Copies the page to a specific section.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24822-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24822-186">JSON representation</span></span>

<span data-ttu-id="24822-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24822-187">Here is a JSON representation of the resource.</span></span>

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


