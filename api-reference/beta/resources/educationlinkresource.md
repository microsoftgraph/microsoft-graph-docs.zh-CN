---
title: educationLinkResource 资源类型
description: educationResource 的子类。 此资源是链接, 不具有与之关联的任何其他数据。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: cd6e2d05fec5bebc00545947023a7ebc7c7150a1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334231"
---
# <a name="educationlinkresource-resource-type"></a><span data-ttu-id="4cc61-104">educationLinkResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="4cc61-104">educationLinkResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cc61-105">[educationResource](educationresource.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="4cc61-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="4cc61-106">此资源是链接, 不具有与之关联的任何其他数据。</span><span class="sxs-lookup"><span data-stu-id="4cc61-106">This resource is a link and does not have any additional data associated with it.</span></span>


## <a name="properties"></a><span data-ttu-id="4cc61-107">属性</span><span class="sxs-lookup"><span data-stu-id="4cc61-107">Properties</span></span>
| <span data-ttu-id="4cc61-108">属性</span><span class="sxs-lookup"><span data-stu-id="4cc61-108">Property</span></span>     | <span data-ttu-id="4cc61-109">类型</span><span class="sxs-lookup"><span data-stu-id="4cc61-109">Type</span></span>   |<span data-ttu-id="4cc61-110">说明</span><span class="sxs-lookup"><span data-stu-id="4cc61-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4cc61-111">link</span><span class="sxs-lookup"><span data-stu-id="4cc61-111">link</span></span>|<span data-ttu-id="4cc61-112">String</span><span class="sxs-lookup"><span data-stu-id="4cc61-112">String</span></span>|<span data-ttu-id="4cc61-113">指向资源的 URL。</span><span class="sxs-lookup"><span data-stu-id="4cc61-113">URL to the resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4cc61-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4cc61-114">JSON representation</span></span>

<span data-ttu-id="4cc61-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4cc61-115">The following is a JSON representation of the resource.</span></span>

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
