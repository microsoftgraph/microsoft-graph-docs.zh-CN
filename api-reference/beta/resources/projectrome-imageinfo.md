---
title: imageInfo 资源类型
description: 代表活动对象的 visualInfo 部件中的**属性**属性的复杂类型。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 347e07b70e8bad6dce8571dd1fbac5cd00d9abdd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978688"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="d8559-103">imageInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8559-103">imageInfo resource type</span></span>

> <span data-ttu-id="d8559-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d8559-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8559-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d8559-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d8559-106">代表[活动](../resources/projectrome-activity.md)对象的[visualInfo](../resources/projectrome-visualinfo.md)部件中的**属性**属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="d8559-106">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="d8559-107">属性</span><span class="sxs-lookup"><span data-stu-id="d8559-107">Properties</span></span>

|<span data-ttu-id="d8559-108">名称</span><span class="sxs-lookup"><span data-stu-id="d8559-108">Name</span></span> | <span data-ttu-id="d8559-109">类型</span><span class="sxs-lookup"><span data-stu-id="d8559-109">Type</span></span> | <span data-ttu-id="d8559-110">说明</span><span class="sxs-lookup"><span data-stu-id="d8559-110">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="d8559-111">iconUrl</span><span class="sxs-lookup"><span data-stu-id="d8559-111">iconUrl</span></span> | <span data-ttu-id="d8559-112">字符串</span><span class="sxs-lookup"><span data-stu-id="d8559-112">String</span></span> | <span data-ttu-id="d8559-113">可选;指向一个表示用于生成活动的应用程序图标的 URI</span><span class="sxs-lookup"><span data-stu-id="d8559-113">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="d8559-114">alternateText</span><span class="sxs-lookup"><span data-stu-id="d8559-114">alternateText</span></span> | <span data-ttu-id="d8559-115">字符串</span><span class="sxs-lookup"><span data-stu-id="d8559-115">String</span></span> | <span data-ttu-id="d8559-116">可选;可选文字辅助内容的图像</span><span class="sxs-lookup"><span data-stu-id="d8559-116">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="d8559-117">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="d8559-117">addImageQuery</span></span> | <span data-ttu-id="d8559-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8559-118">Boolean</span></span> | <span data-ttu-id="d8559-119">可选;参数一起用来指示服务器是能够呈现动态以响应参数化的图像。</span><span class="sxs-lookup"><span data-stu-id="d8559-119">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="d8559-120">例如 – 高对比度图像</span><span class="sxs-lookup"><span data-stu-id="d8559-120">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8559-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8559-121">JSON Representation</span></span>

<span data-ttu-id="d8559-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8559-122">Here is a JSON representation of the resource</span></span>

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
