---
title: governanceRoleAssignment 资源类型
description: 表示用户或组对角色的分配。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9c5ea36bab1edd453e0fceb51324891b45b70167
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497592"
---
# <a name="governanceroleassignment-resource-type"></a><span data-ttu-id="0f2ed-103">governanceRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f2ed-103">governanceRoleAssignment resource type</span></span>

<span data-ttu-id="0f2ed-104">命名空间： microsoft. graph[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="0f2ed-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="0f2ed-105">表示用户或组对角色的分配。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-105">Represents the assignment of a user or group to a role.</span></span>

<span data-ttu-id="0f2ed-106">特权标识管理（PIM）支持两种类型的工作分配：</span><span class="sxs-lookup"><span data-stu-id="0f2ed-106">Privileged Identity Management (PIM) supports two types of assignments:</span></span>

1. <span data-ttu-id="0f2ed-107">主动分配-表示对资源的直接/激活访问。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-107">Active assignment - Represents the direct/activated access to resources.</span></span>
2. <span data-ttu-id="0f2ed-108">符合条件的工作分配-表示对资源的特权访问的中间阶段，在无访问权限和直接访问之间。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-108">Eligible assignment - Represents an intermediate stage of privileged access to resources, between no access and direct access.</span></span> <span data-ttu-id="0f2ed-109">管理员可以提前向用户/组`eligible assignment`分配用户/组，并在需要访问时`activation` ，才能`eligible assignment`在几个小时内获得对该资源的即时访问权限。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-109">Administrators can assign users/groups to `eligible assignment` in advance, and whenever the access is needed, `activation` on the `eligible assignment` is needed to gain the instant access to the resource for several hours.</span></span> <span data-ttu-id="0f2ed-110">激活之后， `active assignment`将为用户/组成员创建，以指示激活的状态。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-110">After activation, an `active assignment` will be created for the users/group members to indicate the activated status.</span></span>

## <a name="methods"></a><span data-ttu-id="0f2ed-111">方法</span><span class="sxs-lookup"><span data-stu-id="0f2ed-111">Methods</span></span>

| <span data-ttu-id="0f2ed-112">方法</span><span class="sxs-lookup"><span data-stu-id="0f2ed-112">Method</span></span>          | <span data-ttu-id="0f2ed-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="0f2ed-113">Return Type</span></span> |<span data-ttu-id="0f2ed-114">说明</span><span class="sxs-lookup"><span data-stu-id="0f2ed-114">Description</span></span>|
|:------------|:--------|:--------|
|[<span data-ttu-id="0f2ed-115">获取</span><span class="sxs-lookup"><span data-stu-id="0f2ed-115">Get</span></span>](../api/governanceroleassignment-get.md) |  [<span data-ttu-id="0f2ed-116">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0f2ed-116">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md) |<span data-ttu-id="0f2ed-117">读取角色分配实体的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-117">Read properties and relationships of a role assignment entity.</span></span>|
|[<span data-ttu-id="0f2ed-118">List</span><span class="sxs-lookup"><span data-stu-id="0f2ed-118">List</span></span>](../api/governanceroleassignment-list.md) | <span data-ttu-id="0f2ed-119">[governanceRoleAssignment](../resources/governanceroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="0f2ed-119">[governanceRoleAssignment](../resources/governanceroleassignment.md) collection</span></span>|<span data-ttu-id="0f2ed-120">列出资源上的角色分配的集合。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-120">List a collection of role assignments on a resource.</span></span> |
|[<span data-ttu-id="0f2ed-121">Export</span><span class="sxs-lookup"><span data-stu-id="0f2ed-121">Export</span></span>](../api/governanceroleassignment-export.md) | <span data-ttu-id="0f2ed-122">八位字节流</span><span class="sxs-lookup"><span data-stu-id="0f2ed-122">octet-stream</span></span> |<span data-ttu-id="0f2ed-123">在资源上下载角色分配的集合，并将其另`.csv`存为文件。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-123">Download a collection of role assignments on a resource and save as a `.csv` file.</span></span>|

<span data-ttu-id="0f2ed-124">`roleAssignments`实体`POST`集`PUT`上`PATCH`不支持`DELETE` 、、或操作。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-124">No `POST`, `PUT`, `PATCH`, or `DELETE` operations are supported on the `roleAssignments` entity set.</span></span> <span data-ttu-id="0f2ed-125">上`governanceRoleAssignment`的任何创建、更新和删除操作均由`governanceRoleAssignmentRequest`完成。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-125">Any create, update, and delete operations on `governanceRoleAssignment` are done by `governanceRoleAssignmentRequest`.</span></span>

## <a name="properties"></a><span data-ttu-id="0f2ed-126">属性</span><span class="sxs-lookup"><span data-stu-id="0f2ed-126">Properties</span></span>
| <span data-ttu-id="0f2ed-127">属性</span><span class="sxs-lookup"><span data-stu-id="0f2ed-127">Property</span></span>  | <span data-ttu-id="0f2ed-128">类型</span><span class="sxs-lookup"><span data-stu-id="0f2ed-128">Type</span></span>      |<span data-ttu-id="0f2ed-129">说明</span><span class="sxs-lookup"><span data-stu-id="0f2ed-129">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="0f2ed-130">id</span><span class="sxs-lookup"><span data-stu-id="0f2ed-130">id</span></span>         |<span data-ttu-id="0f2ed-131">字符串</span><span class="sxs-lookup"><span data-stu-id="0f2ed-131">String</span></span>     |<span data-ttu-id="0f2ed-132">角色分配的 ID。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-132">The ID of the role assignment.</span></span> <span data-ttu-id="0f2ed-133">它采用 GUID 格式。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-133">It is in GUID format.</span></span>|
|<span data-ttu-id="0f2ed-134">resourceId</span><span class="sxs-lookup"><span data-stu-id="0f2ed-134">resourceId</span></span> |<span data-ttu-id="0f2ed-135">String</span><span class="sxs-lookup"><span data-stu-id="0f2ed-135">String</span></span>     |<span data-ttu-id="0f2ed-136">必填。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-136">Required.</span></span> <span data-ttu-id="0f2ed-137">与角色分配相关联的资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-137">The ID of the resource which the role assignment is associated with.</span></span> |
|<span data-ttu-id="0f2ed-138">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="0f2ed-138">roleDefinitionId</span></span>|<span data-ttu-id="0f2ed-139">String</span><span class="sxs-lookup"><span data-stu-id="0f2ed-139">String</span></span>|<span data-ttu-id="0f2ed-140">必填。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-140">Required.</span></span> <span data-ttu-id="0f2ed-141">与角色分配相关联的角色定义的 ID。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-141">The ID of the role definition which the role assignment is associated with.</span></span> |
|<span data-ttu-id="0f2ed-142">subjectId</span><span class="sxs-lookup"><span data-stu-id="0f2ed-142">subjectId</span></span>|<span data-ttu-id="0f2ed-143">String</span><span class="sxs-lookup"><span data-stu-id="0f2ed-143">String</span></span>       |<span data-ttu-id="0f2ed-144">必填。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-144">Required.</span></span> <span data-ttu-id="0f2ed-145">与角色分配相关联的主题的 ID。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-145">The ID of the subject which the role assignment is associated with.</span></span> |
|<span data-ttu-id="0f2ed-146">linkedEligibleRoleAssignmentId</span><span class="sxs-lookup"><span data-stu-id="0f2ed-146">linkedEligibleRoleAssignmentId</span></span>|<span data-ttu-id="0f2ed-147">String</span><span class="sxs-lookup"><span data-stu-id="0f2ed-147">String</span></span>|<span data-ttu-id="0f2ed-148">如果这是`active assignment`并因激活而创建`eligible assignment`，则表示的`eligible assignment`ID。否则，值为`null`。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-148">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the ID of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |
|<span data-ttu-id="0f2ed-149">externalId</span><span class="sxs-lookup"><span data-stu-id="0f2ed-149">externalId</span></span>   |<span data-ttu-id="0f2ed-150">String</span><span class="sxs-lookup"><span data-stu-id="0f2ed-150">String</span></span>     |<span data-ttu-id="0f2ed-151">外部 ID 用于标识提供程序中的角色分配的资源。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-151">The external ID the resource that is used to identify the role assignment in the provider.</span></span>|
|<span data-ttu-id="0f2ed-152">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0f2ed-152">startDateTime</span></span>|<span data-ttu-id="0f2ed-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f2ed-153">DateTimeOffset</span></span>|<span data-ttu-id="0f2ed-154">角色分配的开始时间。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-154">The start time of the role assignment.</span></span> <span data-ttu-id="0f2ed-155">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0f2ed-156">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0f2ed-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0f2ed-157">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0f2ed-157">endDateTime</span></span>|<span data-ttu-id="0f2ed-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f2ed-158">DateTimeOffset</span></span>|<span data-ttu-id="0f2ed-159">对于非永久角色分配，这是角色分配将在何时过期的时间。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-159">For a non-permanent role assignment, this is the time when the role assignment will be expired.</span></span> <span data-ttu-id="0f2ed-160">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-160">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0f2ed-161">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0f2ed-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0f2ed-162">assignmentState</span><span class="sxs-lookup"><span data-stu-id="0f2ed-162">assignmentState</span></span>|<span data-ttu-id="0f2ed-163">String</span><span class="sxs-lookup"><span data-stu-id="0f2ed-163">String</span></span>  |<span data-ttu-id="0f2ed-164">工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-164">The state of the assignment.</span></span> <span data-ttu-id="0f2ed-165">值可以是</span><span class="sxs-lookup"><span data-stu-id="0f2ed-165">The value can be</span></span> <ul><li> <span data-ttu-id="0f2ed-166">`Eligible`对于符合条件的工作分配</span><span class="sxs-lookup"><span data-stu-id="0f2ed-166">`Eligible` for eligible assignment</span></span></li><li> <span data-ttu-id="0f2ed-167">`Active`-如果由管理员直接分配`Active` ，或由用户在符合条件的工作分配上激活。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-167">`Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span></li></ul>|
|<span data-ttu-id="0f2ed-168">memberType</span><span class="sxs-lookup"><span data-stu-id="0f2ed-168">memberType</span></span>|<span data-ttu-id="0f2ed-169">String</span><span class="sxs-lookup"><span data-stu-id="0f2ed-169">String</span></span>      |<span data-ttu-id="0f2ed-170">成员的类型。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-170">The type of member.</span></span> <span data-ttu-id="0f2ed-171">值可以是：</span><span class="sxs-lookup"><span data-stu-id="0f2ed-171">The value can be:</span></span> <ul><li><span data-ttu-id="0f2ed-172">`Inherited`-角色分配是从父资源作用域继承的</span><span class="sxs-lookup"><span data-stu-id="0f2ed-172">`Inherited` - the role assignment is inherited from a parent resource scope</span></span></li><li><span data-ttu-id="0f2ed-173">`Group`-角色分配不是继承的，而是来自组分配的成员身份</span><span class="sxs-lookup"><span data-stu-id="0f2ed-173">`Group`- the role assignment is not inherited, but comes from the membership of a group assignment</span></span></li><li><span data-ttu-id="0f2ed-174">`User`-角色分配既不继承也不从组分配中继承。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-174">`User` - the role assignment is neither inherited nor from a group assignment.</span></span></li></ul>|


## <a name="relationships"></a><span data-ttu-id="0f2ed-175">关系</span><span class="sxs-lookup"><span data-stu-id="0f2ed-175">Relationships</span></span>
| <span data-ttu-id="0f2ed-176">关系</span><span class="sxs-lookup"><span data-stu-id="0f2ed-176">Relationship</span></span> | <span data-ttu-id="0f2ed-177">类型</span><span class="sxs-lookup"><span data-stu-id="0f2ed-177">Type</span></span>   |<span data-ttu-id="0f2ed-178">说明</span><span class="sxs-lookup"><span data-stu-id="0f2ed-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f2ed-179">资源</span><span class="sxs-lookup"><span data-stu-id="0f2ed-179">resource</span></span>|[<span data-ttu-id="0f2ed-180">governanceResource</span><span class="sxs-lookup"><span data-stu-id="0f2ed-180">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="0f2ed-181">只读。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-181">Read-only.</span></span> <span data-ttu-id="0f2ed-182">与角色分配相关联的资源。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-182">The resource associated with the role assignment.</span></span> |
|<span data-ttu-id="0f2ed-183">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="0f2ed-183">roleDefinition</span></span>|[<span data-ttu-id="0f2ed-184">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0f2ed-184">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="0f2ed-185">只读。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-185">Read-only.</span></span> <span data-ttu-id="0f2ed-186">与角色分配相关联的角色定义。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-186">The role definition associated with the role assignment.</span></span> |
|<span data-ttu-id="0f2ed-187">subject</span><span class="sxs-lookup"><span data-stu-id="0f2ed-187">subject</span></span>|[<span data-ttu-id="0f2ed-188">governanceSubject</span><span class="sxs-lookup"><span data-stu-id="0f2ed-188">governanceSubject</span></span>](../resources/governancesubject.md)|<span data-ttu-id="0f2ed-189">只读。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-189">Read-only.</span></span> <span data-ttu-id="0f2ed-190">与角色分配相关联的主题。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-190">The subject associated with the role assignment.</span></span> |
|<span data-ttu-id="0f2ed-191">linkedEligibleRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0f2ed-191">linkedEligibleRoleAssignment</span></span>|[<span data-ttu-id="0f2ed-192">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0f2ed-192">governanceRoleAssignment</span></span>](../resources/governanceroleassignment.md)|<span data-ttu-id="0f2ed-193">只读。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-193">Read-only.</span></span> <span data-ttu-id="0f2ed-194">如果这是`active assignment`并因激活而创建的`eligible assignment`，则它表示该`eligible assignment`对象的对象;否则，值为`null`。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-194">If this is an `active assignment` and created due to activation on an `eligible assignment`, it represents the object of that `eligible assignment`; Otherwise, the value is `null`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0f2ed-195">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f2ed-195">JSON representation</span></span>

<span data-ttu-id="0f2ed-196">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f2ed-196">Here is a JSON representation of the resource.</span></span>


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
