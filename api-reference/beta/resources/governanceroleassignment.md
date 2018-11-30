---
title: governanceRoleAssignment 资源类型
description: 代表向角色分配的用户或组。
ms.openlocfilehash: e29ab163c837ee04f141bdc496abeac760d6a372
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042146"
---
# <a name="governanceroleassignment-resource-type"></a><span data-ttu-id="42b00-103">governanceRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="42b00-103">governanceRoleAssignment resource type</span></span>
> <span data-ttu-id="42b00-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="42b00-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42b00-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="42b00-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="42b00-106">代表向角色分配的用户或组。</span><span class="sxs-lookup"><span data-stu-id="42b00-106">Represents the assignment of a user or group to a role.</span></span>

<span data-ttu-id="42b00-107">特权标识管理 (PIM) 支持两种类型的工作分配：</span><span class="sxs-lookup"><span data-stu-id="42b00-107">Privileged Identity Management (PIM) supports two types of assignments:</span></span>

1. <span data-ttu-id="42b00-108">活动的工作分配-资源表示直接访问。</span><span class="sxs-lookup"><span data-stu-id="42b00-108">Active assignment - Represents the direct access to resources.</span></span>
2. <span data-ttu-id="42b00-109">合格的工作分配的资源，之间没有访问和直接访问代表中间阶段的访问权限。</span><span class="sxs-lookup"><span data-stu-id="42b00-109">Eligible assignment - Represents an intermediate stage of privileged access to resources, between no access and direct access.</span></span> <span data-ttu-id="42b00-110">管理员可以暂时分配到的用户/组`eligible assignment`提前。</span><span class="sxs-lookup"><span data-stu-id="42b00-110">Administrators can temporarily assign users/groups to `eligible assignment` in advance.</span></span> <span data-ttu-id="42b00-111">只要用户/组成员，需要访问`activation`上`eligible assignment`需要几个小时才能资源即时访问。</span><span class="sxs-lookup"><span data-stu-id="42b00-111">Whenever the access is needed for users/group members, `activation` on the `eligible assignment` is needed to gain the instant access to the resource for several hours.</span></span> <span data-ttu-id="42b00-112">激活之后，`active assignment`将创建为以指示的激活的状态的用户/组成员。</span><span class="sxs-lookup"><span data-stu-id="42b00-112">After activation, an `active assignment` will be created for the users/group members to indicate the activated status.</span></span>

## <a name="methods"></a><span data-ttu-id="42b00-113">方法</span><span class="sxs-lookup"><span data-stu-id="42b00-113">Methods</span></span>

