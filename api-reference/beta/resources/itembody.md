---
title: itemBody 资源类型
description: 表示项目正文的属性，例如邮件、事件或组帖子。
ms.openlocfilehash: 4ceada2ffe8106c270aa262d32ff85e349a8e657
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041548"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="d1de0-103">itemBody 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1de0-103">itemBody resource type</span></span>

> <span data-ttu-id="d1de0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d1de0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1de0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d1de0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1de0-106">表示项目正文的属性，例如邮件、事件或组帖子。</span><span class="sxs-lookup"><span data-stu-id="d1de0-106">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="d1de0-107">属性</span><span class="sxs-lookup"><span data-stu-id="d1de0-107">Properties</span></span>
| <span data-ttu-id="d1de0-108">属性</span><span class="sxs-lookup"><span data-stu-id="d1de0-108">Property</span></span>     | <span data-ttu-id="d1de0-109">类型</span><span class="sxs-lookup"><span data-stu-id="d1de0-109">Type</span></span>   |<span data-ttu-id="d1de0-110">说明</span><span class="sxs-lookup"><span data-stu-id="d1de0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1de0-111">内容</span><span class="sxs-lookup"><span data-stu-id="d1de0-111">content</span></span>|<span data-ttu-id="d1de0-112">String</span><span class="sxs-lookup"><span data-stu-id="d1de0-112">String</span></span>|<span data-ttu-id="d1de0-113">项目的内容。</span><span class="sxs-lookup"><span data-stu-id="d1de0-113">The content of the item.</span></span>|
|<span data-ttu-id="d1de0-114">contentType</span><span class="sxs-lookup"><span data-stu-id="d1de0-114">contentType</span></span>|<span data-ttu-id="d1de0-115">String</span><span class="sxs-lookup"><span data-stu-id="d1de0-115">String</span></span>|<span data-ttu-id="d1de0-p102">内容的类型。可能的值为 `Text` 和 `HTML`。</span><span class="sxs-lookup"><span data-stu-id="d1de0-p102">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d1de0-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1de0-118">JSON representation</span></span>

<span data-ttu-id="d1de0-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1de0-119">Here is a JSON representation of the resource</span></span>

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
