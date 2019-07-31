---
title: mentionsPreview 资源类型
description: 表示有关在资源实例中提及对象的信息。
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5c4604657e18498a85aa8646b5d69db7d74299bc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009704"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="645fd-103">mentionsPreview 资源类型</span><span class="sxs-lookup"><span data-stu-id="645fd-103">mentionsPreview resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="645fd-104">表示有关在资源实例中[提及](../resources/mention.md)对象的信息。</span><span class="sxs-lookup"><span data-stu-id="645fd-104">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="645fd-105">属性</span><span class="sxs-lookup"><span data-stu-id="645fd-105">Properties</span></span>
| <span data-ttu-id="645fd-106">属性</span><span class="sxs-lookup"><span data-stu-id="645fd-106">Property</span></span>     | <span data-ttu-id="645fd-107">类型</span><span class="sxs-lookup"><span data-stu-id="645fd-107">Type</span></span>   |<span data-ttu-id="645fd-108">说明</span><span class="sxs-lookup"><span data-stu-id="645fd-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="645fd-109">isMentioned</span><span class="sxs-lookup"><span data-stu-id="645fd-109">isMentioned</span></span> | <span data-ttu-id="645fd-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="645fd-110">Boolean</span></span> | <span data-ttu-id="645fd-111">如此如果在父资源实例中提到了登录用户。</span><span class="sxs-lookup"><span data-stu-id="645fd-111">True if the signed-in user is mentioned in the parent resource instance.</span></span> <span data-ttu-id="645fd-112">只读。</span><span class="sxs-lookup"><span data-stu-id="645fd-112">Read-only.</span></span> <span data-ttu-id="645fd-113">支持筛选器。</span><span class="sxs-lookup"><span data-stu-id="645fd-113">Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="645fd-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="645fd-114">JSON representation</span></span>

<span data-ttu-id="645fd-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="645fd-115">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
