---
title: 电话资源类型
description: 表示电话号码。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ca2c81531aa5bf53c8038fe7e095f056c4682eba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521888"
---
# <a name="phone-resource-type"></a><span data-ttu-id="19da6-103">电话资源类型</span><span class="sxs-lookup"><span data-stu-id="19da6-103">phone resource type</span></span>

<span data-ttu-id="19da6-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="19da6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19da6-105">表示电话号码。</span><span class="sxs-lookup"><span data-stu-id="19da6-105">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="19da6-106">属性</span><span class="sxs-lookup"><span data-stu-id="19da6-106">Properties</span></span>
| <span data-ttu-id="19da6-107">属性</span><span class="sxs-lookup"><span data-stu-id="19da6-107">Property</span></span>     | <span data-ttu-id="19da6-108">类型</span><span class="sxs-lookup"><span data-stu-id="19da6-108">Type</span></span>   |<span data-ttu-id="19da6-109">说明</span><span class="sxs-lookup"><span data-stu-id="19da6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19da6-110">number</span><span class="sxs-lookup"><span data-stu-id="19da6-110">number</span></span>|<span data-ttu-id="19da6-111">string</span><span class="sxs-lookup"><span data-stu-id="19da6-111">string</span></span>|<span data-ttu-id="19da6-112">电话号码。</span><span class="sxs-lookup"><span data-stu-id="19da6-112">The phone number.</span></span>|
|<span data-ttu-id="19da6-113">type</span><span class="sxs-lookup"><span data-stu-id="19da6-113">type</span></span>|<span data-ttu-id="19da6-114">String</span><span class="sxs-lookup"><span data-stu-id="19da6-114">String</span></span>|<span data-ttu-id="19da6-115">电话号码的类型。</span><span class="sxs-lookup"><span data-stu-id="19da6-115">The type of phone number.</span></span> <span data-ttu-id="19da6-116">可取值为：`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio`。</span><span class="sxs-lookup"><span data-stu-id="19da6-116">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="19da6-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19da6-117">JSON representation</span></span>

<span data-ttu-id="19da6-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19da6-118">Here is a JSON representation of the resource.</span></span>

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
