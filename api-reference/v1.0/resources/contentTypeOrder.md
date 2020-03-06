---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
description: contentTypeOrder 资源指定在选择 UI 中显示内容类型的顺序。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9470596cc064006c3bc4307df5f20634886dfc7f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531777"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="051a1-103">ContentTypeOrder 资源类型</span><span class="sxs-lookup"><span data-stu-id="051a1-103">ContentTypeOrder resource type</span></span>

<span data-ttu-id="051a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="051a1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="051a1-105">**contentTypeOrder** 资源指定在选择 UI 中显示内容类型的顺序。</span><span class="sxs-lookup"><span data-stu-id="051a1-105">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="051a1-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="051a1-106">JSON representation</span></span>

<span data-ttu-id="051a1-107">下面是 **contentTypeOrder** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="051a1-107">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="051a1-108">属性</span><span class="sxs-lookup"><span data-stu-id="051a1-108">Properties</span></span>

| <span data-ttu-id="051a1-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="051a1-109">Property name</span></span> | <span data-ttu-id="051a1-110">类型</span><span class="sxs-lookup"><span data-stu-id="051a1-110">Type</span></span>    | <span data-ttu-id="051a1-111">说明</span><span class="sxs-lookup"><span data-stu-id="051a1-111">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="051a1-112">**default**</span><span class="sxs-lookup"><span data-stu-id="051a1-112">**default**</span></span>   | <span data-ttu-id="051a1-113">boolean</span><span class="sxs-lookup"><span data-stu-id="051a1-113">boolean</span></span> | <span data-ttu-id="051a1-114">这是否为默认的内容类型</span><span class="sxs-lookup"><span data-stu-id="051a1-114">Whether this is the default Content Type</span></span>
| <span data-ttu-id="051a1-115">**position**</span><span class="sxs-lookup"><span data-stu-id="051a1-115">**position**</span></span>  | <span data-ttu-id="051a1-116">Int32</span><span class="sxs-lookup"><span data-stu-id="051a1-116">Int32</span></span>   | <span data-ttu-id="051a1-117">指定在选择 UI 中显示内容类型的位置。</span><span class="sxs-lookup"><span data-stu-id="051a1-117">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
