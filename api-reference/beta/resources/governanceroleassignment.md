---
title: governanceRoleAssignment 资源类型
description: 代表向角色分配的用户或组。
ms.openlocfilehash: 3b0520f4641c961358b2db990914fbdf8de254f8
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191135"
---
# <a name="governanceroleassignment-resource-type"></a><span data-ttu-id="b173c-103">governanceRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="b173c-103">governanceRoleAssignment resource type</span></span>
> <span data-ttu-id="b173c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b173c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b173c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b173c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b173c-106">代表向角色分配的用户或组。</span><span class="sxs-lookup"><span data-stu-id="b173c-106">Represents the assignment of a user or group to a role.</span></span>

<span data-ttu-id="b173c-107">特权标识管理 (PIM) 支持两种类型的工作分配：</span><span class="sxs-lookup"><span data-stu-id="b173c-107">Privileged Identity Management (PIM) supports two types of assignments:</span></span>

1. <span data-ttu-id="b173c-108">活动的工作分配-表示激活直接/资源访问权限。</span><span class="sxs-lookup"><span data-stu-id="b173c-108">Active assignment - Represents the direct/activated access to resources.</span></span>
2. <span data-ttu-id="b173c-109">合格的工作分配的资源，之间没有访问和直接访问代表中间阶段的访问权限。</span><span class="sxs-lookup"><span data-stu-id="b173c-109">Eligible assignment - Represents an intermediate stage of privileged access to resources, between no access and direct access.</span></span> <span data-ttu-id="b173c-110">管理员可以分配给用户/组`eligible assignment`提前，每当和需要访问时，`activation`上`eligible assignment`需要几个小时才能资源即时访问。</span><span class="sxs-lookup"><span data-stu-id="b173c-110">Administrators can assign users/groups to `eligible assignment` in advance, and whenever the access is needed, `activation` on the `eligible assignment` is needed to gain the instant access to the resource for several hours.</span></span> <span data-ttu-id="b173c-111">激活之后，`active assignment`将创建为以指示的激活的状态的用户/组成员。</span><span class="sxs-lookup"><span data-stu-id="b173c-111">After activation, an `active assignment` will be created for the users/group members to indicate the activated status.</span></span>

## <a name="methods"></a><span data-ttu-id="b173c-112">方法</span><span class="sxs-lookup"><span data-stu-id="b173c-112">Methods</span></span>

