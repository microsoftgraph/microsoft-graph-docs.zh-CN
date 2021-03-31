---
title: 电话资源类型
description: 表示电话号码。
localization_priority: Normal
author: Jumaodhiss
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6740d1cd1746151d35f7627d9ab5125724adc3f0
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469232"
---
# <a name="phone-resource-type"></a><span data-ttu-id="f8780-103">电话资源类型</span><span class="sxs-lookup"><span data-stu-id="f8780-103">phone resource type</span></span>

<span data-ttu-id="f8780-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8780-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f8780-105">表示电话号码。</span><span class="sxs-lookup"><span data-stu-id="f8780-105">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="f8780-106">属性</span><span class="sxs-lookup"><span data-stu-id="f8780-106">Properties</span></span>
| <span data-ttu-id="f8780-107">属性</span><span class="sxs-lookup"><span data-stu-id="f8780-107">Property</span></span>     | <span data-ttu-id="f8780-108">类型</span><span class="sxs-lookup"><span data-stu-id="f8780-108">Type</span></span>   |<span data-ttu-id="f8780-109">说明</span><span class="sxs-lookup"><span data-stu-id="f8780-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8780-110">number</span><span class="sxs-lookup"><span data-stu-id="f8780-110">number</span></span>|<span data-ttu-id="f8780-111">string</span><span class="sxs-lookup"><span data-stu-id="f8780-111">string</span></span>|<span data-ttu-id="f8780-112">电话号码。</span><span class="sxs-lookup"><span data-stu-id="f8780-112">The phone number.</span></span>|
|<span data-ttu-id="f8780-113">type</span><span class="sxs-lookup"><span data-stu-id="f8780-113">type</span></span>|<span data-ttu-id="f8780-114">phoneType</span><span class="sxs-lookup"><span data-stu-id="f8780-114">phoneType</span></span>|<span data-ttu-id="f8780-115">电话号码的类型。</span><span class="sxs-lookup"><span data-stu-id="f8780-115">The type of phone number.</span></span> <span data-ttu-id="f8780-116">可取值包括：`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio`。</span><span class="sxs-lookup"><span data-stu-id="f8780-116">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f8780-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8780-117">JSON representation</span></span>

<span data-ttu-id="f8780-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8780-118">Here is a JSON representation of the resource.</span></span>

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

