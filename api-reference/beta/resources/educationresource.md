---
title: educationResource 资源类型
description: 系统中所有资源对象的超类。 资源与 **工作分配和****/或提交** 相关联，它表示正在学习的对象
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: df2e9b0c49085503e76d56643a755e74e2f0cfaa
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722401"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="ea3b6-104">educationResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="ea3b6-104">educationResource resource type</span></span>

<span data-ttu-id="ea3b6-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea3b6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea3b6-106">系统中所有资源对象的超类。</span><span class="sxs-lookup"><span data-stu-id="ea3b6-106">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="ea3b6-107">资源与工作分配和/或提交相关联，它表示正在提供或提交的学习对象。</span><span class="sxs-lookup"><span data-stu-id="ea3b6-107">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="ea3b6-108">不能直接实例化资源;您必须创建一个表示所使用的资源类型的子类。</span><span class="sxs-lookup"><span data-stu-id="ea3b6-108">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="ea3b6-109">此资源存储所有资源类型的通用属性。</span><span class="sxs-lookup"><span data-stu-id="ea3b6-109">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="ea3b6-110">属性</span><span class="sxs-lookup"><span data-stu-id="ea3b6-110">Properties</span></span>
| <span data-ttu-id="ea3b6-111">属性</span><span class="sxs-lookup"><span data-stu-id="ea3b6-111">Property</span></span>     | <span data-ttu-id="ea3b6-112">类型</span><span class="sxs-lookup"><span data-stu-id="ea3b6-112">Type</span></span>   |<span data-ttu-id="ea3b6-113">说明</span><span class="sxs-lookup"><span data-stu-id="ea3b6-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea3b6-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="ea3b6-114">createdBy</span></span>|[<span data-ttu-id="ea3b6-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="ea3b6-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="ea3b6-116">创建资源的人。</span><span class="sxs-lookup"><span data-stu-id="ea3b6-116">Who created the resource.</span></span>|
|<span data-ttu-id="ea3b6-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea3b6-117">createdDateTime</span></span>|<span data-ttu-id="ea3b6-118">创建资源的时间。</span><span class="sxs-lookup"><span data-stu-id="ea3b6-118">Moment in time when the resource was created.</span></span>  <span data-ttu-id="ea3b6-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea3b6-119">DateTimeOffset</span></span>|<span data-ttu-id="ea3b6-120">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ea3b6-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ea3b6-121">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="ea3b6-121">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="ea3b6-122">displayName</span><span class="sxs-lookup"><span data-stu-id="ea3b6-122">displayName</span></span>|<span data-ttu-id="ea3b6-123">String</span><span class="sxs-lookup"><span data-stu-id="ea3b6-123">String</span></span>|<span data-ttu-id="ea3b6-124">资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ea3b6-124">Display name of resource.</span></span>|
|<span data-ttu-id="ea3b6-125">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ea3b6-125">lastModifiedBy</span></span>|[<span data-ttu-id="ea3b6-126">identitySet</span><span class="sxs-lookup"><span data-stu-id="ea3b6-126">identitySet</span></span>](identityset.md)|<span data-ttu-id="ea3b6-127">上次修改资源的用户是谁。</span><span class="sxs-lookup"><span data-stu-id="ea3b6-127">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="ea3b6-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea3b6-128">lastModifiedDateTime</span></span>|<span data-ttu-id="ea3b6-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea3b6-129">DateTimeOffset</span></span>|<span data-ttu-id="ea3b6-130">上次修改资源的时间。</span><span class="sxs-lookup"><span data-stu-id="ea3b6-130">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="ea3b6-131">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ea3b6-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ea3b6-132">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="ea3b6-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea3b6-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea3b6-133">JSON representation</span></span>

<span data-ttu-id="ea3b6-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea3b6-134">The following is a JSON representation of the resource.</span></span>

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


