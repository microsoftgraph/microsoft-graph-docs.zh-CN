---
title: skillProficiency 资源类型
description: skillProficiency 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 9490947aea170f2b6e94ecd8f02f59d396746e3a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938707"
---
# <a name="skillproficiency-resource-type"></a><span data-ttu-id="04483-103">skillProficiency 资源类型</span><span class="sxs-lookup"><span data-stu-id="04483-103">skillProficiency resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04483-104">代表有关用户在各种服务中与自己关联的技能的详细信息。</span><span class="sxs-lookup"><span data-stu-id="04483-104">Represents detailed information about skills the user has associated with themselves in various services.</span></span>

<span data-ttu-id="04483-105">继承自[itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="04483-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="04483-106">方法</span><span class="sxs-lookup"><span data-stu-id="04483-106">Methods</span></span>
 
| <span data-ttu-id="04483-107">方法</span><span class="sxs-lookup"><span data-stu-id="04483-107">Method</span></span>                                                 | <span data-ttu-id="04483-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="04483-108">Return Type</span></span>                             | <span data-ttu-id="04483-109">说明</span><span class="sxs-lookup"><span data-stu-id="04483-109">Description</span></span>                                                   |
|:-------------------------------------------------------|:----------------------------------------|:--------------------------------------------------------------|
| [<span data-ttu-id="04483-110">获取 skillProficiency</span><span class="sxs-lookup"><span data-stu-id="04483-110">Get skillProficiency</span></span>](../api/skillproficiency-get.md) | [<span data-ttu-id="04483-111">skillProficiency</span><span class="sxs-lookup"><span data-stu-id="04483-111">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="04483-112">读取 skillProficiency 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="04483-112">Read properties and relationships of skillProficiency object.</span></span> |
| [<span data-ttu-id="04483-113">Update</span><span class="sxs-lookup"><span data-stu-id="04483-113">Update</span></span>](../api/skillproficiency-update.md)            | [<span data-ttu-id="04483-114">skillProficiency</span><span class="sxs-lookup"><span data-stu-id="04483-114">skillProficiency</span></span>](skillproficiency.md) | <span data-ttu-id="04483-115">更新 skillProficiency 对象。</span><span class="sxs-lookup"><span data-stu-id="04483-115">Update skillProficiency object.</span></span>                               |
| [<span data-ttu-id="04483-116">删除</span><span class="sxs-lookup"><span data-stu-id="04483-116">Delete</span></span>](../api/skillproficiency-delete.md)            | <span data-ttu-id="04483-117">无</span><span class="sxs-lookup"><span data-stu-id="04483-117">None</span></span>                                    | <span data-ttu-id="04483-118">删除 skillProficiency 对象。</span><span class="sxs-lookup"><span data-stu-id="04483-118">Delete skillProficiency object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="04483-119">属性</span><span class="sxs-lookup"><span data-stu-id="04483-119">Properties</span></span>

| <span data-ttu-id="04483-120">属性</span><span class="sxs-lookup"><span data-stu-id="04483-120">Property</span></span>     | <span data-ttu-id="04483-121">类型</span><span class="sxs-lookup"><span data-stu-id="04483-121">Type</span></span>             | <span data-ttu-id="04483-122">描述</span><span class="sxs-lookup"><span data-stu-id="04483-122">Description</span></span>                                                                                                                        |
|:-------------|:-----------------|:-----------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="04483-123">类别</span><span class="sxs-lookup"><span data-stu-id="04483-123">categories</span></span>    |<span data-ttu-id="04483-124">String collection</span><span class="sxs-lookup"><span data-stu-id="04483-124">String collection</span></span> | <span data-ttu-id="04483-125">包含用户与技能相关联的类别（例如：个人、职业、爱好）</span><span class="sxs-lookup"><span data-stu-id="04483-125">Contains categories a user has associated with the skill (eg: personal, professional, hobby)</span></span>                                       |
|<span data-ttu-id="04483-126">displayName</span><span class="sxs-lookup"><span data-stu-id="04483-126">displayName</span></span>   |<span data-ttu-id="04483-127">String</span><span class="sxs-lookup"><span data-stu-id="04483-127">String</span></span>            | <span data-ttu-id="04483-128">包含技能的友好名称。</span><span class="sxs-lookup"><span data-stu-id="04483-128">Contains a friendly name for the skill.</span></span>                                                                                            |      
|<span data-ttu-id="04483-129">水平</span><span class="sxs-lookup"><span data-stu-id="04483-129">proficiency</span></span>   |<span data-ttu-id="04483-130">string</span><span class="sxs-lookup"><span data-stu-id="04483-130">string</span></span>            | <span data-ttu-id="04483-131">可取值为：`elementary`、`limitedWorking`、`generalProfessional`、`advancedProfessional`、`expert`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="04483-131">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="04483-132">webUrl</span><span class="sxs-lookup"><span data-stu-id="04483-132">webUrl</span></span>        |<span data-ttu-id="04483-133">String</span><span class="sxs-lookup"><span data-stu-id="04483-133">String</span></span>            | <span data-ttu-id="04483-134">包含指向有关技能的信息源的链接。</span><span class="sxs-lookup"><span data-stu-id="04483-134">Contains a link to an information source about the skill.</span></span>                                                                          |

## <a name="relationships"></a><span data-ttu-id="04483-135">关系</span><span class="sxs-lookup"><span data-stu-id="04483-135">Relationships</span></span>

<span data-ttu-id="04483-136">无</span><span class="sxs-lookup"><span data-stu-id="04483-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04483-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04483-137">JSON representation</span></span>

<span data-ttu-id="04483-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04483-138">The following is a JSON representation of the resource.</span></span>

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