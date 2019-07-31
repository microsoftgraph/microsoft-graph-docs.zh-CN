---
title: governanceRoleAssignment 资源类型
description: 表示用户或组对角色的分配。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 518fbe18fcd09b1b4cc9730c6b7f0112adabfeae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971884"
---
# <a name="governanceroleassignment-resource-type"></a><span data-ttu-id="46fff-103">governanceRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="46fff-103">governanceRoleAssignment resource type</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46fff-104">表示用户或组对角色的分配。</span><span class="sxs-lookup"><span data-stu-id="46fff-104">Represents the assignment of a user or group to a role.</span></span>

<span data-ttu-id="46fff-105">特权标识管理 (PIM) 支持两种类型的工作分配:</span><span class="sxs-lookup"><span data-stu-id="46fff-105">Privileged Identity Management (PIM) supports two types of assignments:</span></span>

1. <span data-ttu-id="46fff-106">主动分配-表示对资源的直接/激活访问。</span><span class="sxs-lookup"><span data-stu-id="46fff-106">Active assignment - Represents the direct/activated access to resources.</span></span>
2. <span data-ttu-id="46fff-107">符合条件的工作分配-表示对资源的特权访问的中间阶段, 在无访问权限和直接访问之间。</span><span class="sxs-lookup"><span data-stu-id="46fff-107">Eligible assignment - Represents an intermediate stage of privileged access to resources, between no access and direct access.</span></span> <span data-ttu-id="46fff-108">管理员可以提前向用户/组`eligible assignment`分配用户/组, 并在需要访问时`activation` , 才能`eligible assignment`在几个小时内获得对该资源的即时访问权限。</span><span class="sxs-lookup"><span data-stu-id="46fff-108">Administrators can assign users/groups to `eligible assignment` in advance, and whenever the access is needed, `activation` on the `eligible assignment` is needed to gain the instant access to the resource for several hours.</span></span> <span data-ttu-id="46fff-109">激活之后, `active assignment`将为用户/组成员创建, 以指示激活的状态。</span><span class="sxs-lookup"><span data-stu-id="46fff-109">After activation, an `active assignment` will be created for the users/group members to indicate the activated status.</span></span>

## <a name="methods"></a><span data-ttu-id="46fff-110">方法</span><span class="sxs-lookup"><span data-stu-id="46fff-110">Methods</span></span>

