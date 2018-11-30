---
title: phone 资源类型
description: 表示一个电话号码。
ms.openlocfilehash: 1293b1f84d9e73f5d92c9b6f6b078b5f39126e33
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010609"
---
# <a name="phone-resource-type"></a><span data-ttu-id="49e9c-103">phone 资源类型</span><span class="sxs-lookup"><span data-stu-id="49e9c-103">phone resource type</span></span>

<span data-ttu-id="49e9c-104">表示一个电话号码。</span><span class="sxs-lookup"><span data-stu-id="49e9c-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="49e9c-105">属性</span><span class="sxs-lookup"><span data-stu-id="49e9c-105">Properties</span></span>
| <span data-ttu-id="49e9c-106">属性</span><span class="sxs-lookup"><span data-stu-id="49e9c-106">Property</span></span>     | <span data-ttu-id="49e9c-107">类型</span><span class="sxs-lookup"><span data-stu-id="49e9c-107">Type</span></span>   |<span data-ttu-id="49e9c-108">说明</span><span class="sxs-lookup"><span data-stu-id="49e9c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49e9c-109">number</span><span class="sxs-lookup"><span data-stu-id="49e9c-109">number</span></span>|<span data-ttu-id="49e9c-110">string</span><span class="sxs-lookup"><span data-stu-id="49e9c-110">string</span></span>|<span data-ttu-id="49e9c-111">电话号码。</span><span class="sxs-lookup"><span data-stu-id="49e9c-111">The phone number.</span></span>|
|<span data-ttu-id="49e9c-112">type</span><span class="sxs-lookup"><span data-stu-id="49e9c-112">type</span></span>|<span data-ttu-id="49e9c-113">phoneType</span><span class="sxs-lookup"><span data-stu-id="49e9c-113">phoneType</span></span>|<span data-ttu-id="49e9c-114">电话号码的类型。</span><span class="sxs-lookup"><span data-stu-id="49e9c-114">The type of phone number.</span></span> <span data-ttu-id="49e9c-115">可能的值为： `home`， `business`， `mobile`， `other`， `assistant`， `homeFax`， `businessFax`， `otherFax`， `pager`， `radio`。</span><span class="sxs-lookup"><span data-stu-id="49e9c-115">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="49e9c-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49e9c-116">JSON representation</span></span>

<span data-ttu-id="49e9c-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49e9c-117">Here is a JSON representation of the resource.</span></span>

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
