---
title: educationResource 资源类型
description: 超类别的系统中的所有资源对象。 资源相关联的**工作分配**和/或**提交**，该对象表示正在学习对象
ms.openlocfilehash: b7e64a946992bb0b43c5bfe50e8d92b5f7176856
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046883"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="e3e74-104">educationResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="e3e74-104">educationResource resource type</span></span>

> <span data-ttu-id="e3e74-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e3e74-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3e74-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e3e74-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3e74-107">超类别的系统中的所有资源对象。</span><span class="sxs-lookup"><span data-stu-id="e3e74-107">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="e3e74-108">资源相关联的**工作分配**和/或**提交**，该对象表示正在学习对象分发或传递。</span><span class="sxs-lookup"><span data-stu-id="e3e74-108">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="e3e74-109">不能直接调用实例化资源您必须进行子类表示正在使用的资源的类型。</span><span class="sxs-lookup"><span data-stu-id="e3e74-109">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="e3e74-110">此资源存储跨所有资源类型的通用属性。</span><span class="sxs-lookup"><span data-stu-id="e3e74-110">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="e3e74-111">属性</span><span class="sxs-lookup"><span data-stu-id="e3e74-111">Properties</span></span>
| <span data-ttu-id="e3e74-112">属性</span><span class="sxs-lookup"><span data-stu-id="e3e74-112">Property</span></span>     | <span data-ttu-id="e3e74-113">类型</span><span class="sxs-lookup"><span data-stu-id="e3e74-113">Type</span></span>   |<span data-ttu-id="e3e74-114">说明</span><span class="sxs-lookup"><span data-stu-id="e3e74-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3e74-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="e3e74-115">createdBy</span></span>|[<span data-ttu-id="e3e74-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="e3e74-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="e3e74-117">资源创建者。</span><span class="sxs-lookup"><span data-stu-id="e3e74-117">Who created the resource.</span></span>|
|<span data-ttu-id="e3e74-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3e74-118">createdDateTime</span></span>|<span data-ttu-id="e3e74-119">创建资源时时刻。</span><span class="sxs-lookup"><span data-stu-id="e3e74-119">Moment in time when the resource was created.</span></span>  <span data-ttu-id="e3e74-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3e74-120">DateTimeOffset</span></span>|<span data-ttu-id="e3e74-p105">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e3e74-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e3e74-123">displayName</span><span class="sxs-lookup"><span data-stu-id="e3e74-123">displayName</span></span>|<span data-ttu-id="e3e74-124">字符串</span><span class="sxs-lookup"><span data-stu-id="e3e74-124">String</span></span>|<span data-ttu-id="e3e74-125">显示资源的名称。</span><span class="sxs-lookup"><span data-stu-id="e3e74-125">Display name of resource.</span></span>|
|<span data-ttu-id="e3e74-126">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="e3e74-126">lastModifiedBy</span></span>|[<span data-ttu-id="e3e74-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="e3e74-127">identitySet</span></span>](identityset.md)|<span data-ttu-id="e3e74-128">谁是最后一个用户修改的资源。</span><span class="sxs-lookup"><span data-stu-id="e3e74-128">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="e3e74-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3e74-129">lastModifiedDateTime</span></span>|<span data-ttu-id="e3e74-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3e74-130">DateTimeOffset</span></span>|<span data-ttu-id="e3e74-131">上次修改资源时刻。</span><span class="sxs-lookup"><span data-stu-id="e3e74-131">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="e3e74-132">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="e3e74-132">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e3e74-133">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e3e74-133">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3e74-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3e74-134">JSON representation</span></span>

<span data-ttu-id="e3e74-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3e74-135">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->