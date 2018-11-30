---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
ms.openlocfilehash: 8cb47837d8df1c38ed25fc87d3b4d7da450fed1a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007834"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="40737-102">ContentTypeOrder 资源类型</span><span class="sxs-lookup"><span data-stu-id="40737-102">ContentTypeOrder resource type</span></span>

<span data-ttu-id="40737-103">**contentTypeOrder** 资源指定在选择 UI 中显示内容类型的顺序。</span><span class="sxs-lookup"><span data-stu-id="40737-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="40737-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40737-104">JSON representation</span></span>

<span data-ttu-id="40737-105">下面是 **contentTypeOrder** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40737-105">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="40737-106">属性</span><span class="sxs-lookup"><span data-stu-id="40737-106">Properties</span></span>

| <span data-ttu-id="40737-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="40737-107">Property name</span></span> | <span data-ttu-id="40737-108">类型</span><span class="sxs-lookup"><span data-stu-id="40737-108">Type</span></span>    | <span data-ttu-id="40737-109">说明</span><span class="sxs-lookup"><span data-stu-id="40737-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="40737-110">**default**</span><span class="sxs-lookup"><span data-stu-id="40737-110">**default**</span></span>   | <span data-ttu-id="40737-111">boolean</span><span class="sxs-lookup"><span data-stu-id="40737-111">boolean</span></span> | <span data-ttu-id="40737-112">这是否为默认的内容类型</span><span class="sxs-lookup"><span data-stu-id="40737-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="40737-113">**position**</span><span class="sxs-lookup"><span data-stu-id="40737-113">**position**</span></span>  | <span data-ttu-id="40737-114">Int32</span><span class="sxs-lookup"><span data-stu-id="40737-114">Int32</span></span>   | <span data-ttu-id="40737-115">指定在选择 UI 中显示内容类型的位置。</span><span class="sxs-lookup"><span data-stu-id="40737-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
