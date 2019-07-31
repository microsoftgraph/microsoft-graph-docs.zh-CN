---
title: itemBody 资源类型
description: 表示项目正文的属性，例如邮件、事件或组帖子。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 0fa0360e3fe6c05e18446640900ca8840731219c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010061"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="a0fec-103">itemBody 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0fec-103">itemBody resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0fec-104">表示项目正文的属性，例如邮件、事件或组帖子。</span><span class="sxs-lookup"><span data-stu-id="a0fec-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="a0fec-105">属性</span><span class="sxs-lookup"><span data-stu-id="a0fec-105">Properties</span></span>
| <span data-ttu-id="a0fec-106">属性</span><span class="sxs-lookup"><span data-stu-id="a0fec-106">Property</span></span>     | <span data-ttu-id="a0fec-107">类型</span><span class="sxs-lookup"><span data-stu-id="a0fec-107">Type</span></span>   |<span data-ttu-id="a0fec-108">说明</span><span class="sxs-lookup"><span data-stu-id="a0fec-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0fec-109">内容</span><span class="sxs-lookup"><span data-stu-id="a0fec-109">content</span></span>|<span data-ttu-id="a0fec-110">String</span><span class="sxs-lookup"><span data-stu-id="a0fec-110">String</span></span>|<span data-ttu-id="a0fec-111">项目的内容。</span><span class="sxs-lookup"><span data-stu-id="a0fec-111">The content of the item.</span></span>|
|<span data-ttu-id="a0fec-112">contentType</span><span class="sxs-lookup"><span data-stu-id="a0fec-112">contentType</span></span>|<span data-ttu-id="a0fec-113">String</span><span class="sxs-lookup"><span data-stu-id="a0fec-113">String</span></span>|<span data-ttu-id="a0fec-p101">内容的类型。可能的值为 `text` 和 `HTML`。</span><span class="sxs-lookup"><span data-stu-id="a0fec-p101">The type of the content. Possible values are `text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0fec-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0fec-116">JSON representation</span></span>

<span data-ttu-id="a0fec-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0fec-117">Here is a JSON representation of the resource</span></span>

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
