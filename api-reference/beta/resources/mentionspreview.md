---
title: mentionsPreview 资源类型
description: 表示有关在资源实例中提及对象的信息。
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 721cd2b82e972f98c36252b6cef9c18623390c93
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971601"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="3e954-103">mentionsPreview 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e954-103">mentionsPreview resource type</span></span>

<span data-ttu-id="3e954-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e954-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e954-105">表示有关在资源实例中 [提及](../resources/mention.md) 对象的信息。</span><span class="sxs-lookup"><span data-stu-id="3e954-105">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="3e954-106">属性</span><span class="sxs-lookup"><span data-stu-id="3e954-106">Properties</span></span>
| <span data-ttu-id="3e954-107">属性</span><span class="sxs-lookup"><span data-stu-id="3e954-107">Property</span></span>     | <span data-ttu-id="3e954-108">类型</span><span class="sxs-lookup"><span data-stu-id="3e954-108">Type</span></span>   |<span data-ttu-id="3e954-109">说明</span><span class="sxs-lookup"><span data-stu-id="3e954-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3e954-110">isMentioned</span><span class="sxs-lookup"><span data-stu-id="3e954-110">isMentioned</span></span> | <span data-ttu-id="3e954-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e954-111">Boolean</span></span> | <span data-ttu-id="3e954-112">如此如果在父资源实例中提到了登录用户。</span><span class="sxs-lookup"><span data-stu-id="3e954-112">True if the signed-in user is mentioned in the parent resource instance.</span></span> <span data-ttu-id="3e954-113">只读。</span><span class="sxs-lookup"><span data-stu-id="3e954-113">Read-only.</span></span> <span data-ttu-id="3e954-114">支持筛选器。</span><span class="sxs-lookup"><span data-stu-id="3e954-114">Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3e954-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e954-115">JSON representation</span></span>

<span data-ttu-id="3e954-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e954-116">Here is a JSON representation of the resource.</span></span>

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


