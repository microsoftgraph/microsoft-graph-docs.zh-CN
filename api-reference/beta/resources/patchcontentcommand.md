---
title: patchContentCommand 资源类型
description: PATCH 请求中要对 OneNote 页面进行的更改。
localization_priority: Normal
ms.openlocfilehash: 2e94f67a2a4e2e549d7367f0c48e31745d3bf659
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842726"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="98113-103">patchContentCommand 资源类型</span><span class="sxs-lookup"><span data-stu-id="98113-103">patchContentCommand resource type</span></span>

> <span data-ttu-id="98113-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="98113-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98113-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="98113-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="98113-106">PATCH 请求中要对 OneNote 页面进行的更改。</span><span class="sxs-lookup"><span data-stu-id="98113-106">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="98113-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98113-107">JSON representation</span></span>

<span data-ttu-id="98113-108">其是 [PATCH pages/{id}\`](../api/page-update.md) 请求的正文中发送的资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98113-108">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="98113-109">属性</span><span class="sxs-lookup"><span data-stu-id="98113-109">Properties</span></span>
| <span data-ttu-id="98113-110">属性</span><span class="sxs-lookup"><span data-stu-id="98113-110">Property</span></span>     | <span data-ttu-id="98113-111">类型</span><span class="sxs-lookup"><span data-stu-id="98113-111">Type</span></span>   |<span data-ttu-id="98113-112">说明</span><span class="sxs-lookup"><span data-stu-id="98113-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98113-113">action</span><span class="sxs-lookup"><span data-stu-id="98113-113">action</span></span>|<span data-ttu-id="98113-114">String</span><span class="sxs-lookup"><span data-stu-id="98113-114">String</span></span>|<span data-ttu-id="98113-p102">要在目标元素上执行的操作。可取值为：`replace`、`append`、`delete`、`insert` 或 `prepend`。</span><span class="sxs-lookup"><span data-stu-id="98113-p102">The action to perform on the target element. Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="98113-117">content</span><span class="sxs-lookup"><span data-stu-id="98113-117">content</span></span>|<span data-ttu-id="98113-118">String</span><span class="sxs-lookup"><span data-stu-id="98113-118">String</span></span>|<span data-ttu-id="98113-p103">要添加到页面的格式标准的 HTML 字符串或任意图片或二进制文件数据。如果内容包含二进制数据，则必须使用包含“Commands”部分的 `multipart/form-data` 内容类型发送请求。</span><span class="sxs-lookup"><span data-stu-id="98113-p103">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="98113-121">position</span><span class="sxs-lookup"><span data-stu-id="98113-121">position</span></span>|<span data-ttu-id="98113-122">String</span><span class="sxs-lookup"><span data-stu-id="98113-122">String</span></span>|<span data-ttu-id="98113-p104">要添加所提供的内容的位置，与目标元素有关。可能的值是：`after`（默认值）或 `before`。</span><span class="sxs-lookup"><span data-stu-id="98113-p104">The location to add the supplied content, relative to the target element. Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="98113-125">target</span><span class="sxs-lookup"><span data-stu-id="98113-125">target</span></span>|<span data-ttu-id="98113-126">字符串</span><span class="sxs-lookup"><span data-stu-id="98113-126">String</span></span>|<span data-ttu-id="98113-p105">要更新的元素。必须为 `#<data-id>` 或元素生成的 `<id>`，或 `body` 或 `title` 关键词。</span><span class="sxs-lookup"><span data-stu-id="98113-p105">The element to update. Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
