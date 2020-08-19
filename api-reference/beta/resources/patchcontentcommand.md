---
title: patchContentCommand 资源类型
description: 对修补程序请求中的 OneNote 页面进行的更改。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: cd7033ba271ba777d35f2469984662edbd7ffe53
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807176"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="76c34-103">patchContentCommand 资源类型</span><span class="sxs-lookup"><span data-stu-id="76c34-103">patchContentCommand resource type</span></span>

<span data-ttu-id="76c34-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76c34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76c34-105">对修补程序请求中的 OneNote 页面进行的更改。</span><span class="sxs-lookup"><span data-stu-id="76c34-105">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="76c34-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76c34-106">JSON representation</span></span>

<span data-ttu-id="76c34-107">下面是资源的 JSON 表示形式，它是在 [修补程序页/{id} '](../api/page-update.md) 请求的正文中发送的。</span><span class="sxs-lookup"><span data-stu-id="76c34-107">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span>

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

## <a name="properties"></a><span data-ttu-id="76c34-108">属性</span><span class="sxs-lookup"><span data-stu-id="76c34-108">Properties</span></span>
| <span data-ttu-id="76c34-109">属性</span><span class="sxs-lookup"><span data-stu-id="76c34-109">Property</span></span>     | <span data-ttu-id="76c34-110">类型</span><span class="sxs-lookup"><span data-stu-id="76c34-110">Type</span></span>   |<span data-ttu-id="76c34-111">说明</span><span class="sxs-lookup"><span data-stu-id="76c34-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76c34-112">action</span><span class="sxs-lookup"><span data-stu-id="76c34-112">action</span></span>|<span data-ttu-id="76c34-113">String</span><span class="sxs-lookup"><span data-stu-id="76c34-113">String</span></span>|<span data-ttu-id="76c34-114">要在目标元素上执行的操作。</span><span class="sxs-lookup"><span data-stu-id="76c34-114">The action to perform on the target element.</span></span> <span data-ttu-id="76c34-115">可取值为：`replace`、`append`、`delete`、`insert` 或 `prepend`。</span><span class="sxs-lookup"><span data-stu-id="76c34-115">Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="76c34-116">内容</span><span class="sxs-lookup"><span data-stu-id="76c34-116">content</span></span>|<span data-ttu-id="76c34-117">String</span><span class="sxs-lookup"><span data-stu-id="76c34-117">String</span></span>|<span data-ttu-id="76c34-118">要添加到页面的格式标准的 HTML 字符串或任意图像或二进制文件数据。</span><span class="sxs-lookup"><span data-stu-id="76c34-118">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="76c34-119">如果内容包含二进制数据，则必须使用 `multipart/form-data` 包含 "命令" 部分的内容类型发送该请求。</span><span class="sxs-lookup"><span data-stu-id="76c34-119">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="76c34-120">position</span><span class="sxs-lookup"><span data-stu-id="76c34-120">position</span></span>|<span data-ttu-id="76c34-121">String</span><span class="sxs-lookup"><span data-stu-id="76c34-121">String</span></span>|<span data-ttu-id="76c34-122">要添加所提供的内容的位置，与目标元素有关。</span><span class="sxs-lookup"><span data-stu-id="76c34-122">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="76c34-123">可能的值包括： `after` (默认) 或 `before` 。</span><span class="sxs-lookup"><span data-stu-id="76c34-123">Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="76c34-124">target</span><span class="sxs-lookup"><span data-stu-id="76c34-124">target</span></span>|<span data-ttu-id="76c34-125">String</span><span class="sxs-lookup"><span data-stu-id="76c34-125">String</span></span>|<span data-ttu-id="76c34-126">要更新的元素。</span><span class="sxs-lookup"><span data-stu-id="76c34-126">The element to update.</span></span> <span data-ttu-id="76c34-127">必须是 `#<data-id>` 或生成 `{id}` 的元素，或 `body` 或 `title` 关键字。</span><span class="sxs-lookup"><span data-stu-id="76c34-127">Must be the `#<data-id>` or the generated `{id}` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
