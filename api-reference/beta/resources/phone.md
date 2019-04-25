---
title: 电话资源类型
description: 表示电话号码。
localization_priority: Normal
ms.openlocfilehash: a343d4e1d65126048a27ad723c86ae49eb2ed752
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573765"
---
# <a name="phone-resource-type"></a><span data-ttu-id="ac2cb-103">电话资源类型</span><span class="sxs-lookup"><span data-stu-id="ac2cb-103">phone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac2cb-104">表示电话号码。</span><span class="sxs-lookup"><span data-stu-id="ac2cb-104">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="ac2cb-105">属性</span><span class="sxs-lookup"><span data-stu-id="ac2cb-105">Properties</span></span>
| <span data-ttu-id="ac2cb-106">属性</span><span class="sxs-lookup"><span data-stu-id="ac2cb-106">Property</span></span>     | <span data-ttu-id="ac2cb-107">类型</span><span class="sxs-lookup"><span data-stu-id="ac2cb-107">Type</span></span>   |<span data-ttu-id="ac2cb-108">说明</span><span class="sxs-lookup"><span data-stu-id="ac2cb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac2cb-109">数字</span><span class="sxs-lookup"><span data-stu-id="ac2cb-109">number</span></span>|<span data-ttu-id="ac2cb-110">string</span><span class="sxs-lookup"><span data-stu-id="ac2cb-110">string</span></span>|<span data-ttu-id="ac2cb-111">电话号码。</span><span class="sxs-lookup"><span data-stu-id="ac2cb-111">The phone number.</span></span>|
|<span data-ttu-id="ac2cb-112">type</span><span class="sxs-lookup"><span data-stu-id="ac2cb-112">type</span></span>|<span data-ttu-id="ac2cb-113">String</span><span class="sxs-lookup"><span data-stu-id="ac2cb-113">String</span></span>|<span data-ttu-id="ac2cb-114">电话号码的类型。</span><span class="sxs-lookup"><span data-stu-id="ac2cb-114">The type of phone number.</span></span> <span data-ttu-id="ac2cb-115">可取值为：`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio`。</span><span class="sxs-lookup"><span data-stu-id="ac2cb-115">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac2cb-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ac2cb-116">JSON representation</span></span>

<span data-ttu-id="ac2cb-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac2cb-117">Here is a JSON representation of the resource.</span></span>

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
