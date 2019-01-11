---
title: phone 资源类型
description: 表示一个电话号码。
localization_priority: Normal
ms.openlocfilehash: 7397349e1fee1164d3bcde8ebc785edd9402fe75
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874177"
---
# <a name="phone-resource-type"></a><span data-ttu-id="3ceb8-103">phone 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ceb8-103">phone resource type</span></span>

> <span data-ttu-id="3ceb8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3ceb8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ceb8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3ceb8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3ceb8-106">表示一个电话号码。</span><span class="sxs-lookup"><span data-stu-id="3ceb8-106">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="3ceb8-107">属性</span><span class="sxs-lookup"><span data-stu-id="3ceb8-107">Properties</span></span>
| <span data-ttu-id="3ceb8-108">属性</span><span class="sxs-lookup"><span data-stu-id="3ceb8-108">Property</span></span>     | <span data-ttu-id="3ceb8-109">类型</span><span class="sxs-lookup"><span data-stu-id="3ceb8-109">Type</span></span>   |<span data-ttu-id="3ceb8-110">说明</span><span class="sxs-lookup"><span data-stu-id="3ceb8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ceb8-111">number</span><span class="sxs-lookup"><span data-stu-id="3ceb8-111">number</span></span>|<span data-ttu-id="3ceb8-112">string</span><span class="sxs-lookup"><span data-stu-id="3ceb8-112">string</span></span>|<span data-ttu-id="3ceb8-113">电话号码。</span><span class="sxs-lookup"><span data-stu-id="3ceb8-113">The phone number.</span></span>|
|<span data-ttu-id="3ceb8-114">type</span><span class="sxs-lookup"><span data-stu-id="3ceb8-114">type</span></span>|<span data-ttu-id="3ceb8-115">String</span><span class="sxs-lookup"><span data-stu-id="3ceb8-115">String</span></span>|<span data-ttu-id="3ceb8-p102">电话号码的类型。可能的值是：`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio`。</span><span class="sxs-lookup"><span data-stu-id="3ceb8-p102">The type of phone number. Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ceb8-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ceb8-118">JSON representation</span></span>

<span data-ttu-id="3ceb8-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ceb8-119">Here is a JSON representation of the resource.</span></span>

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
