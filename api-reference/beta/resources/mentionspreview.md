---
title: mentionsPreview 资源类型
description: 代表资源实例中提及对象的信息。
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 55eb69d9ef9f6c3686026f6d46a9c78cc4df167b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518763"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="52a16-103">mentionsPreview 资源类型</span><span class="sxs-lookup"><span data-stu-id="52a16-103">mentionsPreview resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52a16-104">代表资源实例中[有提及](../resources/mention.md)对象的信息。</span><span class="sxs-lookup"><span data-stu-id="52a16-104">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="52a16-105">属性</span><span class="sxs-lookup"><span data-stu-id="52a16-105">Properties</span></span>
| <span data-ttu-id="52a16-106">属性</span><span class="sxs-lookup"><span data-stu-id="52a16-106">Property</span></span>     | <span data-ttu-id="52a16-107">类型</span><span class="sxs-lookup"><span data-stu-id="52a16-107">Type</span></span>   |<span data-ttu-id="52a16-108">说明</span><span class="sxs-lookup"><span data-stu-id="52a16-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="52a16-109">isMentioned</span><span class="sxs-lookup"><span data-stu-id="52a16-109">isMentioned</span></span> | <span data-ttu-id="52a16-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="52a16-110">Boolean</span></span> | <span data-ttu-id="52a16-111">如果已登录的用户提及的父资源实例中，则为 true。</span><span class="sxs-lookup"><span data-stu-id="52a16-111">True if the signed-in user is mentioned in the parent resource instance.</span></span> <span data-ttu-id="52a16-112">只读。</span><span class="sxs-lookup"><span data-stu-id="52a16-112">Read-only.</span></span> <span data-ttu-id="52a16-113">支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="52a16-113">Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="52a16-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52a16-114">JSON representation</span></span>

<span data-ttu-id="52a16-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52a16-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mentionsPreview"
}-->

```json
{
  "isMentioned": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mentionsPreview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mentionspreview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
