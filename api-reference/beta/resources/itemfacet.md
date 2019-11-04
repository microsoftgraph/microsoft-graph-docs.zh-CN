---
title: itemFacet 资源类型
description: itemFacet 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: bb89037b3d5b88e57ec12b2b02a5e2ed37cb2601
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939325"
---
# <a name="itemfacet-resource-type"></a><span data-ttu-id="ede56-103">itemFacet 资源类型</span><span class="sxs-lookup"><span data-stu-id="ede56-103">itemFacet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ede56-104">表示[配置文件](profile.md)entityset 中的所有资源类型继承自的抽象基类型。</span><span class="sxs-lookup"><span data-stu-id="ede56-104">Represents the abstract base type that all resource types in the [profile](profile.md) entityset inherit from.</span></span>

## <a name="properties"></a><span data-ttu-id="ede56-105">属性</span><span class="sxs-lookup"><span data-stu-id="ede56-105">Properties</span></span>

| <span data-ttu-id="ede56-106">属性</span><span class="sxs-lookup"><span data-stu-id="ede56-106">Property</span></span>             | <span data-ttu-id="ede56-107">类型</span><span class="sxs-lookup"><span data-stu-id="ede56-107">Type</span></span>                            | <span data-ttu-id="ede56-108">描述</span><span class="sxs-lookup"><span data-stu-id="ede56-108">Description</span></span> |
|:---------------------|:--------------------------------|:------------|
|<span data-ttu-id="ede56-109">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="ede56-109">allowedAudiences</span></span>      |<span data-ttu-id="ede56-110">string</span><span class="sxs-lookup"><span data-stu-id="ede56-110">string</span></span>                           | <span data-ttu-id="ede56-111">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="ede56-111">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>  |
|<span data-ttu-id="ede56-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="ede56-112">createdBy</span></span>             |[<span data-ttu-id="ede56-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="ede56-113">identitySet</span></span>](identityset.md)    | <span data-ttu-id="ede56-114">实体最初创建时。</span><span class="sxs-lookup"><span data-stu-id="ede56-114">When the entity was originally created.</span></span>   |
|<span data-ttu-id="ede56-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ede56-115">createdDateTime</span></span>       |<span data-ttu-id="ede56-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ede56-116">DateTimeOffset</span></span>                   |<span data-ttu-id="ede56-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ede56-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ede56-119">id</span><span class="sxs-lookup"><span data-stu-id="ede56-119">id</span></span>                    |<span data-ttu-id="ede56-120">字符串</span><span class="sxs-lookup"><span data-stu-id="ede56-120">String</span></span>                           | <span data-ttu-id="ede56-121">只读。</span><span class="sxs-lookup"><span data-stu-id="ede56-121">Read-only.</span></span>|
|<span data-ttu-id="ede56-122">推导</span><span class="sxs-lookup"><span data-stu-id="ede56-122">inference</span></span>             |[<span data-ttu-id="ede56-123">inferenceData</span><span class="sxs-lookup"><span data-stu-id="ede56-123">inferenceData</span></span>](inferencedata.md)| <span data-ttu-id="ede56-124">如果对实体进行推断，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="ede56-124">Contains inference detail if the entity is inferred.</span></span> |
|<span data-ttu-id="ede56-125">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ede56-125">lastModifiedBy</span></span>        |[<span data-ttu-id="ede56-126">identitySet</span><span class="sxs-lookup"><span data-stu-id="ede56-126">identitySet</span></span>](identityset.md)    | <span data-ttu-id="ede56-127">上次修改实体的合作伙伴或用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="ede56-127">Identifier of the partner or user who last modified the entity.</span></span> |
|<span data-ttu-id="ede56-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ede56-128">lastModifiedDateTime</span></span>  |<span data-ttu-id="ede56-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ede56-129">DateTimeOffset</span></span>                   |<span data-ttu-id="ede56-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ede56-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="ede56-132">关系</span><span class="sxs-lookup"><span data-stu-id="ede56-132">Relationships</span></span>

<span data-ttu-id="ede56-133">无</span><span class="sxs-lookup"><span data-stu-id="ede56-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ede56-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ede56-134">JSON representation</span></span>

<span data-ttu-id="ede56-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ede56-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemFacet",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "allowedAudiences": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "inference": {"@odata.type": "microsoft.graph.inferenceData"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemFacet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->