---
title: patchContentCommand 资源类型
description: 对修补程序请求中的 OneNote 页面进行的更改。
localization_priority: Normal
ms.openlocfilehash: fb0900490b3fe05e6fb90dc4ab8252620bf43983
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462541"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="74f96-103">patchContentCommand 资源类型</span><span class="sxs-lookup"><span data-stu-id="74f96-103">patchContentCommand resource type</span></span>

<span data-ttu-id="74f96-104">对修补程序请求中的 OneNote 页面进行的更改。</span><span class="sxs-lookup"><span data-stu-id="74f96-104">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="74f96-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="74f96-105">JSON representation</span></span>

<span data-ttu-id="74f96-106">下面是资源的 JSON 表示形式, 它是在[修补程序页/{id} '](../api/page-update.md)请求的正文中发送的。</span><span class="sxs-lookup"><span data-stu-id="74f96-106">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="74f96-107">属性</span><span class="sxs-lookup"><span data-stu-id="74f96-107">Properties</span></span>
| <span data-ttu-id="74f96-108">属性</span><span class="sxs-lookup"><span data-stu-id="74f96-108">Property</span></span>     | <span data-ttu-id="74f96-109">类型</span><span class="sxs-lookup"><span data-stu-id="74f96-109">Type</span></span>   |<span data-ttu-id="74f96-110">说明</span><span class="sxs-lookup"><span data-stu-id="74f96-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74f96-111">action</span><span class="sxs-lookup"><span data-stu-id="74f96-111">action</span></span>|<span data-ttu-id="74f96-112">onenotePatchActionType</span><span class="sxs-lookup"><span data-stu-id="74f96-112">onenotePatchActionType</span></span>|<span data-ttu-id="74f96-113">要在目标元素上执行的操作。</span><span class="sxs-lookup"><span data-stu-id="74f96-113">The action to perform on the target element.</span></span> <span data-ttu-id="74f96-114">可能的值为: `replace`、 `append`、 `delete` `insert`、或`prepend`。</span><span class="sxs-lookup"><span data-stu-id="74f96-114">The possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="74f96-115">内容</span><span class="sxs-lookup"><span data-stu-id="74f96-115">content</span></span>|<span data-ttu-id="74f96-116">String</span><span class="sxs-lookup"><span data-stu-id="74f96-116">String</span></span>|<span data-ttu-id="74f96-117">要添加到页面的格式标准的 HTML 字符串或任意图像或二进制文件数据。</span><span class="sxs-lookup"><span data-stu-id="74f96-117">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="74f96-118">如果内容包含二进制数据, 则必须使用包含 "命令" 部分`multipart/form-data`的内容类型发送该请求。</span><span class="sxs-lookup"><span data-stu-id="74f96-118">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="74f96-119">position</span><span class="sxs-lookup"><span data-stu-id="74f96-119">position</span></span>|<span data-ttu-id="74f96-120">onenotePatchInsertPosition</span><span class="sxs-lookup"><span data-stu-id="74f96-120">onenotePatchInsertPosition</span></span>|<span data-ttu-id="74f96-121">要添加所提供的内容的位置，与目标元素有关。</span><span class="sxs-lookup"><span data-stu-id="74f96-121">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="74f96-122">可能的值为: `after` (默认) 或`before`。</span><span class="sxs-lookup"><span data-stu-id="74f96-122">The possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="74f96-123">target</span><span class="sxs-lookup"><span data-stu-id="74f96-123">target</span></span>|<span data-ttu-id="74f96-124">字符串</span><span class="sxs-lookup"><span data-stu-id="74f96-124">String</span></span>|<span data-ttu-id="74f96-125">要更新的元素。</span><span class="sxs-lookup"><span data-stu-id="74f96-125">The element to update.</span></span> <span data-ttu-id="74f96-126">必须是`#<data-id>`或生成`<id>`的元素, 或`body`或`title`关键字。</span><span class="sxs-lookup"><span data-stu-id="74f96-126">Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
