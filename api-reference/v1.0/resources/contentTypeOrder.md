---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
ms.openlocfilehash: fe7309373ded16fe2660e0c5a69773c18ffb581a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="63815-102">ContentTypeOrder 资源类型</span><span class="sxs-lookup"><span data-stu-id="63815-102">ContentTypeOrder resource type</span></span>

<span data-ttu-id="63815-103">**contentTypeOrder** 资源指定 Content Type 将显示在选择 UI 中的顺序。</span><span class="sxs-lookup"><span data-stu-id="63815-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="63815-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63815-104">JSON representation</span></span>

<span data-ttu-id="63815-105">下面是 **contentTypeOrder** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63815-105">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="63815-106">属性</span><span class="sxs-lookup"><span data-stu-id="63815-106">Properties</span></span>

| <span data-ttu-id="63815-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="63815-107">Property name</span></span> | <span data-ttu-id="63815-108">类型</span><span class="sxs-lookup"><span data-stu-id="63815-108">Type</span></span>    | <span data-ttu-id="63815-109">说明</span><span class="sxs-lookup"><span data-stu-id="63815-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="63815-110">**default**</span><span class="sxs-lookup"><span data-stu-id="63815-110">**Default**</span></span>   | <span data-ttu-id="63815-111">boolean</span><span class="sxs-lookup"><span data-stu-id="63815-111">boolean</span></span> | <span data-ttu-id="63815-112">这是否为默认的内容类型</span><span class="sxs-lookup"><span data-stu-id="63815-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="63815-113">**position**</span><span class="sxs-lookup"><span data-stu-id="63815-113">**position**</span></span>  | <span data-ttu-id="63815-114">Int32</span><span class="sxs-lookup"><span data-stu-id="63815-114">Int32</span></span>   | <span data-ttu-id="63815-115">指定在选择 UI 中显示内容类型的位置。</span><span class="sxs-lookup"><span data-stu-id="63815-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
