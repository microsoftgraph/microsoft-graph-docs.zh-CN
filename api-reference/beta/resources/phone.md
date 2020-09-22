---
title: 电话资源类型
description: 表示电话号码。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: davidmu1
ms.openlocfilehash: 0e87557a3c31ef1fb8f5ebbbdd2ff29b67d8ff8c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997898"
---
# <a name="phone-resource-type"></a><span data-ttu-id="c5479-103">电话资源类型</span><span class="sxs-lookup"><span data-stu-id="c5479-103">phone resource type</span></span>

<span data-ttu-id="c5479-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5479-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5479-105">表示电话号码。</span><span class="sxs-lookup"><span data-stu-id="c5479-105">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="c5479-106">属性</span><span class="sxs-lookup"><span data-stu-id="c5479-106">Properties</span></span>
| <span data-ttu-id="c5479-107">属性</span><span class="sxs-lookup"><span data-stu-id="c5479-107">Property</span></span>     | <span data-ttu-id="c5479-108">类型</span><span class="sxs-lookup"><span data-stu-id="c5479-108">Type</span></span>   |<span data-ttu-id="c5479-109">说明</span><span class="sxs-lookup"><span data-stu-id="c5479-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5479-110">数字</span><span class="sxs-lookup"><span data-stu-id="c5479-110">number</span></span>|<span data-ttu-id="c5479-111">字符串</span><span class="sxs-lookup"><span data-stu-id="c5479-111">string</span></span>|<span data-ttu-id="c5479-112">电话号码。</span><span class="sxs-lookup"><span data-stu-id="c5479-112">The phone number.</span></span>|
|<span data-ttu-id="c5479-113">type</span><span class="sxs-lookup"><span data-stu-id="c5479-113">type</span></span>|<span data-ttu-id="c5479-114">String</span><span class="sxs-lookup"><span data-stu-id="c5479-114">String</span></span>|<span data-ttu-id="c5479-115">电话号码的类型。</span><span class="sxs-lookup"><span data-stu-id="c5479-115">The type of phone number.</span></span> <span data-ttu-id="c5479-116">可取值为：`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio`。</span><span class="sxs-lookup"><span data-stu-id="c5479-116">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c5479-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5479-117">JSON representation</span></span>

<span data-ttu-id="c5479-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5479-118">Here is a JSON representation of the resource.</span></span>

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


