---
title: itemBody 资源类型
description: 表示项目正文的属性，例如邮件、事件或组帖子。
localization_priority: Normal
ms.openlocfilehash: df2e7e8cea9e1b2e6a6d1011029a1898e2794f45
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642560"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="84086-103">itemBody 资源类型</span><span class="sxs-lookup"><span data-stu-id="84086-103">itemBody resource type</span></span>

<span data-ttu-id="84086-104">表示项目正文的属性，例如邮件、事件或组帖子。</span><span class="sxs-lookup"><span data-stu-id="84086-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="84086-105">属性</span><span class="sxs-lookup"><span data-stu-id="84086-105">Properties</span></span>
| <span data-ttu-id="84086-106">属性</span><span class="sxs-lookup"><span data-stu-id="84086-106">Property</span></span>     | <span data-ttu-id="84086-107">类型</span><span class="sxs-lookup"><span data-stu-id="84086-107">Type</span></span>   |<span data-ttu-id="84086-108">说明</span><span class="sxs-lookup"><span data-stu-id="84086-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84086-109">内容</span><span class="sxs-lookup"><span data-stu-id="84086-109">content</span></span>|<span data-ttu-id="84086-110">String</span><span class="sxs-lookup"><span data-stu-id="84086-110">String</span></span>|<span data-ttu-id="84086-111">项目的内容。</span><span class="sxs-lookup"><span data-stu-id="84086-111">The content of the item.</span></span>|
|<span data-ttu-id="84086-112">contentType</span><span class="sxs-lookup"><span data-stu-id="84086-112">contentType</span></span>|<span data-ttu-id="84086-113">bodyType</span><span class="sxs-lookup"><span data-stu-id="84086-113">bodyType</span></span>|<span data-ttu-id="84086-p101">内容的类型。可能的值为 `text` 和 `HTML`。</span><span class="sxs-lookup"><span data-stu-id="84086-p101">The type of the content. Possible values are `text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="84086-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84086-116">JSON representation</span></span>

<span data-ttu-id="84086-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84086-117">Here is a JSON representation of the resource</span></span>

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
