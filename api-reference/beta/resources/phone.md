---
title: 电话资源类型
description: 表示电话号码。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: davidmu1
ms.openlocfilehash: 162d6a0ccb927c6a48dc01dc3d1e716ab949d89d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812048"
---
# <a name="phone-resource-type"></a><span data-ttu-id="5147e-103">电话资源类型</span><span class="sxs-lookup"><span data-stu-id="5147e-103">phone resource type</span></span>

<span data-ttu-id="5147e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5147e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5147e-105">表示电话号码。</span><span class="sxs-lookup"><span data-stu-id="5147e-105">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="5147e-106">属性</span><span class="sxs-lookup"><span data-stu-id="5147e-106">Properties</span></span>
| <span data-ttu-id="5147e-107">属性</span><span class="sxs-lookup"><span data-stu-id="5147e-107">Property</span></span>     | <span data-ttu-id="5147e-108">类型</span><span class="sxs-lookup"><span data-stu-id="5147e-108">Type</span></span>   |<span data-ttu-id="5147e-109">说明</span><span class="sxs-lookup"><span data-stu-id="5147e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5147e-110">数字</span><span class="sxs-lookup"><span data-stu-id="5147e-110">number</span></span>|<span data-ttu-id="5147e-111">string</span><span class="sxs-lookup"><span data-stu-id="5147e-111">string</span></span>|<span data-ttu-id="5147e-112">电话号码。</span><span class="sxs-lookup"><span data-stu-id="5147e-112">The phone number.</span></span>|
|<span data-ttu-id="5147e-113">type</span><span class="sxs-lookup"><span data-stu-id="5147e-113">type</span></span>|<span data-ttu-id="5147e-114">String</span><span class="sxs-lookup"><span data-stu-id="5147e-114">String</span></span>|<span data-ttu-id="5147e-115">电话号码的类型。</span><span class="sxs-lookup"><span data-stu-id="5147e-115">The type of phone number.</span></span> <span data-ttu-id="5147e-116">可取值为：`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio`。</span><span class="sxs-lookup"><span data-stu-id="5147e-116">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5147e-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5147e-117">JSON representation</span></span>

<span data-ttu-id="5147e-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5147e-118">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
