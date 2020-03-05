---
title: skillProficiency 资源类型
description: skillProficiency 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6662ab205e390ae72d283d5015aa346c4b6fc2b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520504"
---
# <a name="skillproficiency-resource-type"></a><span data-ttu-id="cd202-103">skillProficiency 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd202-103">skillProficiency resource type</span></span>

<span data-ttu-id="cd202-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="cd202-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd202-105">表示有关与各种服务中的用户相关的技能的详细信息。</span><span class="sxs-lookup"><span data-stu-id="cd202-105">Represents detailed information about skills associated with a user in various services.</span></span>

<span data-ttu-id="cd202-106">继承自[itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="cd202-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="cd202-107">方法</span><span class="sxs-lookup"><span data-stu-id="cd202-107">Methods</span></span>
 
| <span data-ttu-id="cd202-108">方法</span><span class="sxs-lookup"><span data-stu-id="cd202-108">Method</span></span>                                                 | <span data-ttu-id="cd202-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="cd202-109">Return Type</span></span>                             | <span data-ttu-id="cd202-110">说明</span><span class="sxs-lookup"><span data-stu-id="cd202-110">Description</span></span>                                                   |
|:-------------------------------------------------------|:----------------------------------------|:--------------------------------------------------------------|
| [<span data-ttu-id="cd202-111">获取 skillProficiency</span><span class="sxs-lookup"><span data-stu-id="cd202-111">Get skillProficiency</span></span>](../api/skillproficiency-get.md) | [<span data-ttu-id="cd202-112">skillProficiency</span><span class="sxs-lookup"><span data-stu-id="cd202-112">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="cd202-113">读取**skillProficiency**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cd202-113">Read the properties and relationships of a **skillProficiency** object.</span></span> |
| [<span data-ttu-id="cd202-114">更新 skillProficiency</span><span class="sxs-lookup"><span data-stu-id="cd202-114">Update skillProficiency</span></span>](../api/skillproficiency-update.md)            | [<span data-ttu-id="cd202-115">skillProficiency</span><span class="sxs-lookup"><span data-stu-id="cd202-115">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="cd202-116">更新**skillProficiency**对象。</span><span class="sxs-lookup"><span data-stu-id="cd202-116">Update a **skillProficiency** object.</span></span>                               |
| [<span data-ttu-id="cd202-117">删除 skillProficiency</span><span class="sxs-lookup"><span data-stu-id="cd202-117">Delete skillProficiency</span></span>](../api/skillproficiency-delete.md)            | <span data-ttu-id="cd202-118">无</span><span class="sxs-lookup"><span data-stu-id="cd202-118">None</span></span>                                    | <span data-ttu-id="cd202-119">删除**skillProficiency**对象。</span><span class="sxs-lookup"><span data-stu-id="cd202-119">Delete a **skillProficiency** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="cd202-120">属性</span><span class="sxs-lookup"><span data-stu-id="cd202-120">Properties</span></span>

| <span data-ttu-id="cd202-121">属性</span><span class="sxs-lookup"><span data-stu-id="cd202-121">Property</span></span>     | <span data-ttu-id="cd202-122">类型</span><span class="sxs-lookup"><span data-stu-id="cd202-122">Type</span></span>             | <span data-ttu-id="cd202-123">说明</span><span class="sxs-lookup"><span data-stu-id="cd202-123">Description</span></span>                                                                                                                        |
|:-------------|:-----------------|:-----------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="cd202-124">categories</span><span class="sxs-lookup"><span data-stu-id="cd202-124">categories</span></span>    |<span data-ttu-id="cd202-125">String 集合</span><span class="sxs-lookup"><span data-stu-id="cd202-125">String collection</span></span> | <span data-ttu-id="cd202-126">包含用户与技能相关联的类别（例如，个人、职业、爱好）。</span><span class="sxs-lookup"><span data-stu-id="cd202-126">Contains categories a user has associated with the skill (for example, personal, professional, hobby).</span></span>                                       |
|<span data-ttu-id="cd202-127">displayName</span><span class="sxs-lookup"><span data-stu-id="cd202-127">displayName</span></span>   |<span data-ttu-id="cd202-128">String</span><span class="sxs-lookup"><span data-stu-id="cd202-128">String</span></span>            | <span data-ttu-id="cd202-129">包含技能的友好名称。</span><span class="sxs-lookup"><span data-stu-id="cd202-129">Contains a friendly name for the skill.</span></span>                                                                                            |      
|<span data-ttu-id="cd202-130">水平</span><span class="sxs-lookup"><span data-stu-id="cd202-130">proficiency</span></span>   |<span data-ttu-id="cd202-131">string</span><span class="sxs-lookup"><span data-stu-id="cd202-131">string</span></span>            | <span data-ttu-id="cd202-132">可取值为：`elementary`、`limitedWorking`、`generalProfessional`、`advancedProfessional`、`expert`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="cd202-132">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="cd202-133">webUrl</span><span class="sxs-lookup"><span data-stu-id="cd202-133">webUrl</span></span>        |<span data-ttu-id="cd202-134">String</span><span class="sxs-lookup"><span data-stu-id="cd202-134">String</span></span>            | <span data-ttu-id="cd202-135">包含指向有关技能的信息源的链接。</span><span class="sxs-lookup"><span data-stu-id="cd202-135">Contains a link to an information source about the skill.</span></span>                                                                          |

## <a name="relationships"></a><span data-ttu-id="cd202-136">关系</span><span class="sxs-lookup"><span data-stu-id="cd202-136">Relationships</span></span>

<span data-ttu-id="cd202-137">无。</span><span class="sxs-lookup"><span data-stu-id="cd202-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd202-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd202-138">JSON representation</span></span>

<span data-ttu-id="cd202-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd202-139">The following is a JSON representation of the resource.</span></span>

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
