---
title: mentionsPreview 资源类型
description: 代表资源实例中提及对象的信息。
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 3bb087f6eb1d3c49b85213acf60393346a42b7cf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949288"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="7d500-103">mentionsPreview 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d500-103">mentionsPreview resource type</span></span>

> <span data-ttu-id="7d500-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7d500-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d500-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7d500-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d500-106">代表资源实例中[有提及](../resources/mention.md)对象的信息。</span><span class="sxs-lookup"><span data-stu-id="7d500-106">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="7d500-107">属性</span><span class="sxs-lookup"><span data-stu-id="7d500-107">Properties</span></span>
| <span data-ttu-id="7d500-108">属性</span><span class="sxs-lookup"><span data-stu-id="7d500-108">Property</span></span>     | <span data-ttu-id="7d500-109">类型</span><span class="sxs-lookup"><span data-stu-id="7d500-109">Type</span></span>   |<span data-ttu-id="7d500-110">说明</span><span class="sxs-lookup"><span data-stu-id="7d500-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7d500-111">isMentioned</span><span class="sxs-lookup"><span data-stu-id="7d500-111">isMentioned</span></span> | <span data-ttu-id="7d500-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d500-112">Boolean</span></span> | <span data-ttu-id="7d500-113">如果已登录的用户提及的父资源实例中，则为 true。</span><span class="sxs-lookup"><span data-stu-id="7d500-113">True if the signed-in user is mentioned in the parent resource instance.</span></span> <span data-ttu-id="7d500-114">只读。</span><span class="sxs-lookup"><span data-stu-id="7d500-114">Read-only.</span></span> <span data-ttu-id="7d500-115">支持的筛选器。</span><span class="sxs-lookup"><span data-stu-id="7d500-115">Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7d500-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d500-116">JSON representation</span></span>

<span data-ttu-id="7d500-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d500-117">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "mentionsPreview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
