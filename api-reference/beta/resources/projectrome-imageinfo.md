---
title: imageInfo 资源类型
description: 一个复杂类型, 用于表示**** activity 对象的 visualInfo 部分中的属性属性。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 6ffdacefb11f583f8c9529a36472a01537643c3c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344002"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="073c5-103">imageInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="073c5-103">imageInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="073c5-104">一个复杂类型, 用于表示\*\*\*\* [activity](../resources/projectrome-activity.md)对象的[visualInfo](../resources/projectrome-visualinfo.md)部分中的属性属性。</span><span class="sxs-lookup"><span data-stu-id="073c5-104">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="073c5-105">属性</span><span class="sxs-lookup"><span data-stu-id="073c5-105">Properties</span></span>

|<span data-ttu-id="073c5-106">名称</span><span class="sxs-lookup"><span data-stu-id="073c5-106">Name</span></span> | <span data-ttu-id="073c5-107">类型</span><span class="sxs-lookup"><span data-stu-id="073c5-107">Type</span></span> | <span data-ttu-id="073c5-108">说明</span><span class="sxs-lookup"><span data-stu-id="073c5-108">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="073c5-109">iconUrl</span><span class="sxs-lookup"><span data-stu-id="073c5-109">iconUrl</span></span> | <span data-ttu-id="073c5-110">String</span><span class="sxs-lookup"><span data-stu-id="073c5-110">String</span></span> | <span data-ttu-id="073c5-111">Optional指向代表用于生成活动的应用程序的图标的 URI</span><span class="sxs-lookup"><span data-stu-id="073c5-111">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="073c5-112">alternateText</span><span class="sxs-lookup"><span data-stu-id="073c5-112">alternateText</span></span> | <span data-ttu-id="073c5-113">String</span><span class="sxs-lookup"><span data-stu-id="073c5-113">String</span></span> | <span data-ttu-id="073c5-114">Optional图像的可选文本可访问内容</span><span class="sxs-lookup"><span data-stu-id="073c5-114">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="073c5-115">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="073c5-115">addImageQuery</span></span> | <span data-ttu-id="073c5-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="073c5-116">Boolean</span></span> | <span data-ttu-id="073c5-117">Optional用于指示服务器能够动态呈现图像以响应参数化的参数。</span><span class="sxs-lookup"><span data-stu-id="073c5-117">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="073c5-118">例如-高对比度图像</span><span class="sxs-lookup"><span data-stu-id="073c5-118">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="073c5-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="073c5-119">JSON Representation</span></span>

<span data-ttu-id="073c5-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="073c5-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
