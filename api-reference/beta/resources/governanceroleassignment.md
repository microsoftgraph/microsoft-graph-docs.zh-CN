---
title: governanceRoleAssignment 资源类型
description: 代表向角色分配的用户或组。
localization_priority: Normal
ms.openlocfilehash: 77a5238aa337dd8d273d3156d285e081c4bc8875
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512680"
---
# <a name="governanceroleassignment-resource-type"></a><span data-ttu-id="9e507-103">governanceRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e507-103">governanceRoleAssignment resource type</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e507-104">代表向角色分配的用户或组。</span><span class="sxs-lookup"><span data-stu-id="9e507-104">Represents the assignment of a user or group to a role.</span></span>

<span data-ttu-id="9e507-105">特权标识管理 (PIM) 支持两种类型的工作分配：</span><span class="sxs-lookup"><span data-stu-id="9e507-105">Privileged Identity Management (PIM) supports two types of assignments:</span></span>

1. <span data-ttu-id="9e507-106">活动的工作分配-表示激活直接/资源访问权限。</span><span class="sxs-lookup"><span data-stu-id="9e507-106">Active assignment - Represents the direct/activated access to resources.</span></span>
2. <span data-ttu-id="9e507-107">合格的工作分配的资源，之间没有访问和直接访问代表中间阶段的访问权限。</span><span class="sxs-lookup"><span data-stu-id="9e507-107">Eligible assignment - Represents an intermediate stage of privileged access to resources, between no access and direct access.</span></span> <span data-ttu-id="9e507-108">管理员可以分配给用户/组`eligible assignment`提前，每当和需要访问时，`activation`上`eligible assignment`需要几个小时才能资源即时访问。</span><span class="sxs-lookup"><span data-stu-id="9e507-108">Administrators can assign users/groups to `eligible assignment` in advance, and whenever the access is needed, `activation` on the `eligible assignment` is needed to gain the instant access to the resource for several hours.</span></span> <span data-ttu-id="9e507-109">激活之后，`active assignment`将创建为以指示的激活的状态的用户/组成员。</span><span class="sxs-lookup"><span data-stu-id="9e507-109">After activation, an `active assignment` will be created for the users/group members to indicate the activated status.</span></span>

## <a name="methods"></a><span data-ttu-id="9e507-110">方法</span><span class="sxs-lookup"><span data-stu-id="9e507-110">Methods</span></span>

