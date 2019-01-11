---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
ms.openlocfilehash: ad25ececa9a32a1aaab7f25bf909f7e1ef640dec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825751"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="f2217-102">ContentTypeOrder 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2217-102">ContentTypeOrder resource type</span></span>

> <span data-ttu-id="f2217-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f2217-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2217-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f2217-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2217-105">**contentTypeOrder** 资源指定在选择 UI 中显示内容类型的顺序。</span><span class="sxs-lookup"><span data-stu-id="f2217-105">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2217-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2217-106">JSON representation</span></span>

<span data-ttu-id="f2217-107">下面是 **contentTypeOrder** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2217-107">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="f2217-108">属性</span><span class="sxs-lookup"><span data-stu-id="f2217-108">Properties</span></span>

| <span data-ttu-id="f2217-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="f2217-109">Property name</span></span> | <span data-ttu-id="f2217-110">类型</span><span class="sxs-lookup"><span data-stu-id="f2217-110">Type</span></span>    | <span data-ttu-id="f2217-111">说明</span><span class="sxs-lookup"><span data-stu-id="f2217-111">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="f2217-112">**default**</span><span class="sxs-lookup"><span data-stu-id="f2217-112">**default**</span></span>   | <span data-ttu-id="f2217-113">boolean</span><span class="sxs-lookup"><span data-stu-id="f2217-113">boolean</span></span> | <span data-ttu-id="f2217-114">这是否为默认的内容类型</span><span class="sxs-lookup"><span data-stu-id="f2217-114">Whether this is the default Content Type</span></span>
| <span data-ttu-id="f2217-115">**position**</span><span class="sxs-lookup"><span data-stu-id="f2217-115">**position**</span></span>  | <span data-ttu-id="f2217-116">Int32</span><span class="sxs-lookup"><span data-stu-id="f2217-116">Int32</span></span>   | <span data-ttu-id="f2217-117">指定在选择 UI 中显示内容类型的位置。</span><span class="sxs-lookup"><span data-stu-id="f2217-117">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
