---
title: imageInfo 资源类型
description: 代表活动对象的 visualInfo 部件中的**属性**属性的复杂类型。
localization_priority: Normal
ms.openlocfilehash: 2bac97ff945c0e0975ffa19636a954308b895e88
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856460"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="bce80-103">imageInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="bce80-103">imageInfo resource type</span></span>

<span data-ttu-id="bce80-104">代表[活动](../resources/projectrome-activity.md)对象的[visualInfo](../resources/projectrome-visualinfo.md)部件中的**属性**属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="bce80-104">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="bce80-105">属性</span><span class="sxs-lookup"><span data-stu-id="bce80-105">Properties</span></span>

|<span data-ttu-id="bce80-106">名称</span><span class="sxs-lookup"><span data-stu-id="bce80-106">Name</span></span> | <span data-ttu-id="bce80-107">类型</span><span class="sxs-lookup"><span data-stu-id="bce80-107">Type</span></span> | <span data-ttu-id="bce80-108">Description</span><span class="sxs-lookup"><span data-stu-id="bce80-108">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="bce80-109">iconUrl</span><span class="sxs-lookup"><span data-stu-id="bce80-109">iconUrl</span></span> | <span data-ttu-id="bce80-110">字符串</span><span class="sxs-lookup"><span data-stu-id="bce80-110">String</span></span> | <span data-ttu-id="bce80-111">可选;指向一个表示用于生成活动的应用程序图标的 URI</span><span class="sxs-lookup"><span data-stu-id="bce80-111">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="bce80-112">alternateText</span><span class="sxs-lookup"><span data-stu-id="bce80-112">alternateText</span></span> | <span data-ttu-id="bce80-113">字符串</span><span class="sxs-lookup"><span data-stu-id="bce80-113">String</span></span> | <span data-ttu-id="bce80-114">可选;可选文字辅助内容的图像</span><span class="sxs-lookup"><span data-stu-id="bce80-114">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="bce80-115">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="bce80-115">addImageQuery</span></span> | <span data-ttu-id="bce80-116">布尔</span><span class="sxs-lookup"><span data-stu-id="bce80-116">Boolean</span></span> | <span data-ttu-id="bce80-117">可选;参数一起用来指示服务器是能够呈现动态以响应参数化的图像。</span><span class="sxs-lookup"><span data-stu-id="bce80-117">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="bce80-118">例如 – 高对比度图像</span><span class="sxs-lookup"><span data-stu-id="bce80-118">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bce80-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bce80-119">JSON Representation</span></span>

<span data-ttu-id="bce80-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bce80-120">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
