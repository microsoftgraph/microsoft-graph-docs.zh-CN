---
title: itemBody 资源类型
description: 表示项目正文的属性，例如邮件、事件或组帖子。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: grangeryy
ms.openlocfilehash: 0bba7fce9557c6c249ea9aefced5a198a87f5026
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658805"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="f4499-103">itemBody 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4499-103">itemBody resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4499-104">表示项目正文的属性，例如邮件、事件或组帖子。</span><span class="sxs-lookup"><span data-stu-id="f4499-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="f4499-105">属性</span><span class="sxs-lookup"><span data-stu-id="f4499-105">Properties</span></span>
| <span data-ttu-id="f4499-106">属性</span><span class="sxs-lookup"><span data-stu-id="f4499-106">Property</span></span>     | <span data-ttu-id="f4499-107">类型</span><span class="sxs-lookup"><span data-stu-id="f4499-107">Type</span></span>   |<span data-ttu-id="f4499-108">说明</span><span class="sxs-lookup"><span data-stu-id="f4499-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4499-109">内容</span><span class="sxs-lookup"><span data-stu-id="f4499-109">content</span></span>|<span data-ttu-id="f4499-110">String</span><span class="sxs-lookup"><span data-stu-id="f4499-110">String</span></span>|<span data-ttu-id="f4499-111">项目的内容。</span><span class="sxs-lookup"><span data-stu-id="f4499-111">The content of the item.</span></span>|
|<span data-ttu-id="f4499-112">contentType</span><span class="sxs-lookup"><span data-stu-id="f4499-112">contentType</span></span>|<span data-ttu-id="f4499-113">String</span><span class="sxs-lookup"><span data-stu-id="f4499-113">String</span></span>|<span data-ttu-id="f4499-p101">内容的类型。可能的值为 `text` 和 `html`。</span><span class="sxs-lookup"><span data-stu-id="f4499-p101">The type of the content. Possible values are `text` and `html`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4499-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4499-116">JSON representation</span></span>

<span data-ttu-id="f4499-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4499-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemBody"
}-->

```json
{
  "content": "string",
  "contentType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
