---
title: patchContentCommand 资源类型
description: PATCH 请求中要对 OneNote 页面进行的更改。
localization_priority: Normal
ms.openlocfilehash: d0d8f320d22a8b3466ddd53deee5bcb7955ff3d1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523881"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="59c60-103">patchContentCommand 资源类型</span><span class="sxs-lookup"><span data-stu-id="59c60-103">patchContentCommand resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59c60-104">PATCH 请求中要对 OneNote 页面进行的更改。</span><span class="sxs-lookup"><span data-stu-id="59c60-104">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="59c60-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="59c60-105">JSON representation</span></span>

<span data-ttu-id="59c60-106">其是 [PATCH pages/{id}\`](../api/page-update.md) 请求的正文中发送的资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59c60-106">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}-->

```json
{
  "action": "String",
  "content": "string",
  "position": "String",
  "target": "string"
}

```

## <a name="properties"></a><span data-ttu-id="59c60-107">属性</span><span class="sxs-lookup"><span data-stu-id="59c60-107">Properties</span></span>
| <span data-ttu-id="59c60-108">属性</span><span class="sxs-lookup"><span data-stu-id="59c60-108">Property</span></span>     | <span data-ttu-id="59c60-109">类型</span><span class="sxs-lookup"><span data-stu-id="59c60-109">Type</span></span>   |<span data-ttu-id="59c60-110">说明</span><span class="sxs-lookup"><span data-stu-id="59c60-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59c60-111">action</span><span class="sxs-lookup"><span data-stu-id="59c60-111">action</span></span>|<span data-ttu-id="59c60-112">String</span><span class="sxs-lookup"><span data-stu-id="59c60-112">String</span></span>|<span data-ttu-id="59c60-p101">要在目标元素上执行的操作。可取值为：`replace`、`append`、`delete`、`insert` 或 `prepend`。</span><span class="sxs-lookup"><span data-stu-id="59c60-p101">The action to perform on the target element. Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="59c60-115">content</span><span class="sxs-lookup"><span data-stu-id="59c60-115">content</span></span>|<span data-ttu-id="59c60-116">String</span><span class="sxs-lookup"><span data-stu-id="59c60-116">String</span></span>|<span data-ttu-id="59c60-p102">要添加到页面的格式标准的 HTML 字符串或任意图片或二进制文件数据。如果内容包含二进制数据，则必须使用包含“Commands”部分的 `multipart/form-data` 内容类型发送请求。</span><span class="sxs-lookup"><span data-stu-id="59c60-p102">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="59c60-119">position</span><span class="sxs-lookup"><span data-stu-id="59c60-119">position</span></span>|<span data-ttu-id="59c60-120">String</span><span class="sxs-lookup"><span data-stu-id="59c60-120">String</span></span>|<span data-ttu-id="59c60-p103">要添加所提供的内容的位置，与目标元素有关。可能的值是：`after`（默认值）或 `before`。</span><span class="sxs-lookup"><span data-stu-id="59c60-p103">The location to add the supplied content, relative to the target element. Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="59c60-123">target</span><span class="sxs-lookup"><span data-stu-id="59c60-123">target</span></span>|<span data-ttu-id="59c60-124">String</span><span class="sxs-lookup"><span data-stu-id="59c60-124">String</span></span>|<span data-ttu-id="59c60-p104">要更新的元素。必须为 `#<data-id>` 或元素生成的 `<id>`，或 `body` 或 `title` 关键词。</span><span class="sxs-lookup"><span data-stu-id="59c60-p104">The element to update. Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/patchcontentcommand.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