| <span data-ttu-id="9e507-111">方法</span><span class="sxs-lookup"><span data-stu-id="9e507-111">Method</span></span>          | <span data-ttu-id="9e507-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="9e507-112">Return Type</span></span> |<span data-ttu-id="9e507-113">说明</span><span class="sxs-lookup"><span data-stu-id="9e507-113">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="9e507-114">Get</span><span class="sxs-lookup"><span data-stu-id="9e507-114">Get</span></span>](../api/governanceroleassignment-get.md) |  [<span data-ttu-id="9e507-115">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9e507-115">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md) |<span data-ttu-id="9e507-116">读取属性和角色分配实体的关系。</span><span class="sxs-lookup"><span data-stu-id="9e507-116">Read properties and relationships of a role assignment entity.</span></span>|
|[<span data-ttu-id="9e507-117">List</span><span class="sxs-lookup"><span data-stu-id="9e507-117">List</span></span>](../api/governanceroleassignment-list.md) | <span data-ttu-id="9e507-118">[governanceRoleAssignment](../resources/governanceroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="9e507-118">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="9e507-119">列出角色分配对资源的集合。</span><span class="sxs-lookup"><span data-stu-id="9e507-119">List a collection of role assignments on a resource.</span></span> |
|[<span data-ttu-id="9e507-120">Export</span><span class="sxs-lookup"><span data-stu-id="9e507-120">Export</span></span>](../api/governanceroleassignment-export.md) | <span data-ttu-id="9e507-121">八进制流</span><span class="sxs-lookup"><span data-stu-id="9e507-121">octet-stream</span></span> |<span data-ttu-id="9e507-122">下载的资源角色分配集合，并将另存为`.csv`文件。</span><span class="sxs-lookup"><span data-stu-id="9e507-122">Download a collection of role assignments on a resource and save as a `.csv` file.</span></span>|

<span data-ttu-id="9e507-123">不`POST`， `PUT`， `PATCH`，或`DELETE`支持操作`roleAssignments`实体集。</span><span class="sxs-lookup"><span data-stu-id="9e507-123">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `roleAssignments` entity set.</span></span> <span data-ttu-id="9e507-124">任何创建、 更新和删除操作，在`governanceRoleAssignment`通过完成`governanceRoleAssignmentRequest`。</span><span class="sxs-lookup"><span data-stu-id="9e507-124">Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.</span></span>

## <a name="properties"></a><span data-ttu-id="9e507-125">属性</span><span class="sxs-lookup"><span data-stu-id="9e507-125">Properties</span></span>
| <span data-ttu-id="9e507-126">属性</span><span class="sxs-lookup"><span data-stu-id="9e507-126">Property</span></span>  | <span data-ttu-id="9e507-127">类型</span><span class="sxs-lookup"><span data-stu-id="9e507-127">Type</span></span>      |<span data-ttu-id="9e507-128">说明</span><span class="sxs-lookup"><span data-stu-id="9e507-128">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="9e507-129">id</span><span class="sxs-lookup"><span data-stu-id="9e507-129">id</span></span>         |<span data-ttu-id="9e507-130">字符串</span><span class="sxs-lookup"><span data-stu-id="9e507-130">String</span></span>     |<span data-ttu-id="9e507-131">角色分配的 ID。</span><span class="sxs-lookup"><span data-stu-id="9e507-131">The ID of the role assignment.</span></span> <span data-ttu-id="9e507-132">处于 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="9e507-132">It is in GUID format.</span></span>|
|<span data-ttu-id="9e507-133">resourceId</span><span class="sxs-lookup"><span data-stu-id="9e507-133">resourceId</span></span> |<span data-ttu-id="9e507-134">String</span><span class="sxs-lookup"><span data-stu-id="9e507-134">String</span></span>     |<span data-ttu-id="9e507-135">必需。</span><span class="sxs-lookup"><span data-stu-id="9e507-135">Required.</span></span> <span data-ttu-id="9e507-136">资源的角色分配相关联的 ID。</span><span class="sxs-lookup"><span data-stu-id="9e507-136">The ID of the resource which the role assignment is associated with.</span></span> |
|<span data-ttu-id="9e507-137">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="9e507-137">roleDefinitionId</span></span>|<span data-ttu-id="9e507-138">String</span><span class="sxs-lookup"><span data-stu-id="9e507-138">String</span></span>|<span data-ttu-id="9e507-139">必需。</span><span class="sxs-lookup"><span data-stu-id="9e507-139">Required.</span></span> <span data-ttu-id="9e507-140">角色分配相关联的角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="9e507-140">The ID of the role definition which the role assignment is associated with.</span></span> |
|<span data-ttu-id="9e507-141">subjectId</span><span class="sxs-lookup"><span data-stu-id="9e507-141">subjectId</span></span>|<span data-ttu-id="9e507-142">String</span><span class="sxs-lookup"><span data-stu-id="9e507-142">String</span></span>       |<span data-ttu-id="9e507-143">必需。</span><span class="sxs-lookup"><span data-stu-id="9e507-143">Required.</span></span> <span data-ttu-id="9e507-144">该角色分配相关联的主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="9e507-144">The ID of the subject which the role assignment is associated with.</span></span> |
|<span data-ttu-id="9e507-145">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="9e507-145">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="9e507-146">String</span><span class="sxs-lookup"><span data-stu-id="9e507-146">String</span></span>|<span data-ttu-id="9e507-147">如果这是`active assignment`上创建由于激活和`eligible assignment`，它代表该 ID `eligible assignment`;否则，值为`null`。</span><span class="sxs-lookup"><span data-stu-id="9e507-147">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the ID of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |
|<span data-ttu-id="9e507-148">externalId</span><span class="sxs-lookup"><span data-stu-id="9e507-148">externalId</span></span>   |<span data-ttu-id="9e507-149">String</span><span class="sxs-lookup"><span data-stu-id="9e507-149">String</span></span>     |<span data-ttu-id="9e507-150">外部 ID 用于标识提供程序中的角色分配的资源。</span><span class="sxs-lookup"><span data-stu-id="9e507-150">The external ID the resource that is used to identify the role assignment in the provider.</span></span>|
|<span data-ttu-id="9e507-151">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9e507-151">startDateTime</span></span>|<span data-ttu-id="9e507-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e507-152">DateTimeOffset</span></span>|<span data-ttu-id="9e507-153">角色分配的开始时间。</span><span class="sxs-lookup"><span data-stu-id="9e507-153">The start time of the role assignment.</span></span> <span data-ttu-id="9e507-154">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="9e507-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9e507-155">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9e507-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9e507-156">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9e507-156">endDateTime</span></span>|<span data-ttu-id="9e507-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e507-157">DateTimeOffset</span></span>|<span data-ttu-id="9e507-158">对于非永久角色分配，这是时将过期的角色分配的时间。</span><span class="sxs-lookup"><span data-stu-id="9e507-158">For a non-permanent role assignment, this is the time when the role assignment will be expired.</span></span> <span data-ttu-id="9e507-159">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="9e507-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9e507-160">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9e507-160">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9e507-161">assignmentState</span><span class="sxs-lookup"><span data-stu-id="9e507-161">assignmentState</span></span>|<span data-ttu-id="9e507-162">String</span><span class="sxs-lookup"><span data-stu-id="9e507-162">String</span></span>  |<span data-ttu-id="9e507-163">工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="9e507-163">The state of the assignment.</span></span> <span data-ttu-id="9e507-164">值可以是</span><span class="sxs-lookup"><span data-stu-id="9e507-164">The value can be</span></span> <ul><li> <span data-ttu-id="9e507-165">`Eligible`合格的分配</span><span class="sxs-lookup"><span data-stu-id="9e507-165">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="9e507-166">`Active`-如果直接分配`Active`的管理员，或激活合格工作分配的用户。</span><span class="sxs-lookup"><span data-stu-id="9e507-166">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="9e507-167">MemberType</span><span class="sxs-lookup"><span data-stu-id="9e507-167">memberType</span></span>|<span data-ttu-id="9e507-168">String</span><span class="sxs-lookup"><span data-stu-id="9e507-168">String</span></span>      |<span data-ttu-id="9e507-169">成员的类型。</span><span class="sxs-lookup"><span data-stu-id="9e507-169">The type of member.</span></span> <span data-ttu-id="9e507-170">值可以是：</span><span class="sxs-lookup"><span data-stu-id="9e507-170">The value can be:</span></span> <ul><li><span data-ttu-id="9e507-171">`Inherited`-角色分配继承自父资源范围</span><span class="sxs-lookup"><span data-stu-id="9e507-171">`Inherited` - the role assignment is inherited from a parent resource scope</span></span></li><li><span data-ttu-id="9e507-172">`Group`-角色分配不继承的但来自的组分配成员身份</span><span class="sxs-lookup"><span data-stu-id="9e507-172">`Group`- the role assignment is not inherited, but comes from the membership of a group assignment</span></span></li><li><span data-ttu-id="9e507-173">`User`-既不继承的角色分配和从组工作分配。</span><span class="sxs-lookup"><span data-stu-id="9e507-173">`User` - the role assignment is neither inherited nor from a group assignment.</span></span></li></ul>|


## <a name="relationships"></a><span data-ttu-id="9e507-174">关系</span><span class="sxs-lookup"><span data-stu-id="9e507-174">Relationships</span></span>
| <span data-ttu-id="9e507-175">关系</span><span class="sxs-lookup"><span data-stu-id="9e507-175">Relationship</span></span> | <span data-ttu-id="9e507-176">类型</span><span class="sxs-lookup"><span data-stu-id="9e507-176">Type</span></span>   |<span data-ttu-id="9e507-177">说明</span><span class="sxs-lookup"><span data-stu-id="9e507-177">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e507-178">资源</span><span class="sxs-lookup"><span data-stu-id="9e507-178">resource</span></span>|[<span data-ttu-id="9e507-179">governanceResource</span><span class="sxs-lookup"><span data-stu-id="9e507-179">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="9e507-180">只读。</span><span class="sxs-lookup"><span data-stu-id="9e507-180">Read-only.</span></span> <span data-ttu-id="9e507-181">与角色分配关联的资源。</span><span class="sxs-lookup"><span data-stu-id="9e507-181">The resource associated with the role assignment.</span></span> |
|<span data-ttu-id="9e507-182">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9e507-182">roleDefinition</span></span>|[<span data-ttu-id="9e507-183">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9e507-183">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="9e507-184">只读。</span><span class="sxs-lookup"><span data-stu-id="9e507-184">Read-only.</span></span> <span data-ttu-id="9e507-185">与角色分配相关联的角色定义。</span><span class="sxs-lookup"><span data-stu-id="9e507-185">The role definition associated with the role assignment.</span></span> |
|<span data-ttu-id="9e507-186">subject</span><span class="sxs-lookup"><span data-stu-id="9e507-186">subject</span></span>|[<span data-ttu-id="9e507-187">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="9e507-187">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="9e507-188">只读。</span><span class="sxs-lookup"><span data-stu-id="9e507-188">Read-only.</span></span> <span data-ttu-id="9e507-189">主题的角色分配相关联。</span><span class="sxs-lookup"><span data-stu-id="9e507-189">The subject associated with the role assignment.</span></span> |
|<span data-ttu-id="9e507-190">linkedEligibleRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9e507-190">linkedEligibleRoleAssignment</span></span>|[<span data-ttu-id="9e507-191">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9e507-191">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md)|<span data-ttu-id="9e507-192">只读。</span><span class="sxs-lookup"><span data-stu-id="9e507-192">Read-only.</span></span> <span data-ttu-id="9e507-193">如果这是`active assignment`上创建由于激活和`eligible assignment`，它代表的`eligible assignment`;否则，值为`null`。</span><span class="sxs-lookup"><span data-stu-id="9e507-193">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the object of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9e507-194">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e507-194">JSON representation</span></span>

<span data-ttu-id="9e507-195">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e507-195">Here is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "linkedEligibleRoleAssignmentId": "String",
  "externalId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "assignmentState": "String",
  "memberType": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroleassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
