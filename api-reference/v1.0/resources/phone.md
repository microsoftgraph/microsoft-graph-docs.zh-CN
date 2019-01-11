---
title: phone 资源类型
description: 表示一个电话号码。
localization_priority: Normal
ms.openlocfilehash: 6c34033b0895f81619589e7500441fc655842995
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805059"
---
# <a name="phone-resource-type"></a><span data-ttu-id="d4a8a-103">phone 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4a8a-103">phone resource type</span></span>

<span data-ttu-id="d4a8a-104">表示一个电话号码。</span><span class="sxs-lookup"><span data-stu-id="d4a8a-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="d4a8a-105">属性</span><span class="sxs-lookup"><span data-stu-id="d4a8a-105">Properties</span></span>
| <span data-ttu-id="d4a8a-106">属性</span><span class="sxs-lookup"><span data-stu-id="d4a8a-106">Property</span></span>     | <span data-ttu-id="d4a8a-107">类型</span><span class="sxs-lookup"><span data-stu-id="d4a8a-107">Type</span></span>   |<span data-ttu-id="d4a8a-108">说明</span><span class="sxs-lookup"><span data-stu-id="d4a8a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4a8a-109">number</span><span class="sxs-lookup"><span data-stu-id="d4a8a-109">number</span></span>|<span data-ttu-id="d4a8a-110">string</span><span class="sxs-lookup"><span data-stu-id="d4a8a-110">string</span></span>|<span data-ttu-id="d4a8a-111">电话号码。</span><span class="sxs-lookup"><span data-stu-id="d4a8a-111">The phone number.</span></span>|
|<span data-ttu-id="d4a8a-112">type</span><span class="sxs-lookup"><span data-stu-id="d4a8a-112">type</span></span>|<span data-ttu-id="d4a8a-113">phoneType</span><span class="sxs-lookup"><span data-stu-id="d4a8a-113">phoneType</span></span>|<span data-ttu-id="d4a8a-114">电话号码的类型。</span><span class="sxs-lookup"><span data-stu-id="d4a8a-114">The type of phone number.</span></span> <span data-ttu-id="d4a8a-115">可能的值为： `home`， `business`， `mobile`， `other`， `assistant`， `homeFax`， `businessFax`， `otherFax`， `pager`， `radio`。</span><span class="sxs-lookup"><span data-stu-id="d4a8a-115">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4a8a-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4a8a-116">JSON representation</span></span>

<span data-ttu-id="d4a8a-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4a8a-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phone"
}-->

```json
{
  "number": "string",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
