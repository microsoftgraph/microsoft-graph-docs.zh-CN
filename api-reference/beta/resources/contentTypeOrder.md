---
author: daspek
description: contentTypeOrder 资源指定在选择 UI 中显示内容类型的顺序。
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e7adde2a0452e9fe13a8f547eeec6fed957460da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998899"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="d2f68-103">ContentTypeOrder 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2f68-103">ContentTypeOrder resource type</span></span>

<span data-ttu-id="d2f68-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2f68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2f68-105">**contentTypeOrder** 资源指定在选择 UI 中显示内容类型的顺序。</span><span class="sxs-lookup"><span data-stu-id="d2f68-105">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2f68-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2f68-106">JSON representation</span></span>

<span data-ttu-id="d2f68-107">下面是 **contentTypeOrder** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2f68-107">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="d2f68-108">属性</span><span class="sxs-lookup"><span data-stu-id="d2f68-108">Properties</span></span>

| <span data-ttu-id="d2f68-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="d2f68-109">Property name</span></span> | <span data-ttu-id="d2f68-110">类型</span><span class="sxs-lookup"><span data-stu-id="d2f68-110">Type</span></span>    | <span data-ttu-id="d2f68-111">说明</span><span class="sxs-lookup"><span data-stu-id="d2f68-111">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="d2f68-112">**default**</span><span class="sxs-lookup"><span data-stu-id="d2f68-112">**default**</span></span>   | <span data-ttu-id="d2f68-113">boolean</span><span class="sxs-lookup"><span data-stu-id="d2f68-113">boolean</span></span> | <span data-ttu-id="d2f68-114">这是否为默认的内容类型</span><span class="sxs-lookup"><span data-stu-id="d2f68-114">Whether this is the default Content Type</span></span>
| <span data-ttu-id="d2f68-115">**position**</span><span class="sxs-lookup"><span data-stu-id="d2f68-115">**position**</span></span>  | <span data-ttu-id="d2f68-116">Int32</span><span class="sxs-lookup"><span data-stu-id="d2f68-116">Int32</span></span>   | <span data-ttu-id="d2f68-117">指定在选择 UI 中显示内容类型的位置。</span><span class="sxs-lookup"><span data-stu-id="d2f68-117">Specifies the position in which the Content Type appears in the selection UI.</span></span>

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


