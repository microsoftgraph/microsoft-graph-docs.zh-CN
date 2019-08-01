---
title: 电话资源类型
description: 表示电话号码。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6bdcc4331b14ad7a0e03404781014b66daf55b46
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035474"
---
# <a name="phone-resource-type"></a><span data-ttu-id="1242b-103">电话资源类型</span><span class="sxs-lookup"><span data-stu-id="1242b-103">phone resource type</span></span>

<span data-ttu-id="1242b-104">表示电话号码。</span><span class="sxs-lookup"><span data-stu-id="1242b-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="1242b-105">属性</span><span class="sxs-lookup"><span data-stu-id="1242b-105">Properties</span></span>
| <span data-ttu-id="1242b-106">属性</span><span class="sxs-lookup"><span data-stu-id="1242b-106">Property</span></span>     | <span data-ttu-id="1242b-107">类型</span><span class="sxs-lookup"><span data-stu-id="1242b-107">Type</span></span>   |<span data-ttu-id="1242b-108">说明</span><span class="sxs-lookup"><span data-stu-id="1242b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1242b-109">number</span><span class="sxs-lookup"><span data-stu-id="1242b-109">number</span></span>|<span data-ttu-id="1242b-110">string</span><span class="sxs-lookup"><span data-stu-id="1242b-110">string</span></span>|<span data-ttu-id="1242b-111">电话号码。</span><span class="sxs-lookup"><span data-stu-id="1242b-111">The phone number.</span></span>|
|<span data-ttu-id="1242b-112">type</span><span class="sxs-lookup"><span data-stu-id="1242b-112">type</span></span>|<span data-ttu-id="1242b-113">phoneType</span><span class="sxs-lookup"><span data-stu-id="1242b-113">phoneType</span></span>|<span data-ttu-id="1242b-114">电话号码的类型。</span><span class="sxs-lookup"><span data-stu-id="1242b-114">The type of phone number.</span></span> <span data-ttu-id="1242b-115">可取值包括：`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio`。</span><span class="sxs-lookup"><span data-stu-id="1242b-115">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1242b-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1242b-116">JSON representation</span></span>

<span data-ttu-id="1242b-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1242b-117">Here is a JSON representation of the resource.</span></span>

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
