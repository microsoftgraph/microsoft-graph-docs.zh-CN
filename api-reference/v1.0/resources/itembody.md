---
title: itemBody 资源类型
description: 表示项目正文的属性，例如邮件、事件或组帖子。
ms.openlocfilehash: ebcc2797052ac3a5a73547332e37c5e9c1bd3a41
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010276"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="08288-103">itemBody 资源类型</span><span class="sxs-lookup"><span data-stu-id="08288-103">itemBody resource type</span></span>

<span data-ttu-id="08288-104">表示项目正文的属性，例如邮件、事件或组帖子。</span><span class="sxs-lookup"><span data-stu-id="08288-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="08288-105">属性</span><span class="sxs-lookup"><span data-stu-id="08288-105">Properties</span></span>
| <span data-ttu-id="08288-106">属性</span><span class="sxs-lookup"><span data-stu-id="08288-106">Property</span></span>     | <span data-ttu-id="08288-107">类型</span><span class="sxs-lookup"><span data-stu-id="08288-107">Type</span></span>   |<span data-ttu-id="08288-108">说明</span><span class="sxs-lookup"><span data-stu-id="08288-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08288-109">内容</span><span class="sxs-lookup"><span data-stu-id="08288-109">content</span></span>|<span data-ttu-id="08288-110">String</span><span class="sxs-lookup"><span data-stu-id="08288-110">String</span></span>|<span data-ttu-id="08288-111">项目的内容。</span><span class="sxs-lookup"><span data-stu-id="08288-111">The content of the item.</span></span>|
|<span data-ttu-id="08288-112">contentType</span><span class="sxs-lookup"><span data-stu-id="08288-112">contentType</span></span>|<span data-ttu-id="08288-113">bodyType</span><span class="sxs-lookup"><span data-stu-id="08288-113">bodyType</span></span>|<span data-ttu-id="08288-p101">内容的类型。可能的值为 `Text` 和 `HTML`。</span><span class="sxs-lookup"><span data-stu-id="08288-p101">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08288-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="08288-116">JSON representation</span></span>

<span data-ttu-id="08288-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08288-117">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
