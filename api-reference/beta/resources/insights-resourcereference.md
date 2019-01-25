---
title: resourceReference 资源类型
description: 包含属性的见解复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4fa4563904472fad9fc28fa4acb10b77887b5872
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520002"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="2a239-103">resourceReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a239-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a239-104">包含属性的[见解](insights.md)复杂类型。</span><span class="sxs-lookup"><span data-stu-id="2a239-104">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a239-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a239-105">JSON representation</span></span>

<span data-ttu-id="2a239-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a239-106">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="2a239-107">属性</span><span class="sxs-lookup"><span data-stu-id="2a239-107">Properties</span></span>

| <span data-ttu-id="2a239-108">属性</span><span class="sxs-lookup"><span data-stu-id="2a239-108">Property</span></span>      | <span data-ttu-id="2a239-109">类型</span><span class="sxs-lookup"><span data-stu-id="2a239-109">Type</span></span>      | <span data-ttu-id="2a239-110">说明</span><span class="sxs-lookup"><span data-stu-id="2a239-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="2a239-111">WebUrl</span><span class="sxs-lookup"><span data-stu-id="2a239-111">webUrl</span></span>        | <span data-ttu-id="2a239-112">String</span><span class="sxs-lookup"><span data-stu-id="2a239-112">String</span></span>    | <span data-ttu-id="2a239-113">通向引用的项的 URL。</span><span class="sxs-lookup"><span data-stu-id="2a239-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="2a239-114">id</span><span class="sxs-lookup"><span data-stu-id="2a239-114">id</span></span>            | <span data-ttu-id="2a239-115">字串符号</span><span class="sxs-lookup"><span data-stu-id="2a239-115">String</span></span>    | <span data-ttu-id="2a239-116">项目的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2a239-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="2a239-117">type</span><span class="sxs-lookup"><span data-stu-id="2a239-117">type</span></span>          | <span data-ttu-id="2a239-118">字符串</span><span class="sxs-lookup"><span data-stu-id="2a239-118">String</span></span>    | <span data-ttu-id="2a239-119">一个 string 值，可以用于分类项目，如"microsoft.graph.driveItem"</span><span class="sxs-lookup"><span data-stu-id="2a239-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcereference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
