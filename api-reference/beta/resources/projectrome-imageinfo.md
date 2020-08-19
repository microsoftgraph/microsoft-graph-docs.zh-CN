---
title: imageInfo 资源类型
description: 一个复杂类型，用于表示 activity 对象的 visualInfo 部分中 **的属性属性** 。
localization_priority: Normal
ms.prod: project-rome
doc_type: resourcePageType
author: ailae
ms.openlocfilehash: a57155a880e9ba4e00dd9a4d17ddae3742bbaa8e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807478"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="886af-103">imageInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="886af-103">imageInfo resource type</span></span>

<span data-ttu-id="886af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="886af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="886af-105">一个复杂类型，用于表示[activity](../resources/projectrome-activity.md)对象的[visualInfo](../resources/projectrome-visualinfo.md)部分中**的属性属性**。</span><span class="sxs-lookup"><span data-stu-id="886af-105">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="886af-106">属性</span><span class="sxs-lookup"><span data-stu-id="886af-106">Properties</span></span>

|<span data-ttu-id="886af-107">名称</span><span class="sxs-lookup"><span data-stu-id="886af-107">Name</span></span> | <span data-ttu-id="886af-108">类型</span><span class="sxs-lookup"><span data-stu-id="886af-108">Type</span></span> | <span data-ttu-id="886af-109">说明</span><span class="sxs-lookup"><span data-stu-id="886af-109">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="886af-110">iconUrl</span><span class="sxs-lookup"><span data-stu-id="886af-110">iconUrl</span></span> | <span data-ttu-id="886af-111">String</span><span class="sxs-lookup"><span data-stu-id="886af-111">String</span></span> | <span data-ttu-id="886af-112">Optional指向代表用于生成活动的应用程序的图标的 URI</span><span class="sxs-lookup"><span data-stu-id="886af-112">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="886af-113">alternateText</span><span class="sxs-lookup"><span data-stu-id="886af-113">alternateText</span></span> | <span data-ttu-id="886af-114">String</span><span class="sxs-lookup"><span data-stu-id="886af-114">String</span></span> | <span data-ttu-id="886af-115">Optional图像的可选文本可访问内容</span><span class="sxs-lookup"><span data-stu-id="886af-115">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="886af-116">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="886af-116">addImageQuery</span></span> | <span data-ttu-id="886af-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="886af-117">Boolean</span></span> | <span data-ttu-id="886af-118">Optional用于指示服务器能够动态呈现图像以响应参数化的参数。</span><span class="sxs-lookup"><span data-stu-id="886af-118">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="886af-119">例如-高对比度图像</span><span class="sxs-lookup"><span data-stu-id="886af-119">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="886af-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="886af-120">JSON Representation</span></span>

<span data-ttu-id="886af-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="886af-121">Here is a JSON representation of the resource</span></span>

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
