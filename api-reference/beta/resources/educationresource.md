---
title: educationResource 资源类型
description: 超类别的系统中的所有资源对象。 资源相关联的**工作分配**和/或**提交**，该对象表示正在学习对象
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 87b19f849e24f1780a1d13c7aa1b3eb83543fdec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523216"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="16b50-104">educationResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="16b50-104">educationResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16b50-105">超类别的系统中的所有资源对象。</span><span class="sxs-lookup"><span data-stu-id="16b50-105">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="16b50-106">资源相关联的**工作分配**和/或**提交**，该对象表示正在学习对象分发或传递。</span><span class="sxs-lookup"><span data-stu-id="16b50-106">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="16b50-107">不能直接调用实例化资源您必须进行子类表示正在使用的资源的类型。</span><span class="sxs-lookup"><span data-stu-id="16b50-107">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="16b50-108">此资源存储跨所有资源类型的通用属性。</span><span class="sxs-lookup"><span data-stu-id="16b50-108">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="16b50-109">属性</span><span class="sxs-lookup"><span data-stu-id="16b50-109">Properties</span></span>
| <span data-ttu-id="16b50-110">属性</span><span class="sxs-lookup"><span data-stu-id="16b50-110">Property</span></span>     | <span data-ttu-id="16b50-111">类型</span><span class="sxs-lookup"><span data-stu-id="16b50-111">Type</span></span>   |<span data-ttu-id="16b50-112">说明</span><span class="sxs-lookup"><span data-stu-id="16b50-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16b50-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="16b50-113">createdBy</span></span>|[<span data-ttu-id="16b50-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="16b50-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="16b50-115">资源创建者。</span><span class="sxs-lookup"><span data-stu-id="16b50-115">Who created the resource.</span></span>|
|<span data-ttu-id="16b50-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16b50-116">createdDateTime</span></span>|<span data-ttu-id="16b50-117">创建资源时时刻。</span><span class="sxs-lookup"><span data-stu-id="16b50-117">Moment in time when the resource was created.</span></span>  <span data-ttu-id="16b50-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16b50-118">DateTimeOffset</span></span>|<span data-ttu-id="16b50-p104">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="16b50-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="16b50-121">displayName</span><span class="sxs-lookup"><span data-stu-id="16b50-121">displayName</span></span>|<span data-ttu-id="16b50-122">String</span><span class="sxs-lookup"><span data-stu-id="16b50-122">String</span></span>|<span data-ttu-id="16b50-123">显示资源的名称。</span><span class="sxs-lookup"><span data-stu-id="16b50-123">Display name of resource.</span></span>|
|<span data-ttu-id="16b50-124">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="16b50-124">lastModifiedBy</span></span>|[<span data-ttu-id="16b50-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="16b50-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="16b50-126">谁是最后一个用户修改的资源。</span><span class="sxs-lookup"><span data-stu-id="16b50-126">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="16b50-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16b50-127">lastModifiedDateTime</span></span>|<span data-ttu-id="16b50-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16b50-128">DateTimeOffset</span></span>|<span data-ttu-id="16b50-129">上次修改资源时刻。</span><span class="sxs-lookup"><span data-stu-id="16b50-129">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="16b50-130">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="16b50-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="16b50-131">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="16b50-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16b50-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16b50-132">JSON representation</span></span>

<span data-ttu-id="16b50-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16b50-133">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
