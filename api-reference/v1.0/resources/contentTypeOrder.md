---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
description: contentTypeOrder 资源指定在选择 UI 中显示内容类型的顺序。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5c77f2dd3763199fea8f0a1377a1b46f8aa4881d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032835"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="6c88e-103">ContentTypeOrder 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c88e-103">ContentTypeOrder resource type</span></span>

<span data-ttu-id="6c88e-104">**contentTypeOrder** 资源指定在选择 UI 中显示内容类型的顺序。</span><span class="sxs-lookup"><span data-stu-id="6c88e-104">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c88e-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c88e-105">JSON representation</span></span>

<span data-ttu-id="6c88e-106">下面是 **contentTypeOrder** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c88e-106">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="6c88e-107">属性</span><span class="sxs-lookup"><span data-stu-id="6c88e-107">Properties</span></span>

| <span data-ttu-id="6c88e-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="6c88e-108">Property name</span></span> | <span data-ttu-id="6c88e-109">类型</span><span class="sxs-lookup"><span data-stu-id="6c88e-109">Type</span></span>    | <span data-ttu-id="6c88e-110">说明</span><span class="sxs-lookup"><span data-stu-id="6c88e-110">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="6c88e-111">**default**</span><span class="sxs-lookup"><span data-stu-id="6c88e-111">**default**</span></span>   | <span data-ttu-id="6c88e-112">boolean</span><span class="sxs-lookup"><span data-stu-id="6c88e-112">boolean</span></span> | <span data-ttu-id="6c88e-113">这是否为默认的内容类型</span><span class="sxs-lookup"><span data-stu-id="6c88e-113">Whether this is the default Content Type</span></span>
| <span data-ttu-id="6c88e-114">**position**</span><span class="sxs-lookup"><span data-stu-id="6c88e-114">**position**</span></span>  | <span data-ttu-id="6c88e-115">Int32</span><span class="sxs-lookup"><span data-stu-id="6c88e-115">Int32</span></span>   | <span data-ttu-id="6c88e-116">指定在选择 UI 中显示内容类型的位置。</span><span class="sxs-lookup"><span data-stu-id="6c88e-116">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
