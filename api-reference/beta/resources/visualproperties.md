---
title: visualProperties 资源类型
description: '表示面向用户的视觉通知的可视内容（即标题和正文）。  '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 1678f560fa003c1884a9fa673ee85b7473e36c88
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519461"
---
# <a name="visualproperties-resource-type"></a><span data-ttu-id="d68d1-103">visualProperties 资源类型</span><span class="sxs-lookup"><span data-stu-id="d68d1-103">visualProperties resource type</span></span>

<span data-ttu-id="d68d1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d68d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d68d1-105">表示面向用户的视觉通知的可视内容（即标题和正文）。</span><span class="sxs-lookup"><span data-stu-id="d68d1-105">Represents the visual content, namely title and body, of a visual notification targeted to a user.</span></span> 

## <a name="properties"></a><span data-ttu-id="d68d1-106">属性</span><span class="sxs-lookup"><span data-stu-id="d68d1-106">Properties</span></span>

| <span data-ttu-id="d68d1-107">属性</span><span class="sxs-lookup"><span data-stu-id="d68d1-107">Property</span></span>     | <span data-ttu-id="d68d1-108">类型</span><span class="sxs-lookup"><span data-stu-id="d68d1-108">Type</span></span>        | <span data-ttu-id="d68d1-109">说明</span><span class="sxs-lookup"><span data-stu-id="d68d1-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d68d1-110">title</span><span class="sxs-lookup"><span data-stu-id="d68d1-110">title</span></span>|<span data-ttu-id="d68d1-111">String</span><span class="sxs-lookup"><span data-stu-id="d68d1-111">String</span></span>|<span data-ttu-id="d68d1-112">可视用户通知的标题。</span><span class="sxs-lookup"><span data-stu-id="d68d1-112">The title of a visual user notification.</span></span> <span data-ttu-id="d68d1-113">此字段对于 visual 通知负载来说是必需的。</span><span class="sxs-lookup"><span data-stu-id="d68d1-113">This field is required for visual notification payloads.</span></span> |
|<span data-ttu-id="d68d1-114">body</span><span class="sxs-lookup"><span data-stu-id="d68d1-114">body</span></span>|<span data-ttu-id="d68d1-115">String</span><span class="sxs-lookup"><span data-stu-id="d68d1-115">String</span></span>|<span data-ttu-id="d68d1-116">可视化用户通知的正文。</span><span class="sxs-lookup"><span data-stu-id="d68d1-116">The body of a visual user notification.</span></span> <span data-ttu-id="d68d1-117">正文是可选的。</span><span class="sxs-lookup"><span data-stu-id="d68d1-117">Body is optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d68d1-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d68d1-118">JSON representation</span></span>

<span data-ttu-id="d68d1-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d68d1-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.visualProperties",
  "baseType": null
}-->

```json
{
  "title": "String",
  "body": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualProperties resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->