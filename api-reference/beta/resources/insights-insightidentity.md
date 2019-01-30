---
title: insightIdentity
description: 包含共享项目的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 45ac8874a30ebb4f3196f03a675229bf1fab750c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643886"
---
# <a name="insightidentity"></a><span data-ttu-id="c4fc6-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="c4fc6-103">insightIdentity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4fc6-104">包含[共享](insights-shared.md)项目的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="c4fc6-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="c4fc6-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c4fc6-105">JSON representation</span></span>
<span data-ttu-id="c4fc6-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4fc6-106">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="c4fc6-107">属性</span><span class="sxs-lookup"><span data-stu-id="c4fc6-107">Properties</span></span>

| <span data-ttu-id="c4fc6-108">属性</span><span class="sxs-lookup"><span data-stu-id="c4fc6-108">Property</span></span>              | <span data-ttu-id="c4fc6-109">类型</span><span class="sxs-lookup"><span data-stu-id="c4fc6-109">Type</span></span>          | <span data-ttu-id="c4fc6-110">说明</span><span class="sxs-lookup"><span data-stu-id="c4fc6-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="c4fc6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c4fc6-111">displayName</span></span>       | <span data-ttu-id="c4fc6-112">String</span><span class="sxs-lookup"><span data-stu-id="c4fc6-112">String</span></span>          | <span data-ttu-id="c4fc6-113">共享项目的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c4fc6-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="c4fc6-114">id</span><span class="sxs-lookup"><span data-stu-id="c4fc6-114">id</span></span>              | <span data-ttu-id="c4fc6-115">String</span><span class="sxs-lookup"><span data-stu-id="c4fc6-115">String</span></span>        | <span data-ttu-id="c4fc6-116">共享项目的用户的 id。</span><span class="sxs-lookup"><span data-stu-id="c4fc6-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="c4fc6-117">address</span><span class="sxs-lookup"><span data-stu-id="c4fc6-117">address</span></span>             | <span data-ttu-id="c4fc6-118">String</span><span class="sxs-lookup"><span data-stu-id="c4fc6-118">String</span></span>      | <span data-ttu-id="c4fc6-119">共享项目的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="c4fc6-119">The email address of the user who shared the item.</span></span>  |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-insightidentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
