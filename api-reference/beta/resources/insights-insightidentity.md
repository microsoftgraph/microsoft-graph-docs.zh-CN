---
title: insightIdentity
description: 包含共享项目的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 47283a82260d4f03a271a16660d58aca60da94e1
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577224"
---
# <a name="insightidentity"></a><span data-ttu-id="9aa00-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="9aa00-103">insightIdentity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9aa00-104">包含[共享](insights-shared.md)项目的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="9aa00-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="9aa00-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9aa00-105">JSON representation</span></span>
<span data-ttu-id="9aa00-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9aa00-106">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueLegacyExtendedProperty",
    "multiValueLegacyExtendedProperty"
  ],
  "@odata.type": "microsoft.graph.insightIdentity"
}-->
```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="9aa00-107">属性</span><span class="sxs-lookup"><span data-stu-id="9aa00-107">Properties</span></span>

| <span data-ttu-id="9aa00-108">属性</span><span class="sxs-lookup"><span data-stu-id="9aa00-108">Property</span></span>              | <span data-ttu-id="9aa00-109">类型</span><span class="sxs-lookup"><span data-stu-id="9aa00-109">Type</span></span>          | <span data-ttu-id="9aa00-110">说明</span><span class="sxs-lookup"><span data-stu-id="9aa00-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="9aa00-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9aa00-111">displayName</span></span>       | <span data-ttu-id="9aa00-112">String</span><span class="sxs-lookup"><span data-stu-id="9aa00-112">String</span></span>          | <span data-ttu-id="9aa00-113">共享项目的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9aa00-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="9aa00-114">id</span><span class="sxs-lookup"><span data-stu-id="9aa00-114">id</span></span>              | <span data-ttu-id="9aa00-115">String</span><span class="sxs-lookup"><span data-stu-id="9aa00-115">String</span></span>        | <span data-ttu-id="9aa00-116">共享项目的用户的 id。</span><span class="sxs-lookup"><span data-stu-id="9aa00-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="9aa00-117">address</span><span class="sxs-lookup"><span data-stu-id="9aa00-117">address</span></span>             | <span data-ttu-id="9aa00-118">String</span><span class="sxs-lookup"><span data-stu-id="9aa00-118">String</span></span>      | <span data-ttu-id="9aa00-119">共享项目的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="9aa00-119">The email address of the user who shared the item.</span></span>  |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-insightidentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
