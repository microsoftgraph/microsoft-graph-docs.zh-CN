---
title: 电话资源类型
description: 表示电话号码。
localization_priority: Normal
ms.openlocfilehash: 6c34033b0895f81619589e7500441fc655842995
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462534"
---
# <a name="phone-resource-type"></a><span data-ttu-id="6c336-103">电话资源类型</span><span class="sxs-lookup"><span data-stu-id="6c336-103">phone resource type</span></span>

<span data-ttu-id="6c336-104">表示电话号码。</span><span class="sxs-lookup"><span data-stu-id="6c336-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="6c336-105">属性</span><span class="sxs-lookup"><span data-stu-id="6c336-105">Properties</span></span>
| <span data-ttu-id="6c336-106">属性</span><span class="sxs-lookup"><span data-stu-id="6c336-106">Property</span></span>     | <span data-ttu-id="6c336-107">类型</span><span class="sxs-lookup"><span data-stu-id="6c336-107">Type</span></span>   |<span data-ttu-id="6c336-108">说明</span><span class="sxs-lookup"><span data-stu-id="6c336-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c336-109">number</span><span class="sxs-lookup"><span data-stu-id="6c336-109">number</span></span>|<span data-ttu-id="6c336-110">字符串</span><span class="sxs-lookup"><span data-stu-id="6c336-110">string</span></span>|<span data-ttu-id="6c336-111">电话号码。</span><span class="sxs-lookup"><span data-stu-id="6c336-111">The phone number.</span></span>|
|<span data-ttu-id="6c336-112">类型</span><span class="sxs-lookup"><span data-stu-id="6c336-112">type</span></span>|<span data-ttu-id="6c336-113">phoneType</span><span class="sxs-lookup"><span data-stu-id="6c336-113">phoneType</span></span>|<span data-ttu-id="6c336-114">电话号码的类型。</span><span class="sxs-lookup"><span data-stu-id="6c336-114">The type of phone number.</span></span> <span data-ttu-id="6c336-115">可取值包括：`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio`。</span><span class="sxs-lookup"><span data-stu-id="6c336-115">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c336-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c336-116">JSON representation</span></span>

<span data-ttu-id="6c336-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c336-117">Here is a JSON representation of the resource.</span></span>

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
