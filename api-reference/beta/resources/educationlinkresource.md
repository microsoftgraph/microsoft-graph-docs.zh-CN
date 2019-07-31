---
title: educationLinkResource 资源类型
description: EducationResource 的子类。 此资源是链接, 不具有与之关联的任何其他数据。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 58558ba55846614ce0bf0d08614faab34e4989af
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972654"
---
# <a name="educationlinkresource-resource-type"></a><span data-ttu-id="aa8fc-104">educationLinkResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa8fc-104">educationLinkResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa8fc-105">[EducationResource](educationresource.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="aa8fc-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="aa8fc-106">此资源是链接, 不具有与之关联的任何其他数据。</span><span class="sxs-lookup"><span data-stu-id="aa8fc-106">This resource is a link and does not have any additional data associated with it.</span></span>


## <a name="properties"></a><span data-ttu-id="aa8fc-107">属性</span><span class="sxs-lookup"><span data-stu-id="aa8fc-107">Properties</span></span>
| <span data-ttu-id="aa8fc-108">属性</span><span class="sxs-lookup"><span data-stu-id="aa8fc-108">Property</span></span>     | <span data-ttu-id="aa8fc-109">类型</span><span class="sxs-lookup"><span data-stu-id="aa8fc-109">Type</span></span>   |<span data-ttu-id="aa8fc-110">说明</span><span class="sxs-lookup"><span data-stu-id="aa8fc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa8fc-111">link</span><span class="sxs-lookup"><span data-stu-id="aa8fc-111">link</span></span>|<span data-ttu-id="aa8fc-112">String</span><span class="sxs-lookup"><span data-stu-id="aa8fc-112">String</span></span>|<span data-ttu-id="aa8fc-113">指向资源的 URL。</span><span class="sxs-lookup"><span data-stu-id="aa8fc-113">URL to the resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa8fc-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa8fc-114">JSON representation</span></span>

<span data-ttu-id="aa8fc-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa8fc-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationLinkResource"
}-->

```json
{
  "link": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationLinkResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
