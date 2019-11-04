---
title: skillProficiency 资源类型
description: skillProficiency 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0bb63903b5a3eb0eeed8683463b9927537180f53
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950421"
---
# <a name="skillproficiency-resource-type"></a><span data-ttu-id="d8d9f-103">skillProficiency 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8d9f-103">skillProficiency resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8d9f-104">表示有关与各种服务中的用户相关的技能的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d8d9f-104">Represents detailed information about skills associated with a user in various services.</span></span>

<span data-ttu-id="d8d9f-105">继承自[itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="d8d9f-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d8d9f-106">方法</span><span class="sxs-lookup"><span data-stu-id="d8d9f-106">Methods</span></span>
 
| <span data-ttu-id="d8d9f-107">方法</span><span class="sxs-lookup"><span data-stu-id="d8d9f-107">Method</span></span>                                                 | <span data-ttu-id="d8d9f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d8d9f-108">Return Type</span></span>                             | <span data-ttu-id="d8d9f-109">说明</span><span class="sxs-lookup"><span data-stu-id="d8d9f-109">Description</span></span>                                                   |
|:-------------------------------------------------------|:----------------------------------------|:--------------------------------------------------------------|
| [<span data-ttu-id="d8d9f-110">获取 skillProficiency</span><span class="sxs-lookup"><span data-stu-id="d8d9f-110">Get skillProficiency</span></span>](../api/skillproficiency-get.md) | [<span data-ttu-id="d8d9f-111">skillProficiency</span><span class="sxs-lookup"><span data-stu-id="d8d9f-111">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="d8d9f-112">读取**skillProficiency**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d8d9f-112">Read the properties and relationships of a **skillProficiency** object.</span></span> |
| [<span data-ttu-id="d8d9f-113">更新 skillProficiency</span><span class="sxs-lookup"><span data-stu-id="d8d9f-113">Update skillProficiency</span></span>](../api/skillproficiency-update.md)            | [<span data-ttu-id="d8d9f-114">skillProficiency</span><span class="sxs-lookup"><span data-stu-id="d8d9f-114">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="d8d9f-115">更新**skillProficiency**对象。</span><span class="sxs-lookup"><span data-stu-id="d8d9f-115">Update a **skillProficiency** object.</span></span>                               |
| [<span data-ttu-id="d8d9f-116">删除 skillProficiency</span><span class="sxs-lookup"><span data-stu-id="d8d9f-116">Delete skillProficiency</span></span>](../api/skillproficiency-delete.md)            | <span data-ttu-id="d8d9f-117">无</span><span class="sxs-lookup"><span data-stu-id="d8d9f-117">None</span></span>                                    | <span data-ttu-id="d8d9f-118">删除**skillProficiency**对象。</span><span class="sxs-lookup"><span data-stu-id="d8d9f-118">Delete a **skillProficiency** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="d8d9f-119">属性</span><span class="sxs-lookup"><span data-stu-id="d8d9f-119">Properties</span></span>

| <span data-ttu-id="d8d9f-120">属性</span><span class="sxs-lookup"><span data-stu-id="d8d9f-120">Property</span></span>     | <span data-ttu-id="d8d9f-121">类型</span><span class="sxs-lookup"><span data-stu-id="d8d9f-121">Type</span></span>             | <span data-ttu-id="d8d9f-122">描述</span><span class="sxs-lookup"><span data-stu-id="d8d9f-122">Description</span></span>                                                                                                                        |
|:-------------|:-----------------|:-----------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="d8d9f-123">类别</span><span class="sxs-lookup"><span data-stu-id="d8d9f-123">categories</span></span>    |<span data-ttu-id="d8d9f-124">String collection</span><span class="sxs-lookup"><span data-stu-id="d8d9f-124">String collection</span></span> | <span data-ttu-id="d8d9f-125">包含用户与技能相关联的类别（例如，个人、职业、爱好）。</span><span class="sxs-lookup"><span data-stu-id="d8d9f-125">Contains categories a user has associated with the skill (for example, personal, professional, hobby).</span></span>                                       |
|<span data-ttu-id="d8d9f-126">displayName</span><span class="sxs-lookup"><span data-stu-id="d8d9f-126">displayName</span></span>   |<span data-ttu-id="d8d9f-127">String</span><span class="sxs-lookup"><span data-stu-id="d8d9f-127">String</span></span>            | <span data-ttu-id="d8d9f-128">包含技能的友好名称。</span><span class="sxs-lookup"><span data-stu-id="d8d9f-128">Contains a friendly name for the skill.</span></span>                                                                                            |      
|<span data-ttu-id="d8d9f-129">水平</span><span class="sxs-lookup"><span data-stu-id="d8d9f-129">proficiency</span></span>   |<span data-ttu-id="d8d9f-130">string</span><span class="sxs-lookup"><span data-stu-id="d8d9f-130">string</span></span>            | <span data-ttu-id="d8d9f-131">可取值为：`elementary`、`limitedWorking`、`generalProfessional`、`advancedProfessional`、`expert`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="d8d9f-131">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d8d9f-132">webUrl</span><span class="sxs-lookup"><span data-stu-id="d8d9f-132">webUrl</span></span>        |<span data-ttu-id="d8d9f-133">String</span><span class="sxs-lookup"><span data-stu-id="d8d9f-133">String</span></span>            | <span data-ttu-id="d8d9f-134">包含指向有关技能的信息源的链接。</span><span class="sxs-lookup"><span data-stu-id="d8d9f-134">Contains a link to an information source about the skill.</span></span>                                                                          |

## <a name="relationships"></a><span data-ttu-id="d8d9f-135">关系</span><span class="sxs-lookup"><span data-stu-id="d8d9f-135">Relationships</span></span>

<span data-ttu-id="d8d9f-136">无。</span><span class="sxs-lookup"><span data-stu-id="d8d9f-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8d9f-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8d9f-137">JSON representation</span></span>

<span data-ttu-id="d8d9f-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8d9f-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.skillProficiency",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "displayName": "String",
  "proficiency": "string",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "skillProficiency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
