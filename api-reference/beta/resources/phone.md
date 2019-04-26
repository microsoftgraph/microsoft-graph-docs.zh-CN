---
title: 电话资源类型
description: 表示电话号码。
localization_priority: Normal
ms.openlocfilehash: 643b146f95fcc85be530ce7907c872f56033240e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344952"
---
# <a name="phone-resource-type"></a><span data-ttu-id="7cc87-103">电话资源类型</span><span class="sxs-lookup"><span data-stu-id="7cc87-103">phone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cc87-104">表示电话号码。</span><span class="sxs-lookup"><span data-stu-id="7cc87-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="7cc87-105">属性</span><span class="sxs-lookup"><span data-stu-id="7cc87-105">Properties</span></span>
| <span data-ttu-id="7cc87-106">属性</span><span class="sxs-lookup"><span data-stu-id="7cc87-106">Property</span></span>     | <span data-ttu-id="7cc87-107">类型</span><span class="sxs-lookup"><span data-stu-id="7cc87-107">Type</span></span>   |<span data-ttu-id="7cc87-108">说明</span><span class="sxs-lookup"><span data-stu-id="7cc87-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7cc87-109">数字</span><span class="sxs-lookup"><span data-stu-id="7cc87-109">number</span></span>|<span data-ttu-id="7cc87-110">string</span><span class="sxs-lookup"><span data-stu-id="7cc87-110">string</span></span>|<span data-ttu-id="7cc87-111">电话号码。</span><span class="sxs-lookup"><span data-stu-id="7cc87-111">The phone number.</span></span>|
|<span data-ttu-id="7cc87-112">type</span><span class="sxs-lookup"><span data-stu-id="7cc87-112">type</span></span>|<span data-ttu-id="7cc87-113">String</span><span class="sxs-lookup"><span data-stu-id="7cc87-113">String</span></span>|<span data-ttu-id="7cc87-114">电话号码的类型。</span><span class="sxs-lookup"><span data-stu-id="7cc87-114">The type of phone number.</span></span> <span data-ttu-id="7cc87-115">可取值为：`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio`。</span><span class="sxs-lookup"><span data-stu-id="7cc87-115">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7cc87-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7cc87-116">JSON representation</span></span>

<span data-ttu-id="7cc87-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7cc87-117">Here is a JSON representation of the resource.</span></span>

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
