---
title: resourceReference 资源类型
description: 包含属性的见解复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 8cc7e686aebd531a25b6c1637fcf99338df09396
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572295"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="6abe9-103">resourceReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="6abe9-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6abe9-104">包含属性的[见解](insights.md)复杂类型。</span><span class="sxs-lookup"><span data-stu-id="6abe9-104">Complex type containing properties of [insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="6abe9-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6abe9-105">JSON representation</span></span>

<span data-ttu-id="6abe9-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6abe9-106">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueLegacyExtendedProperty",
    "multiValueLegacyExtendedProperty"
  ],
  "@odata.type": "microsoft.graph.resourceReference"
}-->
```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="6abe9-107">属性</span><span class="sxs-lookup"><span data-stu-id="6abe9-107">Properties</span></span>

| <span data-ttu-id="6abe9-108">属性</span><span class="sxs-lookup"><span data-stu-id="6abe9-108">Property</span></span>      | <span data-ttu-id="6abe9-109">类型</span><span class="sxs-lookup"><span data-stu-id="6abe9-109">Type</span></span>      | <span data-ttu-id="6abe9-110">说明</span><span class="sxs-lookup"><span data-stu-id="6abe9-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="6abe9-111">WebUrl</span><span class="sxs-lookup"><span data-stu-id="6abe9-111">webUrl</span></span>        | <span data-ttu-id="6abe9-112">String</span><span class="sxs-lookup"><span data-stu-id="6abe9-112">String</span></span>    | <span data-ttu-id="6abe9-113">通向引用的项的 URL。</span><span class="sxs-lookup"><span data-stu-id="6abe9-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="6abe9-114">id</span><span class="sxs-lookup"><span data-stu-id="6abe9-114">id</span></span>            | <span data-ttu-id="6abe9-115">String</span><span class="sxs-lookup"><span data-stu-id="6abe9-115">String</span></span>    | <span data-ttu-id="6abe9-116">项目的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6abe9-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="6abe9-117">type</span><span class="sxs-lookup"><span data-stu-id="6abe9-117">type</span></span>          | <span data-ttu-id="6abe9-118">String</span><span class="sxs-lookup"><span data-stu-id="6abe9-118">String</span></span>    | <span data-ttu-id="6abe9-119">一个 string 值，可以用于分类项目，如"microsoft.graph.driveItem"</span><span class="sxs-lookup"><span data-stu-id="6abe9-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcereference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
