---
title: changeTrackedEntity 资源类型
description: 表示用于跟踪对任何受支持的班次资源所做更改的实体
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a167f6409ba972b66f23a3608047b4e72c036846
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951977"
---
# <a name="changetrackedentity-resource-type"></a><span data-ttu-id="a4f37-103">changeTrackedEntity 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4f37-103">changeTrackedEntity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4f37-104">表示用于跟踪对任何受支持的[日程安排](schedule.md)和关联资源所做更改的实体。</span><span class="sxs-lookup"><span data-stu-id="a4f37-104">Represents an entity to track changes made to any supported [schedule](schedule.md) and associated resource.</span></span>

## <a name="properties"></a><span data-ttu-id="a4f37-105">属性</span><span class="sxs-lookup"><span data-stu-id="a4f37-105">Properties</span></span>

| <span data-ttu-id="a4f37-106">属性</span><span class="sxs-lookup"><span data-stu-id="a4f37-106">Property</span></span>     | <span data-ttu-id="a4f37-107">类型</span><span class="sxs-lookup"><span data-stu-id="a4f37-107">Type</span></span>        | <span data-ttu-id="a4f37-108">说明</span><span class="sxs-lookup"><span data-stu-id="a4f37-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a4f37-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4f37-109">createdDateTime</span></span>|<span data-ttu-id="a4f37-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4f37-110">DateTimeOffset</span></span>|<span data-ttu-id="a4f37-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a4f37-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a4f37-113">id</span><span class="sxs-lookup"><span data-stu-id="a4f37-113">id</span></span>|<span data-ttu-id="a4f37-114">String</span><span class="sxs-lookup"><span data-stu-id="a4f37-114">String</span></span>| <span data-ttu-id="a4f37-115">只读。</span><span class="sxs-lookup"><span data-stu-id="a4f37-115">Read-only.</span></span>|
|<span data-ttu-id="a4f37-116">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a4f37-116">lastModifiedBy</span></span>|[<span data-ttu-id="a4f37-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="a4f37-117">identitySet</span></span>](identityset.md)|<span data-ttu-id="a4f37-118">上次修改实体的人员的标识。</span><span class="sxs-lookup"><span data-stu-id="a4f37-118">Identity of the person who last modified the entity.</span></span>|
|<span data-ttu-id="a4f37-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4f37-119">lastModifiedDateTime</span></span>|<span data-ttu-id="a4f37-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4f37-120">DateTimeOffset</span></span>|<span data-ttu-id="a4f37-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a4f37-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4f37-123">关系</span><span class="sxs-lookup"><span data-stu-id="a4f37-123">Relationships</span></span>

<span data-ttu-id="a4f37-124">无。</span><span class="sxs-lookup"><span data-stu-id="a4f37-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4f37-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4f37-125">JSON representation</span></span>

<span data-ttu-id="a4f37-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4f37-126">The following is a JSON representation of the resource.</span></span>

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
