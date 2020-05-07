---
title: changeTrackedEntity 资源类型
description: 表示用于跟踪对任何受支持的班次资源所做更改的实体
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3e345caf373753ee699d822fd36da0d3afe2fc94
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154961"
---
# <a name="changetrackedentity-resource-type"></a><span data-ttu-id="07617-103">changeTrackedEntity 资源类型</span><span class="sxs-lookup"><span data-stu-id="07617-103">changeTrackedEntity resource type</span></span>

<span data-ttu-id="07617-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07617-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="07617-105">表示用于跟踪对任何受支持的[日程安排](schedule.md)和关联资源所做更改的实体。</span><span class="sxs-lookup"><span data-stu-id="07617-105">Represents an entity to track changes made to any supported [schedule](schedule.md) and associated resource.</span></span>

## <a name="properties"></a><span data-ttu-id="07617-106">属性</span><span class="sxs-lookup"><span data-stu-id="07617-106">Properties</span></span>

| <span data-ttu-id="07617-107">属性</span><span class="sxs-lookup"><span data-stu-id="07617-107">Property</span></span>     | <span data-ttu-id="07617-108">类型</span><span class="sxs-lookup"><span data-stu-id="07617-108">Type</span></span>        | <span data-ttu-id="07617-109">说明</span><span class="sxs-lookup"><span data-stu-id="07617-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="07617-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07617-110">createdDateTime</span></span>|<span data-ttu-id="07617-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07617-111">DateTimeOffset</span></span>|<span data-ttu-id="07617-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="07617-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="07617-114">id</span><span class="sxs-lookup"><span data-stu-id="07617-114">id</span></span>|<span data-ttu-id="07617-115">字符串</span><span class="sxs-lookup"><span data-stu-id="07617-115">String</span></span>| <span data-ttu-id="07617-116">只读。</span><span class="sxs-lookup"><span data-stu-id="07617-116">Read-only.</span></span>|
|<span data-ttu-id="07617-117">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="07617-117">lastModifiedBy</span></span>|[<span data-ttu-id="07617-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="07617-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="07617-119">上次修改实体的人员的标识。</span><span class="sxs-lookup"><span data-stu-id="07617-119">Identity of the person who last modified the entity.</span></span>|
|<span data-ttu-id="07617-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07617-120">lastModifiedDateTime</span></span>|<span data-ttu-id="07617-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07617-121">DateTimeOffset</span></span>|<span data-ttu-id="07617-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="07617-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="07617-124">关系</span><span class="sxs-lookup"><span data-stu-id="07617-124">Relationships</span></span>

<span data-ttu-id="07617-125">无。</span><span class="sxs-lookup"><span data-stu-id="07617-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="07617-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07617-126">JSON representation</span></span>

<span data-ttu-id="07617-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07617-127">The following is a JSON representation of the resource.</span></span>

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
