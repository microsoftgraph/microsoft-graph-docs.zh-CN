---
title: itemFacet 资源类型
description: itemFacet 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: efd4977872dfefc5a0e5be9b10ad1fa196fa20a4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523070"
---
# <a name="itemfacet-resource-type"></a><span data-ttu-id="445b0-103">itemFacet 资源类型</span><span class="sxs-lookup"><span data-stu-id="445b0-103">itemFacet resource type</span></span>

<span data-ttu-id="445b0-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="445b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="445b0-105">表示[配置文件](profile.md)entityset 中的所有资源类型继承自的抽象基类型。</span><span class="sxs-lookup"><span data-stu-id="445b0-105">Represents the abstract base type that all resource types in the [profile](profile.md) entityset inherit from.</span></span>

## <a name="properties"></a><span data-ttu-id="445b0-106">属性</span><span class="sxs-lookup"><span data-stu-id="445b0-106">Properties</span></span>

| <span data-ttu-id="445b0-107">属性</span><span class="sxs-lookup"><span data-stu-id="445b0-107">Property</span></span>             | <span data-ttu-id="445b0-108">类型</span><span class="sxs-lookup"><span data-stu-id="445b0-108">Type</span></span>                            | <span data-ttu-id="445b0-109">说明</span><span class="sxs-lookup"><span data-stu-id="445b0-109">Description</span></span> |
|:---------------------|:--------------------------------|:------------|
|<span data-ttu-id="445b0-110">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="445b0-110">allowedAudiences</span></span>      |<span data-ttu-id="445b0-111">string</span><span class="sxs-lookup"><span data-stu-id="445b0-111">string</span></span>                           | <span data-ttu-id="445b0-112">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="445b0-112">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>  |
|<span data-ttu-id="445b0-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="445b0-113">createdBy</span></span>             |[<span data-ttu-id="445b0-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="445b0-114">identitySet</span></span>](identityset.md)    | <span data-ttu-id="445b0-115">实体最初创建时。</span><span class="sxs-lookup"><span data-stu-id="445b0-115">When the entity was originally created.</span></span>   |
|<span data-ttu-id="445b0-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="445b0-116">createdDateTime</span></span>       |<span data-ttu-id="445b0-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="445b0-117">DateTimeOffset</span></span>                   |<span data-ttu-id="445b0-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="445b0-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="445b0-120">id</span><span class="sxs-lookup"><span data-stu-id="445b0-120">id</span></span>                    |<span data-ttu-id="445b0-121">String</span><span class="sxs-lookup"><span data-stu-id="445b0-121">String</span></span>                           | <span data-ttu-id="445b0-122">只读。</span><span class="sxs-lookup"><span data-stu-id="445b0-122">Read-only.</span></span>|
|<span data-ttu-id="445b0-123">推导</span><span class="sxs-lookup"><span data-stu-id="445b0-123">inference</span></span>             |[<span data-ttu-id="445b0-124">inferenceData</span><span class="sxs-lookup"><span data-stu-id="445b0-124">inferenceData</span></span>](inferencedata.md)| <span data-ttu-id="445b0-125">如果对实体进行推断，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="445b0-125">Contains inference detail if the entity is inferred.</span></span> |
|<span data-ttu-id="445b0-126">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="445b0-126">lastModifiedBy</span></span>        |[<span data-ttu-id="445b0-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="445b0-127">identitySet</span></span>](identityset.md)    | <span data-ttu-id="445b0-128">上次修改实体的合作伙伴或用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="445b0-128">Identifier of the partner or user who last modified the entity.</span></span> |
|<span data-ttu-id="445b0-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="445b0-129">lastModifiedDateTime</span></span>  |<span data-ttu-id="445b0-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="445b0-130">DateTimeOffset</span></span>                   |<span data-ttu-id="445b0-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="445b0-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="445b0-133">关系</span><span class="sxs-lookup"><span data-stu-id="445b0-133">Relationships</span></span>

<span data-ttu-id="445b0-134">无</span><span class="sxs-lookup"><span data-stu-id="445b0-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="445b0-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="445b0-135">JSON representation</span></span>

<span data-ttu-id="445b0-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="445b0-136">The following is a JSON representation of the resource.</span></span>

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