| <span data-ttu-id="42b00-114">方法</span><span class="sxs-lookup"><span data-stu-id="42b00-114">Method</span></span>          | <span data-ttu-id="42b00-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="42b00-115">Return Type</span></span> |<span data-ttu-id="42b00-116">说明</span><span class="sxs-lookup"><span data-stu-id="42b00-116">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="42b00-117">Get</span><span class="sxs-lookup"><span data-stu-id="42b00-117">Get</span></span>](../api/governanceroleassignment-get.md) |  [<span data-ttu-id="42b00-118">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="42b00-118">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md) |<span data-ttu-id="42b00-119">读取属性和角色分配实体的关系。</span><span class="sxs-lookup"><span data-stu-id="42b00-119">Read properties and relationships of a role assignment entity.</span></span>|
|[<span data-ttu-id="42b00-120">List</span><span class="sxs-lookup"><span data-stu-id="42b00-120">List</span></span>](../api/governanceroleassignment-list.md) | <span data-ttu-id="42b00-121">[governanceRoleAssignment](../resources/governanceroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="42b00-121">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="42b00-122">列出角色分配对资源的集合。</span><span class="sxs-lookup"><span data-stu-id="42b00-122">List a collection of role assignments on a resource.</span></span> |
|[<span data-ttu-id="42b00-123">Export</span><span class="sxs-lookup"><span data-stu-id="42b00-123">Export</span></span>](../api/governanceroleassignment-export.md) | <span data-ttu-id="42b00-124">八进制流</span><span class="sxs-lookup"><span data-stu-id="42b00-124">octet-stream</span></span> |<span data-ttu-id="42b00-125">下载的资源角色分配集合，并将另存为`.csv`文件。</span><span class="sxs-lookup"><span data-stu-id="42b00-125">Download a collection of role assignments on a resource and save as a `.csv` file.</span></span>|

<span data-ttu-id="42b00-126">不`POST`， `PUT`， `PATCH`，或`DELETE`支持操作`roleAssignments`实体集。</span><span class="sxs-lookup"><span data-stu-id="42b00-126">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `roleAssignments` entity set.</span></span> <span data-ttu-id="42b00-127">任何创建、 更新和删除操作，在`governanceRoleAssignment`通过完成`governanceRoleAssignmentRequest`。</span><span class="sxs-lookup"><span data-stu-id="42b00-127">Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.</span></span>

## <a name="properties"></a><span data-ttu-id="42b00-128">属性</span><span class="sxs-lookup"><span data-stu-id="42b00-128">Properties</span></span>
| <span data-ttu-id="42b00-129">属性</span><span class="sxs-lookup"><span data-stu-id="42b00-129">Property</span></span>  | <span data-ttu-id="42b00-130">类型</span><span class="sxs-lookup"><span data-stu-id="42b00-130">Type</span></span>      |<span data-ttu-id="42b00-131">说明</span><span class="sxs-lookup"><span data-stu-id="42b00-131">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="42b00-132">id</span><span class="sxs-lookup"><span data-stu-id="42b00-132">id</span></span>         |<span data-ttu-id="42b00-133">字符串</span><span class="sxs-lookup"><span data-stu-id="42b00-133">String</span></span>     |<span data-ttu-id="42b00-134">角色分配的 ID。</span><span class="sxs-lookup"><span data-stu-id="42b00-134">The ID of the role assignment.</span></span> <span data-ttu-id="42b00-135">处于 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="42b00-135">It is in GUID format.</span></span>|
|<span data-ttu-id="42b00-136">resourceId</span><span class="sxs-lookup"><span data-stu-id="42b00-136">resourceId</span></span> |<span data-ttu-id="42b00-137">String</span><span class="sxs-lookup"><span data-stu-id="42b00-137">String</span></span>     |<span data-ttu-id="42b00-138">必需项。</span><span class="sxs-lookup"><span data-stu-id="42b00-138">Required.</span></span> <span data-ttu-id="42b00-139">资源的角色分配相关联的 ID。</span><span class="sxs-lookup"><span data-stu-id="42b00-139">The ID of the resource which the role assignment is associated with.</span></span> |
|<span data-ttu-id="42b00-140">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="42b00-140">roleDefinitionId</span></span>|<span data-ttu-id="42b00-141">字符串</span><span class="sxs-lookup"><span data-stu-id="42b00-141">String</span></span>|<span data-ttu-id="42b00-142">必需项。</span><span class="sxs-lookup"><span data-stu-id="42b00-142">Required.</span></span> <span data-ttu-id="42b00-143">角色分配相关联的角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="42b00-143">The ID of the role definition which the role assignment is associated with.</span></span> |
|<span data-ttu-id="42b00-144">subjectId</span><span class="sxs-lookup"><span data-stu-id="42b00-144">subjectId</span></span>|<span data-ttu-id="42b00-145">字符串</span><span class="sxs-lookup"><span data-stu-id="42b00-145">String</span></span>       |<span data-ttu-id="42b00-146">必需项。</span><span class="sxs-lookup"><span data-stu-id="42b00-146">Required.</span></span> <span data-ttu-id="42b00-147">该角色分配相关联的主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="42b00-147">The ID of the subject which the role assignment is associated with.</span></span> |
|<span data-ttu-id="42b00-148">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="42b00-148">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="42b00-149">字符串</span><span class="sxs-lookup"><span data-stu-id="42b00-149">String</span></span>|<span data-ttu-id="42b00-150">如果这是`active assignment`上创建由于激活和`eligible assignment`，它代表该 ID `eligible assignment`;否则，值为`null`。</span><span class="sxs-lookup"><span data-stu-id="42b00-150">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the ID of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |
|<span data-ttu-id="42b00-151">externalId</span><span class="sxs-lookup"><span data-stu-id="42b00-151">externalId</span></span>   |<span data-ttu-id="42b00-152">String</span><span class="sxs-lookup"><span data-stu-id="42b00-152">String</span></span>     |<span data-ttu-id="42b00-153">外部 ID 用于标识提供程序中的角色分配的资源。</span><span class="sxs-lookup"><span data-stu-id="42b00-153">The external ID the resource that is used to identify the role assignment in the provider.</span></span>|
|<span data-ttu-id="42b00-154">isPermanent</span><span class="sxs-lookup"><span data-stu-id="42b00-154">isPermanent</span></span>|<span data-ttu-id="42b00-155">布尔</span><span class="sxs-lookup"><span data-stu-id="42b00-155">Boolean</span></span>    |<span data-ttu-id="42b00-156">指示该角色分配是否是一个永久的分配。</span><span class="sxs-lookup"><span data-stu-id="42b00-156">Indicates whether the role assignment is a permanent assignment.</span></span>|
|<span data-ttu-id="42b00-157">startDateTime</span><span class="sxs-lookup"><span data-stu-id="42b00-157">startDateTime</span></span>|<span data-ttu-id="42b00-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42b00-158">DateTimeOffset</span></span>|<span data-ttu-id="42b00-159">角色分配的开始时间。</span><span class="sxs-lookup"><span data-stu-id="42b00-159">The start time of the role assignment.</span></span> <span data-ttu-id="42b00-160">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="42b00-160">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="42b00-161">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="42b00-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="42b00-162">endDateTime</span><span class="sxs-lookup"><span data-stu-id="42b00-162">endDateTime</span></span>|<span data-ttu-id="42b00-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42b00-163">DateTimeOffset</span></span>|<span data-ttu-id="42b00-164">对于非永久角色分配，这是时将过期的角色分配的时间。</span><span class="sxs-lookup"><span data-stu-id="42b00-164">For a non-permanent role assignment, this is the time when the role assignment will be expired.</span></span> <span data-ttu-id="42b00-165">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="42b00-165">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="42b00-166">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="42b00-166">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="42b00-167">assignmentState</span><span class="sxs-lookup"><span data-stu-id="42b00-167">assignmentState</span></span>|<span data-ttu-id="42b00-168">字符串</span><span class="sxs-lookup"><span data-stu-id="42b00-168">String</span></span>  |<span data-ttu-id="42b00-169">工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="42b00-169">The state of the assignment.</span></span> <span data-ttu-id="42b00-170">值可以是</span><span class="sxs-lookup"><span data-stu-id="42b00-170">The value can be</span></span> <ul><li> <span data-ttu-id="42b00-171">`Eligible`合格的分配</span><span class="sxs-lookup"><span data-stu-id="42b00-171">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="42b00-172">`Active`-如果直接分配`Active`的管理员，或激活合格工作分配的用户。</span><span class="sxs-lookup"><span data-stu-id="42b00-172">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="42b00-173">memberType</span><span class="sxs-lookup"><span data-stu-id="42b00-173">memberType</span></span>|<span data-ttu-id="42b00-174">字符串</span><span class="sxs-lookup"><span data-stu-id="42b00-174">String</span></span>      |<span data-ttu-id="42b00-175">成员的类型。</span><span class="sxs-lookup"><span data-stu-id="42b00-175">The type of member.</span></span> <span data-ttu-id="42b00-176">值可以是：</span><span class="sxs-lookup"><span data-stu-id="42b00-176">The value can be:</span></span> <ul><li><span data-ttu-id="42b00-177">`Inherited`-角色分配继承自父资源范围</span><span class="sxs-lookup"><span data-stu-id="42b00-177">`Inherited` - the role assignment is inherited from a parent resource scope</span></span></li><li><span data-ttu-id="42b00-178">`Group`-角色分配不继承的但来自的组分配成员身份</span><span class="sxs-lookup"><span data-stu-id="42b00-178">`Group`- the role assignment is not inherited, but comes from the membership of a group assignment</span></span></li><li><span data-ttu-id="42b00-179">`User`-既不继承的角色分配和从组工作分配。</span><span class="sxs-lookup"><span data-stu-id="42b00-179">`User` - the role assignment is neither inherited nor from a group assignment.</span></span></li></ul>|


## <a name="relationships"></a><span data-ttu-id="42b00-180">Relationships</span><span class="sxs-lookup"><span data-stu-id="42b00-180">Relationships</span></span>
| <span data-ttu-id="42b00-181">关系</span><span class="sxs-lookup"><span data-stu-id="42b00-181">Relationship</span></span> | <span data-ttu-id="42b00-182">类型</span><span class="sxs-lookup"><span data-stu-id="42b00-182">Type</span></span>   |<span data-ttu-id="42b00-183">说明</span><span class="sxs-lookup"><span data-stu-id="42b00-183">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42b00-184">资源</span><span class="sxs-lookup"><span data-stu-id="42b00-184">resource</span></span>|[<span data-ttu-id="42b00-185">governanceResource</span><span class="sxs-lookup"><span data-stu-id="42b00-185">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="42b00-186">只读。</span><span class="sxs-lookup"><span data-stu-id="42b00-186">Read-only.</span></span> <span data-ttu-id="42b00-187">与角色分配关联的资源。</span><span class="sxs-lookup"><span data-stu-id="42b00-187">The resource associated with the role assignment.</span></span> |
|<span data-ttu-id="42b00-188">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="42b00-188">roleDefinition</span></span>|[<span data-ttu-id="42b00-189">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="42b00-189">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="42b00-190">只读。</span><span class="sxs-lookup"><span data-stu-id="42b00-190">Read-only.</span></span> <span data-ttu-id="42b00-191">与角色分配相关联的角色定义。</span><span class="sxs-lookup"><span data-stu-id="42b00-191">The role definition associated with the role assignment.</span></span> |
|<span data-ttu-id="42b00-192">subject</span><span class="sxs-lookup"><span data-stu-id="42b00-192">subject</span></span>|[<span data-ttu-id="42b00-193">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="42b00-193">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="42b00-194">只读。</span><span class="sxs-lookup"><span data-stu-id="42b00-194">Read-only.</span></span> <span data-ttu-id="42b00-195">主题的角色分配相关联。</span><span class="sxs-lookup"><span data-stu-id="42b00-195">The subject associated with the role assignment.</span></span> |
|<span data-ttu-id="42b00-196">linkedEligibleRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="42b00-196">linkedEligibleRoleAssignment</span></span>|[<span data-ttu-id="42b00-197">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="42b00-197">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md)|<span data-ttu-id="42b00-198">只读。</span><span class="sxs-lookup"><span data-stu-id="42b00-198">Read-only.</span></span> <span data-ttu-id="42b00-199">如果这是`active assignment`上创建由于激活和`eligible assignment`，它代表的`eligible assignment`;否则，值为`null`。</span><span class="sxs-lookup"><span data-stu-id="42b00-199">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the object of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="42b00-200">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42b00-200">JSON representation</span></span>

<span data-ttu-id="42b00-201">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42b00-201">Here is a JSON representation of the resource.</span></span>


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
  "isPermanent": true,
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
