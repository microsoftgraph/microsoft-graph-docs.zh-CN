---
title: educationResource 资源类型
description: 系统中所有 resource 对象的超类。 资源与**工作分配**和/或**提交**相关联, 表示学习对象
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 87b19f849e24f1780a1d13c7aa1b3eb83543fdec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542860"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="689ed-104">educationResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="689ed-104">educationResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="689ed-105">系统中所有 resource 对象的超类。</span><span class="sxs-lookup"><span data-stu-id="689ed-105">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="689ed-106">资源与**工作分配**和/或**提交**相关联, 表示正在向外传递或传递的学习对象。</span><span class="sxs-lookup"><span data-stu-id="689ed-106">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="689ed-107">您不能直接实例化资源;您必须创建一个将代表所用资源类型的子类。</span><span class="sxs-lookup"><span data-stu-id="689ed-107">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="689ed-108">此资源在所有资源类型中存储通用属性。</span><span class="sxs-lookup"><span data-stu-id="689ed-108">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="689ed-109">属性</span><span class="sxs-lookup"><span data-stu-id="689ed-109">Properties</span></span>
| <span data-ttu-id="689ed-110">属性</span><span class="sxs-lookup"><span data-stu-id="689ed-110">Property</span></span>     | <span data-ttu-id="689ed-111">类型</span><span class="sxs-lookup"><span data-stu-id="689ed-111">Type</span></span>   |<span data-ttu-id="689ed-112">说明</span><span class="sxs-lookup"><span data-stu-id="689ed-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="689ed-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="689ed-113">createdBy</span></span>|[<span data-ttu-id="689ed-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="689ed-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="689ed-115">创建资源的作者。</span><span class="sxs-lookup"><span data-stu-id="689ed-115">Who created the resource.</span></span>|
|<span data-ttu-id="689ed-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="689ed-116">createdDateTime</span></span>|<span data-ttu-id="689ed-117">创建资源的时间点。</span><span class="sxs-lookup"><span data-stu-id="689ed-117">Moment in time when the resource was created.</span></span>  <span data-ttu-id="689ed-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="689ed-118">DateTimeOffset</span></span>|<span data-ttu-id="689ed-p104">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="689ed-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="689ed-121">displayName</span><span class="sxs-lookup"><span data-stu-id="689ed-121">displayName</span></span>|<span data-ttu-id="689ed-122">String</span><span class="sxs-lookup"><span data-stu-id="689ed-122">String</span></span>|<span data-ttu-id="689ed-123">资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="689ed-123">Display name of resource.</span></span>|
|<span data-ttu-id="689ed-124">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="689ed-124">lastModifiedBy</span></span>|[<span data-ttu-id="689ed-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="689ed-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="689ed-126">谁是修改资源的最后一个用户。</span><span class="sxs-lookup"><span data-stu-id="689ed-126">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="689ed-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="689ed-127">lastModifiedDateTime</span></span>|<span data-ttu-id="689ed-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="689ed-128">DateTimeOffset</span></span>|<span data-ttu-id="689ed-129">上次修改资源的时间点。</span><span class="sxs-lookup"><span data-stu-id="689ed-129">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="689ed-130">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="689ed-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="689ed-131">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="689ed-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="689ed-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="689ed-132">JSON representation</span></span>

<span data-ttu-id="689ed-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="689ed-133">The following is a JSON representation of the resource.</span></span>

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
