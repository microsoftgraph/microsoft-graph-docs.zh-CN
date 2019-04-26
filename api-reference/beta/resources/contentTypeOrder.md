---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
ms.openlocfilehash: 32cca632933cf2b0fad1f8e9149973d95b4322d3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341226"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="0f963-102">ContentTypeOrder 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f963-102">ContentTypeOrder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f963-103">**contentTypeOrder** 资源指定在选择 UI 中显示内容类型的顺序。</span><span class="sxs-lookup"><span data-stu-id="0f963-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f963-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f963-104">JSON representation</span></span>

<span data-ttu-id="0f963-105">下面是 **contentTypeOrder** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f963-105">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="0f963-106">属性</span><span class="sxs-lookup"><span data-stu-id="0f963-106">Properties</span></span>

| <span data-ttu-id="0f963-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="0f963-107">Property name</span></span> | <span data-ttu-id="0f963-108">类型</span><span class="sxs-lookup"><span data-stu-id="0f963-108">Type</span></span>    | <span data-ttu-id="0f963-109">说明</span><span class="sxs-lookup"><span data-stu-id="0f963-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="0f963-110">**default**</span><span class="sxs-lookup"><span data-stu-id="0f963-110">**default**</span></span>   | <span data-ttu-id="0f963-111">boolean</span><span class="sxs-lookup"><span data-stu-id="0f963-111">boolean</span></span> | <span data-ttu-id="0f963-112">这是否为默认的内容类型</span><span class="sxs-lookup"><span data-stu-id="0f963-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="0f963-113">**position**</span><span class="sxs-lookup"><span data-stu-id="0f963-113">**position**</span></span>  | <span data-ttu-id="0f963-114">Int32</span><span class="sxs-lookup"><span data-stu-id="0f963-114">Int32</span></span>   | <span data-ttu-id="0f963-115">指定在选择 UI 中显示内容类型的位置。</span><span class="sxs-lookup"><span data-stu-id="0f963-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder",
  "suppressions": []
}
-->
