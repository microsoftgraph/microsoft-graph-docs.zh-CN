---
title: itemBody 资源类型
description: 表示项目正文的属性，例如邮件、事件或组帖子。
localization_priority: Normal
ms.openlocfilehash: f316beda82f292e62d5063f45363e08eeeff7111
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526142"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="d7eab-103">itemBody 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7eab-103">itemBody resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7eab-104">表示项目正文的属性，例如邮件、事件或组帖子。</span><span class="sxs-lookup"><span data-stu-id="d7eab-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="d7eab-105">属性</span><span class="sxs-lookup"><span data-stu-id="d7eab-105">Properties</span></span>
| <span data-ttu-id="d7eab-106">属性</span><span class="sxs-lookup"><span data-stu-id="d7eab-106">Property</span></span>     | <span data-ttu-id="d7eab-107">类型</span><span class="sxs-lookup"><span data-stu-id="d7eab-107">Type</span></span>   |<span data-ttu-id="d7eab-108">说明</span><span class="sxs-lookup"><span data-stu-id="d7eab-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7eab-109">内容</span><span class="sxs-lookup"><span data-stu-id="d7eab-109">content</span></span>|<span data-ttu-id="d7eab-110">String</span><span class="sxs-lookup"><span data-stu-id="d7eab-110">String</span></span>|<span data-ttu-id="d7eab-111">项目的内容。</span><span class="sxs-lookup"><span data-stu-id="d7eab-111">The content of the item.</span></span>|
|<span data-ttu-id="d7eab-112">contentType</span><span class="sxs-lookup"><span data-stu-id="d7eab-112">contentType</span></span>|<span data-ttu-id="d7eab-113">String</span><span class="sxs-lookup"><span data-stu-id="d7eab-113">String</span></span>|<span data-ttu-id="d7eab-p101">内容的类型。可能的值为 `Text` 和 `HTML`。</span><span class="sxs-lookup"><span data-stu-id="d7eab-p101">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7eab-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7eab-116">JSON representation</span></span>

<span data-ttu-id="d7eab-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7eab-117">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/itembody.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
