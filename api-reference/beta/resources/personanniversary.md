---
title: personAnniversary 资源类型
description: personAnniversary 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: c8ea4e9bf7db268c5ec6bffad1c7d43cbbdd2439
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227727"
---
# <a name="personanniversary-resource-type"></a><span data-ttu-id="beffc-103">personAnniversary 资源类型</span><span class="sxs-lookup"><span data-stu-id="beffc-103">personAnniversary resource type</span></span>

<span data-ttu-id="beffc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="beffc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="beffc-105">表示与用户[配置文件](profile.md)中的人员关联的有意义日期的详细信息。</span><span class="sxs-lookup"><span data-stu-id="beffc-105">Represents the details of meaningful dates associated with a person in a user's [profile](profile.md).</span></span>

<span data-ttu-id="beffc-106">继承自[itemFacet](itemFacet.md)。</span><span class="sxs-lookup"><span data-stu-id="beffc-106">Inherits from [itemFacet](itemFacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="beffc-107">方法</span><span class="sxs-lookup"><span data-stu-id="beffc-107">Methods</span></span>

| <span data-ttu-id="beffc-108">方法</span><span class="sxs-lookup"><span data-stu-id="beffc-108">Method</span></span>                                                   | <span data-ttu-id="beffc-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="beffc-109">Return Type</span></span>                               | <span data-ttu-id="beffc-110">说明</span><span class="sxs-lookup"><span data-stu-id="beffc-110">Description</span></span>                                                              |
|:---------------------------------------------------------|:------------------------------------------|:-------------------------------------------------------------------------|
| [<span data-ttu-id="beffc-111">获取 personAnniversary</span><span class="sxs-lookup"><span data-stu-id="beffc-111">Get personAnniversary</span></span>](../api/personanniversary-get.md) | [<span data-ttu-id="beffc-112">personAnniversary</span><span class="sxs-lookup"><span data-stu-id="beffc-112">personAnniversary</span></span>](personanniversary.md) | <span data-ttu-id="beffc-113">读取**personAnniversary**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="beffc-113">Read the properties and relationships of a **personAnniversary** object.</span></span> |
| [<span data-ttu-id="beffc-114">更新</span><span class="sxs-lookup"><span data-stu-id="beffc-114">Update</span></span>](../api/personanniversary-update.md)             | [<span data-ttu-id="beffc-115">personAnniversary</span><span class="sxs-lookup"><span data-stu-id="beffc-115">personAnniversary</span></span>](personanniversary.md) | <span data-ttu-id="beffc-116">更新**personAnniversary**对象。</span><span class="sxs-lookup"><span data-stu-id="beffc-116">Update a **personAnniversary** object.</span></span>                                   |
| [<span data-ttu-id="beffc-117">删除</span><span class="sxs-lookup"><span data-stu-id="beffc-117">Delete</span></span>](../api/personanniversary-delete.md)             | <span data-ttu-id="beffc-118">无</span><span class="sxs-lookup"><span data-stu-id="beffc-118">None</span></span>                                      | <span data-ttu-id="beffc-119">删除**personAnniversary**对象。</span><span class="sxs-lookup"><span data-stu-id="beffc-119">Delete a **personAnniversary** object.</span></span>                                   |

## <a name="properties"></a><span data-ttu-id="beffc-120">属性</span><span class="sxs-lookup"><span data-stu-id="beffc-120">Properties</span></span>

| <span data-ttu-id="beffc-121">属性</span><span class="sxs-lookup"><span data-stu-id="beffc-121">Property</span></span>     | <span data-ttu-id="beffc-122">类型</span><span class="sxs-lookup"><span data-stu-id="beffc-122">Type</span></span>        | <span data-ttu-id="beffc-123">说明</span><span class="sxs-lookup"><span data-stu-id="beffc-123">Description</span></span>                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|<span data-ttu-id="beffc-124">date</span><span class="sxs-lookup"><span data-stu-id="beffc-124">date</span></span>          |<span data-ttu-id="beffc-125">Date</span><span class="sxs-lookup"><span data-stu-id="beffc-125">Date</span></span>         | <span data-ttu-id="beffc-126">包含与周年纪念类型相关联的日期。</span><span class="sxs-lookup"><span data-stu-id="beffc-126">Contains the date associated with the anniversary type.</span></span>          |
|<span data-ttu-id="beffc-127">类型</span><span class="sxs-lookup"><span data-stu-id="beffc-127">type</span></span>          |<span data-ttu-id="beffc-128">string</span><span class="sxs-lookup"><span data-stu-id="beffc-128">string</span></span>       | <span data-ttu-id="beffc-129">可取值为：`birthday`、`wedding`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="beffc-129">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="beffc-130">关系</span><span class="sxs-lookup"><span data-stu-id="beffc-130">Relationships</span></span>

<span data-ttu-id="beffc-131">无。</span><span class="sxs-lookup"><span data-stu-id="beffc-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="beffc-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="beffc-132">JSON representation</span></span>

<span data-ttu-id="beffc-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="beffc-133">The following is a JSON representation of the resource.</span></span>

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
