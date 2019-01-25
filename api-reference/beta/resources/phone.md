---
title: phone 资源类型
description: 表示一个电话号码。
localization_priority: Normal
ms.openlocfilehash: a343d4e1d65126048a27ad723c86ae49eb2ed752
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527227"
---
# <a name="phone-resource-type"></a><span data-ttu-id="be605-103">phone 资源类型</span><span class="sxs-lookup"><span data-stu-id="be605-103">phone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be605-104">表示一个电话号码。</span><span class="sxs-lookup"><span data-stu-id="be605-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="be605-105">属性</span><span class="sxs-lookup"><span data-stu-id="be605-105">Properties</span></span>
| <span data-ttu-id="be605-106">属性</span><span class="sxs-lookup"><span data-stu-id="be605-106">Property</span></span>     | <span data-ttu-id="be605-107">类型</span><span class="sxs-lookup"><span data-stu-id="be605-107">Type</span></span>   |<span data-ttu-id="be605-108">说明</span><span class="sxs-lookup"><span data-stu-id="be605-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be605-109">number</span><span class="sxs-lookup"><span data-stu-id="be605-109">number</span></span>|<span data-ttu-id="be605-110">string</span><span class="sxs-lookup"><span data-stu-id="be605-110">string</span></span>|<span data-ttu-id="be605-111">电话号码。</span><span class="sxs-lookup"><span data-stu-id="be605-111">The phone number.</span></span>|
|<span data-ttu-id="be605-112">type</span><span class="sxs-lookup"><span data-stu-id="be605-112">type</span></span>|<span data-ttu-id="be605-113">String</span><span class="sxs-lookup"><span data-stu-id="be605-113">String</span></span>|<span data-ttu-id="be605-p101">电话号码的类型。可能的值是：`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio`。</span><span class="sxs-lookup"><span data-stu-id="be605-p101">The type of phone number. Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be605-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be605-116">JSON representation</span></span>

<span data-ttu-id="be605-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be605-117">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/phone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
