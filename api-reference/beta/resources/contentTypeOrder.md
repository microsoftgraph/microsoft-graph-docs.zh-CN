---
author: daspek
description: contentTypeOrder 资源指定在选择 UI 中显示内容类型的顺序。
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 7198e6f17fc77c73c5b2334bc6d1e7b7262f5dcd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507441"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="d157c-103">ContentTypeOrder 资源类型</span><span class="sxs-lookup"><span data-stu-id="d157c-103">ContentTypeOrder resource type</span></span>

<span data-ttu-id="d157c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d157c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d157c-105">**contentTypeOrder** 资源指定在选择 UI 中显示内容类型的顺序。</span><span class="sxs-lookup"><span data-stu-id="d157c-105">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d157c-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d157c-106">JSON representation</span></span>

<span data-ttu-id="d157c-107">下面是 **contentTypeOrder** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d157c-107">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="d157c-108">属性</span><span class="sxs-lookup"><span data-stu-id="d157c-108">Properties</span></span>

| <span data-ttu-id="d157c-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="d157c-109">Property name</span></span> | <span data-ttu-id="d157c-110">类型</span><span class="sxs-lookup"><span data-stu-id="d157c-110">Type</span></span>    | <span data-ttu-id="d157c-111">说明</span><span class="sxs-lookup"><span data-stu-id="d157c-111">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="d157c-112">**default**</span><span class="sxs-lookup"><span data-stu-id="d157c-112">**default**</span></span>   | <span data-ttu-id="d157c-113">boolean</span><span class="sxs-lookup"><span data-stu-id="d157c-113">boolean</span></span> | <span data-ttu-id="d157c-114">这是否为默认的内容类型</span><span class="sxs-lookup"><span data-stu-id="d157c-114">Whether this is the default Content Type</span></span>
| <span data-ttu-id="d157c-115">**position**</span><span class="sxs-lookup"><span data-stu-id="d157c-115">**position**</span></span>  | <span data-ttu-id="d157c-116">Int32</span><span class="sxs-lookup"><span data-stu-id="d157c-116">Int32</span></span>   | <span data-ttu-id="d157c-117">指定在选择 UI 中显示内容类型的位置。</span><span class="sxs-lookup"><span data-stu-id="d157c-117">Specifies the position in which the Content Type appears in the selection UI.</span></span>

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