| <span data-ttu-id="46fff-111">方法</span><span class="sxs-lookup"><span data-stu-id="46fff-111">Method</span></span>          | <span data-ttu-id="46fff-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="46fff-112">Return Type</span></span> |<span data-ttu-id="46fff-113">说明</span><span class="sxs-lookup"><span data-stu-id="46fff-113">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="46fff-114">Get</span><span class="sxs-lookup"><span data-stu-id="46fff-114">Get</span></span>](../api/governanceroleassignment-get.md) |  [<span data-ttu-id="46fff-115">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="46fff-115">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md) |<span data-ttu-id="46fff-116">读取角色分配实体的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="46fff-116">Read properties and relationships of a role assignment entity.</span></span>|
|[<span data-ttu-id="46fff-117">List</span><span class="sxs-lookup"><span data-stu-id="46fff-117">List</span></span>](../api/governanceroleassignment-list.md) | <span data-ttu-id="46fff-118">[governanceRoleAssignment](../resources/governanceroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="46fff-118">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="46fff-119">列出资源上的角色分配的集合。</span><span class="sxs-lookup"><span data-stu-id="46fff-119">List a collection of role assignments on a resource.</span></span> |
|[<span data-ttu-id="46fff-120">Export</span><span class="sxs-lookup"><span data-stu-id="46fff-120">Export</span></span>](../api/governanceroleassignment-export.md) | <span data-ttu-id="46fff-121">八位字节流</span><span class="sxs-lookup"><span data-stu-id="46fff-121">octet-stream</span></span> |<span data-ttu-id="46fff-122">在资源上下载角色分配的集合, 并将其另`.csv`存为文件。</span><span class="sxs-lookup"><span data-stu-id="46fff-122">Download a collection of role assignments on a resource and save as a `.csv` file.</span></span>|

<span data-ttu-id="46fff-123">`roleAssignments`实体`POST`集`PUT`上`PATCH`不支持`DELETE` 、、或操作。</span><span class="sxs-lookup"><span data-stu-id="46fff-123">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `roleAssignments` entity set.</span></span> <span data-ttu-id="46fff-124">上`governanceRoleAssignment`的任何创建、更新和删除操作均由`governanceRoleAssignmentRequest`完成。</span><span class="sxs-lookup"><span data-stu-id="46fff-124">Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.</span></span>

## <a name="properties"></a><span data-ttu-id="46fff-125">属性</span><span class="sxs-lookup"><span data-stu-id="46fff-125">Properties</span></span>
| <span data-ttu-id="46fff-126">属性</span><span class="sxs-lookup"><span data-stu-id="46fff-126">Property</span></span>  | <span data-ttu-id="46fff-127">类型</span><span class="sxs-lookup"><span data-stu-id="46fff-127">Type</span></span>      |<span data-ttu-id="46fff-128">说明</span><span class="sxs-lookup"><span data-stu-id="46fff-128">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="46fff-129">id</span><span class="sxs-lookup"><span data-stu-id="46fff-129">id</span></span>         |<span data-ttu-id="46fff-130">字符串</span><span class="sxs-lookup"><span data-stu-id="46fff-130">String</span></span>     |<span data-ttu-id="46fff-131">角色分配的 ID。</span><span class="sxs-lookup"><span data-stu-id="46fff-131">The ID of the role assignment.</span></span> <span data-ttu-id="46fff-132">它采用 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="46fff-132">It is in GUID format.</span></span>|
|<span data-ttu-id="46fff-133">resourceId</span><span class="sxs-lookup"><span data-stu-id="46fff-133">resourceId</span></span> |<span data-ttu-id="46fff-134">String</span><span class="sxs-lookup"><span data-stu-id="46fff-134">String</span></span>     |<span data-ttu-id="46fff-135">必需。</span><span class="sxs-lookup"><span data-stu-id="46fff-135">Required.</span></span> <span data-ttu-id="46fff-136">与角色分配相关联的资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="46fff-136">The ID of the resource which the role assignment is associated with.</span></span> |
|<span data-ttu-id="46fff-137">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="46fff-137">roleDefinitionId</span></span>|<span data-ttu-id="46fff-138">String</span><span class="sxs-lookup"><span data-stu-id="46fff-138">String</span></span>|<span data-ttu-id="46fff-139">必需。</span><span class="sxs-lookup"><span data-stu-id="46fff-139">Required.</span></span> <span data-ttu-id="46fff-140">与角色分配相关联的角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="46fff-140">The ID of the role definition which the role assignment is associated with.</span></span> |
|<span data-ttu-id="46fff-141">subjectId</span><span class="sxs-lookup"><span data-stu-id="46fff-141">subjectId</span></span>|<span data-ttu-id="46fff-142">String</span><span class="sxs-lookup"><span data-stu-id="46fff-142">String</span></span>       |<span data-ttu-id="46fff-143">必需。</span><span class="sxs-lookup"><span data-stu-id="46fff-143">Required.</span></span> <span data-ttu-id="46fff-144">与角色分配相关联的主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="46fff-144">The ID of the subject which the role assignment is associated with.</span></span> |
|<span data-ttu-id="46fff-145">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="46fff-145">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="46fff-146">String</span><span class="sxs-lookup"><span data-stu-id="46fff-146">String</span></span>|<span data-ttu-id="46fff-147">如果这是`active assignment`并因激活而创建`eligible assignment`, 则表示的`eligible assignment`ID。否则, 值为`null`。</span><span class="sxs-lookup"><span data-stu-id="46fff-147">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the ID of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |
|<span data-ttu-id="46fff-148">externalId</span><span class="sxs-lookup"><span data-stu-id="46fff-148">externalId</span></span>   |<span data-ttu-id="46fff-149">String</span><span class="sxs-lookup"><span data-stu-id="46fff-149">String</span></span>     |<span data-ttu-id="46fff-150">外部 ID 用于标识提供程序中的角色分配的资源。</span><span class="sxs-lookup"><span data-stu-id="46fff-150">The external ID the resource that is used to identify the role assignment in the provider.</span></span>|
|<span data-ttu-id="46fff-151">startDateTime</span><span class="sxs-lookup"><span data-stu-id="46fff-151">startDateTime</span></span>|<span data-ttu-id="46fff-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46fff-152">DateTimeOffset</span></span>|<span data-ttu-id="46fff-153">角色分配的开始时间。</span><span class="sxs-lookup"><span data-stu-id="46fff-153">The start time of the role assignment.</span></span> <span data-ttu-id="46fff-154">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="46fff-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="46fff-155">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="46fff-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="46fff-156">endDateTime</span><span class="sxs-lookup"><span data-stu-id="46fff-156">endDateTime</span></span>|<span data-ttu-id="46fff-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46fff-157">DateTimeOffset</span></span>|<span data-ttu-id="46fff-158">对于非永久角色分配, 这是角色分配将在何时过期的时间。</span><span class="sxs-lookup"><span data-stu-id="46fff-158">For a non-permanent role assignment, this is the time when the role assignment will be expired.</span></span> <span data-ttu-id="46fff-159">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="46fff-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="46fff-160">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="46fff-160">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="46fff-161">assignmentState</span><span class="sxs-lookup"><span data-stu-id="46fff-161">assignmentState</span></span>|<span data-ttu-id="46fff-162">String</span><span class="sxs-lookup"><span data-stu-id="46fff-162">String</span></span>  |<span data-ttu-id="46fff-163">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="46fff-163">The state of the assignment.</span></span> <span data-ttu-id="46fff-164">值可以是</span><span class="sxs-lookup"><span data-stu-id="46fff-164">The value can be</span></span> <ul><li> <span data-ttu-id="46fff-165">`Eligible`对于符合条件的工作分配</span><span class="sxs-lookup"><span data-stu-id="46fff-165">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="46fff-166">`Active`-如果由管理员直接分配`Active` , 或由用户在符合条件的工作分配上激活。</span><span class="sxs-lookup"><span data-stu-id="46fff-166">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="46fff-167">memberType</span><span class="sxs-lookup"><span data-stu-id="46fff-167">memberType</span></span>|<span data-ttu-id="46fff-168">String</span><span class="sxs-lookup"><span data-stu-id="46fff-168">String</span></span>      |<span data-ttu-id="46fff-169">成员的类型。</span><span class="sxs-lookup"><span data-stu-id="46fff-169">The type of member.</span></span> <span data-ttu-id="46fff-170">值可以是:</span><span class="sxs-lookup"><span data-stu-id="46fff-170">The value can be:</span></span> <ul><li><span data-ttu-id="46fff-171">`Inherited`-角色分配是从父资源作用域继承的</span><span class="sxs-lookup"><span data-stu-id="46fff-171">`Inherited` - the role assignment is inherited from a parent resource scope</span></span></li><li><span data-ttu-id="46fff-172">`Group`-角色分配不是继承的, 而是来自组分配的成员身份</span><span class="sxs-lookup"><span data-stu-id="46fff-172">`Group`- the role assignment is not inherited, but comes from the membership of a group assignment</span></span></li><li><span data-ttu-id="46fff-173">`User`-角色分配既不继承也不从组分配中继承。</span><span class="sxs-lookup"><span data-stu-id="46fff-173">`User` - the role assignment is neither inherited nor from a group assignment.</span></span></li></ul>|


## <a name="relationships"></a><span data-ttu-id="46fff-174">关系</span><span class="sxs-lookup"><span data-stu-id="46fff-174">Relationships</span></span>
| <span data-ttu-id="46fff-175">关系</span><span class="sxs-lookup"><span data-stu-id="46fff-175">Relationship</span></span> | <span data-ttu-id="46fff-176">类型</span><span class="sxs-lookup"><span data-stu-id="46fff-176">Type</span></span>   |<span data-ttu-id="46fff-177">说明</span><span class="sxs-lookup"><span data-stu-id="46fff-177">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46fff-178">资源</span><span class="sxs-lookup"><span data-stu-id="46fff-178">resource</span></span>|[<span data-ttu-id="46fff-179">governanceResource</span><span class="sxs-lookup"><span data-stu-id="46fff-179">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="46fff-180">只读。</span><span class="sxs-lookup"><span data-stu-id="46fff-180">Read-only.</span></span> <span data-ttu-id="46fff-181">与角色分配相关联的资源。</span><span class="sxs-lookup"><span data-stu-id="46fff-181">The resource associated with the role assignment.</span></span> |
|<span data-ttu-id="46fff-182">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="46fff-182">roleDefinition</span></span>|[<span data-ttu-id="46fff-183">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="46fff-183">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="46fff-184">只读。</span><span class="sxs-lookup"><span data-stu-id="46fff-184">Read-only.</span></span> <span data-ttu-id="46fff-185">与角色分配相关联的角色定义。</span><span class="sxs-lookup"><span data-stu-id="46fff-185">The role definition associated with the role assignment.</span></span> |
|<span data-ttu-id="46fff-186">subject</span><span class="sxs-lookup"><span data-stu-id="46fff-186">subject</span></span>|[<span data-ttu-id="46fff-187">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="46fff-187">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="46fff-188">只读。</span><span class="sxs-lookup"><span data-stu-id="46fff-188">Read-only.</span></span> <span data-ttu-id="46fff-189">与角色分配相关联的主题。</span><span class="sxs-lookup"><span data-stu-id="46fff-189">The subject associated with the role assignment.</span></span> |
|<span data-ttu-id="46fff-190">linkedEligibleRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="46fff-190">linkedEligibleRoleAssignment</span></span>|[<span data-ttu-id="46fff-191">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="46fff-191">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md)|<span data-ttu-id="46fff-192">只读。</span><span class="sxs-lookup"><span data-stu-id="46fff-192">Read-only.</span></span> <span data-ttu-id="46fff-193">如果这是`active assignment`并因激活而创建的`eligible assignment`, 则它表示该`eligible assignment`对象的对象;否则, 值为`null`。</span><span class="sxs-lookup"><span data-stu-id="46fff-193">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the object of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="46fff-194">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="46fff-194">JSON representation</span></span>

<span data-ttu-id="46fff-195">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="46fff-195">Here is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
  "suppressions": []
}
-->
