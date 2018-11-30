---
title: imageInfo 资源类型
description: 代表活动对象的 visualInfo 部件中的**属性**属性的复杂类型。
ms.openlocfilehash: 051338230850da7e754c5e8ad4f7d9c52fe17b32
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010558"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="51344-103">imageInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="51344-103">imageInfo resource type</span></span>

<span data-ttu-id="51344-104">代表[活动](../resources/projectrome-activity.md)对象的[visualInfo](../resources/projectrome-visualinfo.md)部件中的**属性**属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="51344-104">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="51344-105">属性</span><span class="sxs-lookup"><span data-stu-id="51344-105">Properties</span></span>

|<span data-ttu-id="51344-106">名称</span><span class="sxs-lookup"><span data-stu-id="51344-106">Name</span></span> | <span data-ttu-id="51344-107">类型</span><span class="sxs-lookup"><span data-stu-id="51344-107">Type</span></span> | <span data-ttu-id="51344-108">说明</span><span class="sxs-lookup"><span data-stu-id="51344-108">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="51344-109">iconUrl</span><span class="sxs-lookup"><span data-stu-id="51344-109">iconUrl</span></span> | <span data-ttu-id="51344-110">字符串</span><span class="sxs-lookup"><span data-stu-id="51344-110">String</span></span> | <span data-ttu-id="51344-111">可选;指向一个表示用于生成活动的应用程序图标的 URI</span><span class="sxs-lookup"><span data-stu-id="51344-111">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="51344-112">alternateText</span><span class="sxs-lookup"><span data-stu-id="51344-112">alternateText</span></span> | <span data-ttu-id="51344-113">字符串</span><span class="sxs-lookup"><span data-stu-id="51344-113">String</span></span> | <span data-ttu-id="51344-114">可选;可选文字辅助内容的图像</span><span class="sxs-lookup"><span data-stu-id="51344-114">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="51344-115">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="51344-115">addImageQuery</span></span> | <span data-ttu-id="51344-116">布尔</span><span class="sxs-lookup"><span data-stu-id="51344-116">Boolean</span></span> | <span data-ttu-id="51344-117">可选;参数一起用来指示服务器是能够呈现动态以响应参数化的图像。</span><span class="sxs-lookup"><span data-stu-id="51344-117">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="51344-118">例如 – 高对比度图像</span><span class="sxs-lookup"><span data-stu-id="51344-118">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51344-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51344-119">JSON Representation</span></span>

<span data-ttu-id="51344-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51344-120">Here is a JSON representation of the resource</span></span>

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