---
title: educationResource 资源类型
description: 系统中所有 resource 对象的超类。 资源与 **工作分配** 和/或 **提交**相关联，表示学习对象
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f48d9b0bab9fbabd7e76da7c8d4bc738de5a137b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979572"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="4cb1c-104">educationResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="4cb1c-104">educationResource resource type</span></span>

<span data-ttu-id="4cb1c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cb1c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cb1c-106">系统中所有 resource 对象的超类。</span><span class="sxs-lookup"><span data-stu-id="4cb1c-106">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="4cb1c-107">资源与 **工作分配** 和/或 **提交**相关联，表示正在向外传递或传递的学习对象。</span><span class="sxs-lookup"><span data-stu-id="4cb1c-107">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="4cb1c-108">您不能直接实例化资源;您必须创建一个将代表所用资源类型的子类。</span><span class="sxs-lookup"><span data-stu-id="4cb1c-108">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="4cb1c-109">此资源在所有资源类型中存储通用属性。</span><span class="sxs-lookup"><span data-stu-id="4cb1c-109">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="4cb1c-110">属性</span><span class="sxs-lookup"><span data-stu-id="4cb1c-110">Properties</span></span>
| <span data-ttu-id="4cb1c-111">属性</span><span class="sxs-lookup"><span data-stu-id="4cb1c-111">Property</span></span>     | <span data-ttu-id="4cb1c-112">类型</span><span class="sxs-lookup"><span data-stu-id="4cb1c-112">Type</span></span>   |<span data-ttu-id="4cb1c-113">说明</span><span class="sxs-lookup"><span data-stu-id="4cb1c-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4cb1c-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="4cb1c-114">createdBy</span></span>|[<span data-ttu-id="4cb1c-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="4cb1c-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="4cb1c-116">创建资源的作者。</span><span class="sxs-lookup"><span data-stu-id="4cb1c-116">Who created the resource.</span></span>|
|<span data-ttu-id="4cb1c-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4cb1c-117">createdDateTime</span></span>|<span data-ttu-id="4cb1c-118">创建资源的时间点。</span><span class="sxs-lookup"><span data-stu-id="4cb1c-118">Moment in time when the resource was created.</span></span>  <span data-ttu-id="4cb1c-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cb1c-119">DateTimeOffset</span></span>|<span data-ttu-id="4cb1c-p104">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4cb1c-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4cb1c-122">displayName</span><span class="sxs-lookup"><span data-stu-id="4cb1c-122">displayName</span></span>|<span data-ttu-id="4cb1c-123">String</span><span class="sxs-lookup"><span data-stu-id="4cb1c-123">String</span></span>|<span data-ttu-id="4cb1c-124">资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4cb1c-124">Display name of resource.</span></span>|
|<span data-ttu-id="4cb1c-125">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="4cb1c-125">lastModifiedBy</span></span>|[<span data-ttu-id="4cb1c-126">identitySet</span><span class="sxs-lookup"><span data-stu-id="4cb1c-126">identitySet</span></span>](identityset.md)|<span data-ttu-id="4cb1c-127">谁是修改资源的最后一个用户。</span><span class="sxs-lookup"><span data-stu-id="4cb1c-127">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="4cb1c-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4cb1c-128">lastModifiedDateTime</span></span>|<span data-ttu-id="4cb1c-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cb1c-129">DateTimeOffset</span></span>|<span data-ttu-id="4cb1c-130">上次修改资源的时间点。</span><span class="sxs-lookup"><span data-stu-id="4cb1c-130">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="4cb1c-131">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="4cb1c-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4cb1c-132">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4cb1c-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4cb1c-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4cb1c-133">JSON representation</span></span>

<span data-ttu-id="4cb1c-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4cb1c-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationResource"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


