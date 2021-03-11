---
title: changeTrackedEntity 资源类型
description: 表示用于跟踪对任意受支持的 Shifts 资源所做的更改的实体
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e02c02b931558b927f29e7b08a18c5d5937f0f72
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720212"
---
# <a name="changetrackedentity-resource-type"></a><span data-ttu-id="87698-103">changeTrackedEntity 资源类型</span><span class="sxs-lookup"><span data-stu-id="87698-103">changeTrackedEntity resource type</span></span>

<span data-ttu-id="87698-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87698-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87698-105">表示用于跟踪对任何受支持的计划和相关资源所做的更改[](schedule.md)的实体。</span><span class="sxs-lookup"><span data-stu-id="87698-105">Represents an entity to track changes made to any supported [schedule](schedule.md) and associated resource.</span></span>

## <a name="properties"></a><span data-ttu-id="87698-106">属性</span><span class="sxs-lookup"><span data-stu-id="87698-106">Properties</span></span>

| <span data-ttu-id="87698-107">属性</span><span class="sxs-lookup"><span data-stu-id="87698-107">Property</span></span>     | <span data-ttu-id="87698-108">类型</span><span class="sxs-lookup"><span data-stu-id="87698-108">Type</span></span>        | <span data-ttu-id="87698-109">说明</span><span class="sxs-lookup"><span data-stu-id="87698-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="87698-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87698-110">createdDateTime</span></span>|<span data-ttu-id="87698-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87698-111">DateTimeOffset</span></span>|<span data-ttu-id="87698-112">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="87698-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="87698-113">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="87698-113">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="87698-114">id</span><span class="sxs-lookup"><span data-stu-id="87698-114">id</span></span>|<span data-ttu-id="87698-115">String</span><span class="sxs-lookup"><span data-stu-id="87698-115">String</span></span>| <span data-ttu-id="87698-116">只读。</span><span class="sxs-lookup"><span data-stu-id="87698-116">Read-only.</span></span>|
|<span data-ttu-id="87698-117">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="87698-117">lastModifiedBy</span></span>|[<span data-ttu-id="87698-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="87698-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="87698-119">上次修改实体的人的标识。</span><span class="sxs-lookup"><span data-stu-id="87698-119">Identity of the person who last modified the entity.</span></span>|
|<span data-ttu-id="87698-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87698-120">lastModifiedDateTime</span></span>|<span data-ttu-id="87698-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87698-121">DateTimeOffset</span></span>|<span data-ttu-id="87698-122">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="87698-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="87698-123">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="87698-123">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="87698-124">关系</span><span class="sxs-lookup"><span data-stu-id="87698-124">Relationships</span></span>

<span data-ttu-id="87698-125">无。</span><span class="sxs-lookup"><span data-stu-id="87698-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="87698-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87698-126">JSON representation</span></span>

<span data-ttu-id="87698-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87698-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeTrackedEntity",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "changeTrackedEntity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


