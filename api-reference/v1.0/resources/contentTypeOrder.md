---
author: daspek
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
description: contentTypeOrder 资源指定在选择 UI 中显示内容类型的顺序。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e25025e86c03d7c94ed88a94ad390a56db4a44b0
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238503"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="205d6-103">ContentTypeOrder 资源类型</span><span class="sxs-lookup"><span data-stu-id="205d6-103">ContentTypeOrder resource type</span></span>

<span data-ttu-id="205d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="205d6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="205d6-105">**contentTypeOrder** 资源指定在选择 UI 中显示内容类型的顺序。</span><span class="sxs-lookup"><span data-stu-id="205d6-105">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="205d6-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="205d6-106">JSON representation</span></span>

<span data-ttu-id="205d6-107">下面是 **contentTypeOrder** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="205d6-107">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="205d6-108">属性</span><span class="sxs-lookup"><span data-stu-id="205d6-108">Properties</span></span>

| <span data-ttu-id="205d6-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="205d6-109">Property name</span></span> | <span data-ttu-id="205d6-110">类型</span><span class="sxs-lookup"><span data-stu-id="205d6-110">Type</span></span>    | <span data-ttu-id="205d6-111">说明</span><span class="sxs-lookup"><span data-stu-id="205d6-111">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="205d6-112">**default**</span><span class="sxs-lookup"><span data-stu-id="205d6-112">**default**</span></span>   | <span data-ttu-id="205d6-113">boolean</span><span class="sxs-lookup"><span data-stu-id="205d6-113">boolean</span></span> | <span data-ttu-id="205d6-114">这是否为默认的内容类型</span><span class="sxs-lookup"><span data-stu-id="205d6-114">Whether this is the default Content Type</span></span>
| <span data-ttu-id="205d6-115">**position**</span><span class="sxs-lookup"><span data-stu-id="205d6-115">**position**</span></span>  | <span data-ttu-id="205d6-116">Int32</span><span class="sxs-lookup"><span data-stu-id="205d6-116">Int32</span></span>   | <span data-ttu-id="205d6-117">指定在选择 UI 中显示内容类型的位置。</span><span class="sxs-lookup"><span data-stu-id="205d6-117">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->

