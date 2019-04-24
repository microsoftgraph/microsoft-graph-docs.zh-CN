---
title: educationCategory 资源类型
description: 可应用于工作分配的类别。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 928f37b4d29a4443c947bd92bf4a71f9f8a05f59
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507313"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="5ed10-103">educationCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="5ed10-103">educationCategory resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ed10-104">可应用于工作分配的类别。</span><span class="sxs-lookup"><span data-stu-id="5ed10-104">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="5ed10-105">方法</span><span class="sxs-lookup"><span data-stu-id="5ed10-105">Methods</span></span>

| <span data-ttu-id="5ed10-106">方法</span><span class="sxs-lookup"><span data-stu-id="5ed10-106">Method</span></span>           | <span data-ttu-id="5ed10-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="5ed10-107">Return Type</span></span>    |<span data-ttu-id="5ed10-108">说明</span><span class="sxs-lookup"><span data-stu-id="5ed10-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5ed10-109">获取 educationCategory</span><span class="sxs-lookup"><span data-stu-id="5ed10-109">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="5ed10-110">educationCategory</span><span class="sxs-lookup"><span data-stu-id="5ed10-110">educationCategory</span></span>](educationCategory.md) | <span data-ttu-id="5ed10-111">获取现有的**educationCategory**。</span><span class="sxs-lookup"><span data-stu-id="5ed10-111">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="5ed10-112">删除类别</span><span class="sxs-lookup"><span data-stu-id="5ed10-112">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="5ed10-113">无</span><span class="sxs-lookup"><span data-stu-id="5ed10-113">None</span></span> | <span data-ttu-id="5ed10-114">删除**educationCategory**。</span><span class="sxs-lookup"><span data-stu-id="5ed10-114">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="5ed10-115">属性</span><span class="sxs-lookup"><span data-stu-id="5ed10-115">Properties</span></span>
| <span data-ttu-id="5ed10-116">属性</span><span class="sxs-lookup"><span data-stu-id="5ed10-116">Property</span></span>     | <span data-ttu-id="5ed10-117">类型</span><span class="sxs-lookup"><span data-stu-id="5ed10-117">Type</span></span>   |<span data-ttu-id="5ed10-118">说明</span><span class="sxs-lookup"><span data-stu-id="5ed10-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ed10-119">id</span><span class="sxs-lookup"><span data-stu-id="5ed10-119">id</span></span>|<span data-ttu-id="5ed10-120">String</span><span class="sxs-lookup"><span data-stu-id="5ed10-120">String</span></span>|<span data-ttu-id="5ed10-121">类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5ed10-121">Unique identifier for the category.</span></span>|
|<span data-ttu-id="5ed10-122">displayName</span><span class="sxs-lookup"><span data-stu-id="5ed10-122">displayName</span></span>|<span data-ttu-id="5ed10-123">String</span><span class="sxs-lookup"><span data-stu-id="5ed10-123">String</span></span>|<span data-ttu-id="5ed10-124">类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5ed10-124">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ed10-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5ed10-125">JSON representation</span></span>

<span data-ttu-id="5ed10-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ed10-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCategory"
}-->

```json
{
  "id": "String (timestamp)",
  "displayName": "String (timestamp)",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationcategory.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
