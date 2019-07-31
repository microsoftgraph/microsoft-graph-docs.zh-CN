---
author: daspek
description: contentTypeInfo 资源指示项的 SharePoint 内容类型。
ms.date: 09/12/2017
title: ContentTypeInfo
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 04316b01c905acb4fe38923f8d664ea892773e8e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012847"
---
# <a name="contenttypeinfo-resource-type"></a><span data-ttu-id="c5ae3-103">ContentTypeInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="c5ae3-103">ContentTypeInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5ae3-104">**contentTypeInfo** 资源指示项的 SharePoint 内容类型。</span><span class="sxs-lookup"><span data-stu-id="c5ae3-104">The **contentTypeInfo** resource indicates the SharePoint content type of an item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5ae3-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5ae3-105">JSON representation</span></span>

<span data-ttu-id="c5ae3-106">下面是 **contentTypeInfo** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5ae3-106">Here is a JSON representation of a **contentTypeInfo** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="c5ae3-107">属性</span><span class="sxs-lookup"><span data-stu-id="c5ae3-107">Properties</span></span>

| <span data-ttu-id="c5ae3-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="c5ae3-108">Property name</span></span>  | <span data-ttu-id="c5ae3-109">类型</span><span class="sxs-lookup"><span data-stu-id="c5ae3-109">Type</span></span>    | <span data-ttu-id="c5ae3-110">说明</span><span class="sxs-lookup"><span data-stu-id="c5ae3-110">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="c5ae3-111">**id**</span><span class="sxs-lookup"><span data-stu-id="c5ae3-111">**id**</span></span>         | <span data-ttu-id="c5ae3-112">string</span><span class="sxs-lookup"><span data-stu-id="c5ae3-112">string</span></span>  | <span data-ttu-id="c5ae3-113">内容类型的 ID。</span><span class="sxs-lookup"><span data-stu-id="c5ae3-113">The id of the content type.</span></span>
| <span data-ttu-id="c5ae3-114">**name**</span><span class="sxs-lookup"><span data-stu-id="c5ae3-114">**name**</span></span>       | <span data-ttu-id="c5ae3-115">string</span><span class="sxs-lookup"><span data-stu-id="c5ae3-115">string</span></span>  | <span data-ttu-id="c5ae3-116">内容类型的名称。</span><span class="sxs-lookup"><span data-stu-id="c5ae3-116">The name of the content type.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo",
  "suppressions": []
}
-->
