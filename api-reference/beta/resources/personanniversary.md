---
title: personAnniversary 资源类型
description: personAnniversary 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 1ad4c5a1792ee0e75a31f165b0a8eebf6f0d2130
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2019
ms.locfileid: "37949515"
---
# <a name="personanniversary-resource-type"></a><span data-ttu-id="97972-103">personAnniversary 资源类型</span><span class="sxs-lookup"><span data-stu-id="97972-103">personAnniversary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97972-104">表示与用户[配置文件](profile.md)中的人员关联的有意义日期的详细信息。</span><span class="sxs-lookup"><span data-stu-id="97972-104">Represents the details of meaningful dates associated with a person in a user's [profile](profile.md).</span></span>

<span data-ttu-id="97972-105">继承自[itemFacet](itemFacet.md)。</span><span class="sxs-lookup"><span data-stu-id="97972-105">Inherits from [itemFacet](itemFacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="97972-106">方法</span><span class="sxs-lookup"><span data-stu-id="97972-106">Methods</span></span>

| <span data-ttu-id="97972-107">方法</span><span class="sxs-lookup"><span data-stu-id="97972-107">Method</span></span>                                                   | <span data-ttu-id="97972-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="97972-108">Return Type</span></span>                               | <span data-ttu-id="97972-109">说明</span><span class="sxs-lookup"><span data-stu-id="97972-109">Description</span></span>                                                    |
|:---------------------------------------------------------|:------------------------------------------|:---------------------------------------------------------------|
| [<span data-ttu-id="97972-110">获取 personAnniversary</span><span class="sxs-lookup"><span data-stu-id="97972-110">Get personAnniversary</span></span>](../api/personanniversary-get.md) | [<span data-ttu-id="97972-111">personAnniversary</span><span class="sxs-lookup"><span data-stu-id="97972-111">personAnniversary</span></span>](personanniversary.md) | <span data-ttu-id="97972-112">读取**personAnniversary**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="97972-112">Read the properties and relationships of a **personAnniversary** object.</span></span> |
| [<span data-ttu-id="97972-113">Update</span><span class="sxs-lookup"><span data-stu-id="97972-113">Update</span></span>](../api/personanniversary-update.md)             | [<span data-ttu-id="97972-114">personAnniversary</span><span class="sxs-lookup"><span data-stu-id="97972-114">personAnniversary</span></span>](personanniversary.md) | <span data-ttu-id="97972-115">更新**personAnniversary**对象。</span><span class="sxs-lookup"><span data-stu-id="97972-115">Update a **personAnniversary** object.</span></span>                               |
| [<span data-ttu-id="97972-116">删除</span><span class="sxs-lookup"><span data-stu-id="97972-116">Delete</span></span>](../api/personanniversary-delete.md)             | <span data-ttu-id="97972-117">无</span><span class="sxs-lookup"><span data-stu-id="97972-117">None</span></span>                                      | <span data-ttu-id="97972-118">删除**personAnniversary**对象。</span><span class="sxs-lookup"><span data-stu-id="97972-118">Delete a **personAnniversary** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="97972-119">属性</span><span class="sxs-lookup"><span data-stu-id="97972-119">Properties</span></span>

| <span data-ttu-id="97972-120">属性</span><span class="sxs-lookup"><span data-stu-id="97972-120">Property</span></span>     | <span data-ttu-id="97972-121">类型</span><span class="sxs-lookup"><span data-stu-id="97972-121">Type</span></span>        | <span data-ttu-id="97972-122">描述</span><span class="sxs-lookup"><span data-stu-id="97972-122">Description</span></span>                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|<span data-ttu-id="97972-123">date</span><span class="sxs-lookup"><span data-stu-id="97972-123">date</span></span>          |<span data-ttu-id="97972-124">Date</span><span class="sxs-lookup"><span data-stu-id="97972-124">Date</span></span>         | <span data-ttu-id="97972-125">包含与周年纪念类型相关联的日期。</span><span class="sxs-lookup"><span data-stu-id="97972-125">Contains the date associated with the anniversary type.</span></span>         |
|<span data-ttu-id="97972-126">类型</span><span class="sxs-lookup"><span data-stu-id="97972-126">type</span></span>          |<span data-ttu-id="97972-127">string</span><span class="sxs-lookup"><span data-stu-id="97972-127">string</span></span>       | <span data-ttu-id="97972-128">可取值为：`birthday`、`wedding`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="97972-128">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97972-129">关系</span><span class="sxs-lookup"><span data-stu-id="97972-129">Relationships</span></span>

<span data-ttu-id="97972-130">无。</span><span class="sxs-lookup"><span data-stu-id="97972-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="97972-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97972-131">JSON representation</span></span>

<span data-ttu-id="97972-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97972-132">The following is a JSON representation of the resource.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personAnniversary",
  "baseType": ""
}-->

```json
{
  "date": "String (timestamp)",
  "type": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personAnniversary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
