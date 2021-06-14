---
title: educationResource 资源类型
description: 系统中所有资源对象的超级类。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d5433bfc5648b8c4d0ff04ab5f91da7df0b1a1c5
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912274"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="c2963-103">educationResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2963-103">educationResource resource type</span></span>

<span data-ttu-id="c2963-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2963-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c2963-105">系统中所有资源对象的超级类。</span><span class="sxs-lookup"><span data-stu-id="c2963-105">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="c2963-106">资源与工作分配和/或 **提交** 相关联，它表示要分配或提交的学习对象。</span><span class="sxs-lookup"><span data-stu-id="c2963-106">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="c2963-107">不能直接实例化资源;您必须创建一个表示所使用的资源类型的子类。</span><span class="sxs-lookup"><span data-stu-id="c2963-107">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="c2963-108">此资源存储所有资源类型的通用属性。</span><span class="sxs-lookup"><span data-stu-id="c2963-108">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="c2963-109">属性</span><span class="sxs-lookup"><span data-stu-id="c2963-109">Properties</span></span>
| <span data-ttu-id="c2963-110">属性</span><span class="sxs-lookup"><span data-stu-id="c2963-110">Property</span></span>     | <span data-ttu-id="c2963-111">类型</span><span class="sxs-lookup"><span data-stu-id="c2963-111">Type</span></span>   |<span data-ttu-id="c2963-112">说明</span><span class="sxs-lookup"><span data-stu-id="c2963-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2963-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="c2963-113">createdBy</span></span>|[<span data-ttu-id="c2963-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="c2963-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="c2963-115">创建资源的人。</span><span class="sxs-lookup"><span data-stu-id="c2963-115">The individual who created the resource.</span></span>|
|<span data-ttu-id="c2963-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c2963-116">createdDateTime</span></span>|<span data-ttu-id="c2963-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2963-117">DateTimeOffset</span></span>|<span data-ttu-id="c2963-118">创建资源的时间。</span><span class="sxs-lookup"><span data-stu-id="c2963-118">Moment in time when the resource was created.</span></span> <span data-ttu-id="c2963-119">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="c2963-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c2963-120">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="c2963-120">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="c2963-121">displayName</span><span class="sxs-lookup"><span data-stu-id="c2963-121">displayName</span></span>|<span data-ttu-id="c2963-122">String</span><span class="sxs-lookup"><span data-stu-id="c2963-122">String</span></span>|<span data-ttu-id="c2963-123">资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c2963-123">Display name of resource.</span></span>|
|<span data-ttu-id="c2963-124">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c2963-124">lastModifiedBy</span></span>|[<span data-ttu-id="c2963-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="c2963-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="c2963-126">最后一个修改资源的用户。</span><span class="sxs-lookup"><span data-stu-id="c2963-126">The last user to modify the resource.</span></span>|
|<span data-ttu-id="c2963-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2963-127">lastModifiedDateTime</span></span>|<span data-ttu-id="c2963-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2963-128">DateTimeOffset</span></span>|<span data-ttu-id="c2963-129">上次修改资源的时间。</span><span class="sxs-lookup"><span data-stu-id="c2963-129">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="c2963-130">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="c2963-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c2963-131">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="c2963-131">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2963-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2963-132">JSON representation</span></span>

<span data-ttu-id="c2963-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2963-133">The following is a JSON representation of the resource.</span></span>

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