| <span data-ttu-id="b173c-113">方法</span><span class="sxs-lookup"><span data-stu-id="b173c-113">Method</span></span>          | <span data-ttu-id="b173c-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="b173c-114">Return Type</span></span> |<span data-ttu-id="b173c-115">说明</span><span class="sxs-lookup"><span data-stu-id="b173c-115">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="b173c-116">Get</span><span class="sxs-lookup"><span data-stu-id="b173c-116">Get</span></span>](../api/governanceroleassignment-get.md) |  [<span data-ttu-id="b173c-117">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b173c-117">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md) |<span data-ttu-id="b173c-118">读取属性和角色分配实体的关系。</span><span class="sxs-lookup"><span data-stu-id="b173c-118">Read properties and relationships of a role assignment entity.</span></span>|
|[<span data-ttu-id="b173c-119">List</span><span class="sxs-lookup"><span data-stu-id="b173c-119">List</span></span>](../api/governanceroleassignment-list.md) | <span data-ttu-id="b173c-120">[governanceRoleAssignment](../resources/governanceroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="b173c-120">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="b173c-121">列出角色分配对资源的集合。</span><span class="sxs-lookup"><span data-stu-id="b173c-121">List a collection of role assignments on a resource.</span></span> |
|[<span data-ttu-id="b173c-122">Export</span><span class="sxs-lookup"><span data-stu-id="b173c-122">Export</span></span>](../api/governanceroleassignment-export.md) | <span data-ttu-id="b173c-123">八进制流</span><span class="sxs-lookup"><span data-stu-id="b173c-123">octet-stream</span></span> |<span data-ttu-id="b173c-124">下载的资源角色分配集合，并将另存为`.csv`文件。</span><span class="sxs-lookup"><span data-stu-id="b173c-124">Download a collection of role assignments on a resource and save as a `.csv` file.</span></span>|

<span data-ttu-id="b173c-125">不`POST`， `PUT`， `PATCH`，或`DELETE`支持操作`roleAssignments`实体集。</span><span class="sxs-lookup"><span data-stu-id="b173c-125">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `roleAssignments` entity set.</span></span> <span data-ttu-id="b173c-126">任何创建、 更新和删除操作，在`governanceRoleAssignment`通过完成`governanceRoleAssignmentRequest`。</span><span class="sxs-lookup"><span data-stu-id="b173c-126">Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.</span></span>

## <a name="properties"></a><span data-ttu-id="b173c-127">属性</span><span class="sxs-lookup"><span data-stu-id="b173c-127">Properties</span></span>
| <span data-ttu-id="b173c-128">属性</span><span class="sxs-lookup"><span data-stu-id="b173c-128">Property</span></span>  | <span data-ttu-id="b173c-129">类型</span><span class="sxs-lookup"><span data-stu-id="b173c-129">Type</span></span>      |<span data-ttu-id="b173c-130">说明</span><span class="sxs-lookup"><span data-stu-id="b173c-130">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="b173c-131">id</span><span class="sxs-lookup"><span data-stu-id="b173c-131">id</span></span>         |<span data-ttu-id="b173c-132">字符串</span><span class="sxs-lookup"><span data-stu-id="b173c-132">String</span></span>     |<span data-ttu-id="b173c-133">角色分配的 ID。</span><span class="sxs-lookup"><span data-stu-id="b173c-133">The ID of the role assignment.</span></span> <span data-ttu-id="b173c-134">处于 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="b173c-134">It is in GUID format.</span></span>|
|<span data-ttu-id="b173c-135">resourceId</span><span class="sxs-lookup"><span data-stu-id="b173c-135">resourceId</span></span> |<span data-ttu-id="b173c-136">String</span><span class="sxs-lookup"><span data-stu-id="b173c-136">String</span></span>     |<span data-ttu-id="b173c-137">必需。</span><span class="sxs-lookup"><span data-stu-id="b173c-137">Required.</span></span> <span data-ttu-id="b173c-138">资源的角色分配相关联的 ID。</span><span class="sxs-lookup"><span data-stu-id="b173c-138">The ID of the resource which the role assignment is associated with.</span></span> |
|<span data-ttu-id="b173c-139">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="b173c-139">roleDefinitionId</span></span>|<span data-ttu-id="b173c-140">字符串</span><span class="sxs-lookup"><span data-stu-id="b173c-140">String</span></span>|<span data-ttu-id="b173c-141">必需。</span><span class="sxs-lookup"><span data-stu-id="b173c-141">Required.</span></span> <span data-ttu-id="b173c-142">角色分配相关联的角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="b173c-142">The ID of the role definition which the role assignment is associated with.</span></span> |
|<span data-ttu-id="b173c-143">subjectId</span><span class="sxs-lookup"><span data-stu-id="b173c-143">subjectId</span></span>|<span data-ttu-id="b173c-144">字符串</span><span class="sxs-lookup"><span data-stu-id="b173c-144">String</span></span>       |<span data-ttu-id="b173c-145">必需。</span><span class="sxs-lookup"><span data-stu-id="b173c-145">Required.</span></span> <span data-ttu-id="b173c-146">该角色分配相关联的主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="b173c-146">The ID of the subject which the role assignment is associated with.</span></span> |
|<span data-ttu-id="b173c-147">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="b173c-147">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="b173c-148">字符串</span><span class="sxs-lookup"><span data-stu-id="b173c-148">String</span></span>|<span data-ttu-id="b173c-149">如果这是`active assignment`上创建由于激活和`eligible assignment`，它代表该 ID `eligible assignment`;否则，值为`null`。</span><span class="sxs-lookup"><span data-stu-id="b173c-149">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the ID of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |
|<span data-ttu-id="b173c-150">externalId</span><span class="sxs-lookup"><span data-stu-id="b173c-150">externalId</span></span>   |<span data-ttu-id="b173c-151">String</span><span class="sxs-lookup"><span data-stu-id="b173c-151">String</span></span>     |<span data-ttu-id="b173c-152">外部 ID 用于标识提供程序中的角色分配的资源。</span><span class="sxs-lookup"><span data-stu-id="b173c-152">The external ID the resource that is used to identify the role assignment in the provider.</span></span>|
|<span data-ttu-id="b173c-153">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b173c-153">startDateTime</span></span>|<span data-ttu-id="b173c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b173c-154">DateTimeOffset</span></span>|<span data-ttu-id="b173c-155">角色分配的开始时间。</span><span class="sxs-lookup"><span data-stu-id="b173c-155">The start time of the role assignment.</span></span> <span data-ttu-id="b173c-156">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="b173c-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b173c-157">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b173c-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b173c-158">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b173c-158">endDateTime</span></span>|<span data-ttu-id="b173c-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b173c-159">DateTimeOffset</span></span>|<span data-ttu-id="b173c-160">对于非永久角色分配，这是时将过期的角色分配的时间。</span><span class="sxs-lookup"><span data-stu-id="b173c-160">For a non-permanent role assignment, this is the time when the role assignment will be expired.</span></span> <span data-ttu-id="b173c-161">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="b173c-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b173c-162">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b173c-162">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b173c-163">assignmentState</span><span class="sxs-lookup"><span data-stu-id="b173c-163">assignmentState</span></span>|<span data-ttu-id="b173c-164">字符串</span><span class="sxs-lookup"><span data-stu-id="b173c-164">String</span></span>  |<span data-ttu-id="b173c-165">工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="b173c-165">The state of the assignment.</span></span> <span data-ttu-id="b173c-166">值可以是</span><span class="sxs-lookup"><span data-stu-id="b173c-166">The value can be</span></span> <ul><li> <span data-ttu-id="b173c-167">`Eligible`合格的分配</span><span class="sxs-lookup"><span data-stu-id="b173c-167">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="b173c-168">`Active`-如果直接分配`Active`的管理员，或激活合格工作分配的用户。</span><span class="sxs-lookup"><span data-stu-id="b173c-168">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="b173c-169">memberType</span><span class="sxs-lookup"><span data-stu-id="b173c-169">memberType</span></span>|<span data-ttu-id="b173c-170">字符串</span><span class="sxs-lookup"><span data-stu-id="b173c-170">String</span></span>      |<span data-ttu-id="b173c-171">成员的类型。</span><span class="sxs-lookup"><span data-stu-id="b173c-171">The type of member.</span></span> <span data-ttu-id="b173c-172">值可以是：</span><span class="sxs-lookup"><span data-stu-id="b173c-172">The value can be:</span></span> <ul><li><span data-ttu-id="b173c-173">`Inherited`-角色分配继承自父资源范围</span><span class="sxs-lookup"><span data-stu-id="b173c-173">`Inherited` - the role assignment is inherited from a parent resource scope</span></span></li><li><span data-ttu-id="b173c-174">`Group`-角色分配不继承的但来自的组分配成员身份</span><span class="sxs-lookup"><span data-stu-id="b173c-174">`Group`- the role assignment is not inherited, but comes from the membership of a group assignment</span></span></li><li><span data-ttu-id="b173c-175">`User`-既不继承的角色分配和从组工作分配。</span><span class="sxs-lookup"><span data-stu-id="b173c-175">`User` - the role assignment is neither inherited nor from a group assignment.</span></span></li></ul>|


## <a name="relationships"></a><span data-ttu-id="b173c-176">Relationships</span><span class="sxs-lookup"><span data-stu-id="b173c-176">Relationships</span></span>
| <span data-ttu-id="b173c-177">关系</span><span class="sxs-lookup"><span data-stu-id="b173c-177">Relationship</span></span> | <span data-ttu-id="b173c-178">类型</span><span class="sxs-lookup"><span data-stu-id="b173c-178">Type</span></span>   |<span data-ttu-id="b173c-179">说明</span><span class="sxs-lookup"><span data-stu-id="b173c-179">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b173c-180">资源</span><span class="sxs-lookup"><span data-stu-id="b173c-180">resource</span></span>|[<span data-ttu-id="b173c-181">governanceResource</span><span class="sxs-lookup"><span data-stu-id="b173c-181">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="b173c-182">只读。</span><span class="sxs-lookup"><span data-stu-id="b173c-182">Read-only.</span></span> <span data-ttu-id="b173c-183">与角色分配关联的资源。</span><span class="sxs-lookup"><span data-stu-id="b173c-183">The resource associated with the role assignment.</span></span> |
|<span data-ttu-id="b173c-184">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="b173c-184">roleDefinition</span></span>|[<span data-ttu-id="b173c-185">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="b173c-185">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="b173c-186">只读。</span><span class="sxs-lookup"><span data-stu-id="b173c-186">Read-only.</span></span> <span data-ttu-id="b173c-187">与角色分配相关联的角色定义。</span><span class="sxs-lookup"><span data-stu-id="b173c-187">The role definition associated with the role assignment.</span></span> |
|<span data-ttu-id="b173c-188">subject</span><span class="sxs-lookup"><span data-stu-id="b173c-188">subject</span></span>|[<span data-ttu-id="b173c-189">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="b173c-189">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="b173c-190">只读。</span><span class="sxs-lookup"><span data-stu-id="b173c-190">Read-only.</span></span> <span data-ttu-id="b173c-191">主题的角色分配相关联。</span><span class="sxs-lookup"><span data-stu-id="b173c-191">The subject associated with the role assignment.</span></span> |
|<span data-ttu-id="b173c-192">linkedEligibleRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b173c-192">linkedEligibleRoleAssignment</span></span>|[<span data-ttu-id="b173c-193">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b173c-193">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md)|<span data-ttu-id="b173c-194">只读。</span><span class="sxs-lookup"><span data-stu-id="b173c-194">Read-only.</span></span> <span data-ttu-id="b173c-195">如果这是`active assignment`上创建由于激活和`eligible assignment`，它代表的`eligible assignment`;否则，值为`null`。</span><span class="sxs-lookup"><span data-stu-id="b173c-195">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the object of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b173c-196">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b173c-196">JSON representation</span></span>

<span data-ttu-id="b173c-197">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b173c-197">Here is a JSON representation of the resource.</span></span>


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
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
