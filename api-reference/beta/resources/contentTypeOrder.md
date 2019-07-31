---
author: daspek
description: contentTypeOrder 资源指定在选择 UI 中显示内容类型的顺序。
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 464ac5978f505e74ca99226080c35574917fd550
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973195"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="8c315-103">ContentTypeOrder 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c315-103">ContentTypeOrder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c315-104">**contentTypeOrder** 资源指定在选择 UI 中显示内容类型的顺序。</span><span class="sxs-lookup"><span data-stu-id="8c315-104">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c315-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c315-105">JSON representation</span></span>

<span data-ttu-id="8c315-106">下面是 **contentTypeOrder** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c315-106">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="8c315-107">属性</span><span class="sxs-lookup"><span data-stu-id="8c315-107">Properties</span></span>

| <span data-ttu-id="8c315-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="8c315-108">Property name</span></span> | <span data-ttu-id="8c315-109">类型</span><span class="sxs-lookup"><span data-stu-id="8c315-109">Type</span></span>    | <span data-ttu-id="8c315-110">说明</span><span class="sxs-lookup"><span data-stu-id="8c315-110">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="8c315-111">**default**</span><span class="sxs-lookup"><span data-stu-id="8c315-111">**default**</span></span>   | <span data-ttu-id="8c315-112">boolean</span><span class="sxs-lookup"><span data-stu-id="8c315-112">boolean</span></span> | <span data-ttu-id="8c315-113">这是否为默认的内容类型</span><span class="sxs-lookup"><span data-stu-id="8c315-113">Whether this is the default Content Type</span></span>
| <span data-ttu-id="8c315-114">**position**</span><span class="sxs-lookup"><span data-stu-id="8c315-114">**position**</span></span>  | <span data-ttu-id="8c315-115">Int32</span><span class="sxs-lookup"><span data-stu-id="8c315-115">Int32</span></span>   | <span data-ttu-id="8c315-116">指定在选择 UI 中显示内容类型的位置。</span><span class="sxs-lookup"><span data-stu-id="8c315-116">Specifies the position in which the Content Type appears in the selection UI.</span></span>

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
