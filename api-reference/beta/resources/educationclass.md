---
title: educationClass 资源类型
description: '表示学校的课程。 **educationClass** 资源对应于 Office 365 组并共享同一个 ID。 学生是课程的正式成员，教师为所有者，且具有相应权限。 若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 2a1fb4434933a4cc41c9a84c54864f2211f40962
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334423"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="1d156-106">educationClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d156-106">educationClass resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d156-107">表示学校的课程。</span><span class="sxs-lookup"><span data-stu-id="1d156-107">Represents a class within a school.</span></span> <span data-ttu-id="1d156-108">**educationClass** 资源对应于 Office 365 组并共享同一个 ID。</span><span class="sxs-lookup"><span data-stu-id="1d156-108">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="1d156-109">学生是课程的正式成员，教师为所有者，且具有相应权限。</span><span class="sxs-lookup"><span data-stu-id="1d156-109">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="1d156-110">若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。</span><span class="sxs-lookup"><span data-stu-id="1d156-110">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="1d156-111">方法</span><span class="sxs-lookup"><span data-stu-id="1d156-111">Methods</span></span>

| <span data-ttu-id="1d156-112">方法</span><span class="sxs-lookup"><span data-stu-id="1d156-112">Method</span></span>           | <span data-ttu-id="1d156-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="1d156-113">Return Type</span></span>    |<span data-ttu-id="1d156-114">说明</span><span class="sxs-lookup"><span data-stu-id="1d156-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1d156-115">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="1d156-115">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="1d156-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="1d156-116">educationClass</span></span>](educationclass.md) |<span data-ttu-id="1d156-117">读取 **educationClass** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1d156-117">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="1d156-118">Add member</span><span class="sxs-lookup"><span data-stu-id="1d156-118">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="1d156-119">educationUser</span><span class="sxs-lookup"><span data-stu-id="1d156-119">educationUser</span></span>](educationuser.md)| <span data-ttu-id="1d156-120">通过发布到 members 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="1d156-120">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="1d156-121">List members</span><span class="sxs-lookup"><span data-stu-id="1d156-121">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="1d156-122">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1d156-122">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="1d156-123">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1d156-123">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="1d156-124">Remove student</span><span class="sxs-lookup"><span data-stu-id="1d156-124">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="1d156-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="1d156-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="1d156-126">通过成员导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="1d156-126">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="1d156-127">List schools</span><span class="sxs-lookup"><span data-stu-id="1d156-127">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="1d156-128">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1d156-128">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="1d156-129">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1d156-129">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="1d156-130">Add teacher</span><span class="sxs-lookup"><span data-stu-id="1d156-130">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="1d156-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="1d156-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="1d156-132">通过发布到 teachers 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="1d156-132">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="1d156-133">List teachers</span><span class="sxs-lookup"><span data-stu-id="1d156-133">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="1d156-134">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1d156-134">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="1d156-135">获取课程的教师列表。</span><span class="sxs-lookup"><span data-stu-id="1d156-135">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="1d156-136">Remove teacher</span><span class="sxs-lookup"><span data-stu-id="1d156-136">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="1d156-137">educationUser</span><span class="sxs-lookup"><span data-stu-id="1d156-137">educationUser</span></span>](educationuser.md)| <span data-ttu-id="1d156-138">通过教师导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="1d156-138">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="1d156-139">创建 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="1d156-139">Create educationAssignment</span></span>](../api/educationclass-post-assignments.md) |[<span data-ttu-id="1d156-140">educationAssignment</span><span class="sxs-lookup"><span data-stu-id="1d156-140">educationAssignment</span></span>](../resources/educationassignment.md)| <span data-ttu-id="1d156-141">通过发布到工作分配集合创建新的**educationAssignment** 。</span><span class="sxs-lookup"><span data-stu-id="1d156-141">Create a new **educationAssignment** by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="1d156-142">列出作业</span><span class="sxs-lookup"><span data-stu-id="1d156-142">List assignments</span></span>](../api/educationclass-list-assignments.md) |<span data-ttu-id="1d156-143">[educationAssignment](../resources/educationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="1d156-143">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="1d156-144">获取**educationAssignment**对象集合。</span><span class="sxs-lookup"><span data-stu-id="1d156-144">Get an **educationAssignment** object collection.</span></span>|
|[<span data-ttu-id="1d156-145">Get group</span><span class="sxs-lookup"><span data-stu-id="1d156-145">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="1d156-146">组</span><span class="sxs-lookup"><span data-stu-id="1d156-146">group</span></span>](group.md)| <span data-ttu-id="1d156-147">获得与此 **educationClass** 对应的 Office 365 **group**。</span><span class="sxs-lookup"><span data-stu-id="1d156-147">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="1d156-148">创建 educationCategory</span><span class="sxs-lookup"><span data-stu-id="1d156-148">Create educationCategory</span></span>](../api/educationclass-post-category.md) | [<span data-ttu-id="1d156-149">educationCategory</span><span class="sxs-lookup"><span data-stu-id="1d156-149">educationCategory</span></span>](educationCategory.md) | <span data-ttu-id="1d156-150">为此类创建新的**educationCategory** 。</span><span class="sxs-lookup"><span data-stu-id="1d156-150">Create a new **educationCategory** for this class.</span></span>|
|[<span data-ttu-id="1d156-151">List categories</span><span class="sxs-lookup"><span data-stu-id="1d156-151">List categories</span></span>](../api/educationclass-list-categories.md) | <span data-ttu-id="1d156-152">[educationCategory](educationCategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="1d156-152">[educationCategory](educationCategory.md) collection</span></span> | <span data-ttu-id="1d156-153">获取属于此类的**educationCategory**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="1d156-153">Get a list of **educationCategory** objects belonging to this class.</span></span>|
|[<span data-ttu-id="1d156-154">Update</span><span class="sxs-lookup"><span data-stu-id="1d156-154">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="1d156-155">educationClass</span><span class="sxs-lookup"><span data-stu-id="1d156-155">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="1d156-156">更新 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="1d156-156">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="1d156-157">删除</span><span class="sxs-lookup"><span data-stu-id="1d156-157">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="1d156-158">无</span><span class="sxs-lookup"><span data-stu-id="1d156-158">None</span></span> |<span data-ttu-id="1d156-159">删除 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="1d156-159">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1d156-160">属性</span><span class="sxs-lookup"><span data-stu-id="1d156-160">Properties</span></span>
| <span data-ttu-id="1d156-161">属性</span><span class="sxs-lookup"><span data-stu-id="1d156-161">Property</span></span>     | <span data-ttu-id="1d156-162">类型</span><span class="sxs-lookup"><span data-stu-id="1d156-162">Type</span></span>   |<span data-ttu-id="1d156-163">说明</span><span class="sxs-lookup"><span data-stu-id="1d156-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d156-164">id</span><span class="sxs-lookup"><span data-stu-id="1d156-164">id</span></span>| <span data-ttu-id="1d156-165">字符串</span><span class="sxs-lookup"><span data-stu-id="1d156-165">String</span></span>| <span data-ttu-id="1d156-166">课程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1d156-166">Unique identifier for the class.</span></span>|
|<span data-ttu-id="1d156-167">说明</span><span class="sxs-lookup"><span data-stu-id="1d156-167">description</span></span>|<span data-ttu-id="1d156-168">String</span><span class="sxs-lookup"><span data-stu-id="1d156-168">String</span></span>| <span data-ttu-id="1d156-169">课程说明。</span><span class="sxs-lookup"><span data-stu-id="1d156-169">Description of the class.</span></span>|
|<span data-ttu-id="1d156-170">displayName</span><span class="sxs-lookup"><span data-stu-id="1d156-170">displayName</span></span>|<span data-ttu-id="1d156-171">String</span><span class="sxs-lookup"><span data-stu-id="1d156-171">String</span></span>| <span data-ttu-id="1d156-172">课程名称。</span><span class="sxs-lookup"><span data-stu-id="1d156-172">Name of the class.</span></span>|
|<span data-ttu-id="1d156-173">mailNickname</span><span class="sxs-lookup"><span data-stu-id="1d156-173">mailNickname</span></span>|<span data-ttu-id="1d156-174">字符串</span><span class="sxs-lookup"><span data-stu-id="1d156-174">String</span></span>| <span data-ttu-id="1d156-175">向所有成员发送电子邮件的邮件名称（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="1d156-175">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="1d156-176">createdBy</span><span class="sxs-lookup"><span data-stu-id="1d156-176">createdBy</span></span>|[<span data-ttu-id="1d156-177">identitySet</span><span class="sxs-lookup"><span data-stu-id="1d156-177">identitySet</span></span>](identityset.md)| <span data-ttu-id="1d156-178">创建了课程的实体</span><span class="sxs-lookup"><span data-stu-id="1d156-178">Entity who created the class</span></span> |
|<span data-ttu-id="1d156-179">classCode</span><span class="sxs-lookup"><span data-stu-id="1d156-179">classCode</span></span>|<span data-ttu-id="1d156-180">String</span><span class="sxs-lookup"><span data-stu-id="1d156-180">String</span></span>| <span data-ttu-id="1d156-181">学校用于标识课程的课程代码。</span><span class="sxs-lookup"><span data-stu-id="1d156-181">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="1d156-182">externalId</span><span class="sxs-lookup"><span data-stu-id="1d156-182">externalId</span></span>|<span data-ttu-id="1d156-183">String</span><span class="sxs-lookup"><span data-stu-id="1d156-183">String</span></span>| <span data-ttu-id="1d156-184">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="1d156-184">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="1d156-185">externalName</span><span class="sxs-lookup"><span data-stu-id="1d156-185">externalName</span></span>|<span data-ttu-id="1d156-186">String</span><span class="sxs-lookup"><span data-stu-id="1d156-186">String</span></span>|<span data-ttu-id="1d156-187">同步系统中的课程名称。</span><span class="sxs-lookup"><span data-stu-id="1d156-187">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="1d156-188">externalSource</span><span class="sxs-lookup"><span data-stu-id="1d156-188">externalSource</span></span>|<span data-ttu-id="1d156-189">string</span><span class="sxs-lookup"><span data-stu-id="1d156-189">string</span></span>| <span data-ttu-id="1d156-190">此课程的创建方式。</span><span class="sxs-lookup"><span data-stu-id="1d156-190">How this class was created.</span></span> <span data-ttu-id="1d156-191">可取值为：`sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="1d156-191">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1d156-192">term</span><span class="sxs-lookup"><span data-stu-id="1d156-192">term</span></span>|[<span data-ttu-id="1d156-193">educationTerm</span><span class="sxs-lookup"><span data-stu-id="1d156-193">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="1d156-194">此课程的学期。</span><span class="sxs-lookup"><span data-stu-id="1d156-194">Term for this class.</span></span>|


## <a name="relationships"></a><span data-ttu-id="1d156-195">关系</span><span class="sxs-lookup"><span data-stu-id="1d156-195">Relationships</span></span>
| <span data-ttu-id="1d156-196">关系</span><span class="sxs-lookup"><span data-stu-id="1d156-196">Relationship</span></span> | <span data-ttu-id="1d156-197">类型</span><span class="sxs-lookup"><span data-stu-id="1d156-197">Type</span></span>   |<span data-ttu-id="1d156-198">说明</span><span class="sxs-lookup"><span data-stu-id="1d156-198">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d156-199">members</span><span class="sxs-lookup"><span data-stu-id="1d156-199">members</span></span>|<span data-ttu-id="1d156-200">[educationUser](../resources/educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1d156-200">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="1d156-201">课程中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="1d156-201">All users in the class.</span></span> <span data-ttu-id="1d156-202">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="1d156-202">Nullable.</span></span>|
|<span data-ttu-id="1d156-203">schools</span><span class="sxs-lookup"><span data-stu-id="1d156-203">schools</span></span>|<span data-ttu-id="1d156-204">[educationSchool](../resources/educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1d156-204">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="1d156-205">与此课程相关的所有学校。</span><span class="sxs-lookup"><span data-stu-id="1d156-205">All schools that this class is associated with.</span></span> <span data-ttu-id="1d156-206">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="1d156-206">Nullable.</span></span>|
|<span data-ttu-id="1d156-207">teachers</span><span class="sxs-lookup"><span data-stu-id="1d156-207">teachers</span></span>|<span data-ttu-id="1d156-208">[educationUser](../resources/educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1d156-208">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="1d156-209">课程中的所有教师。</span><span class="sxs-lookup"><span data-stu-id="1d156-209">All teachers in the class.</span></span> <span data-ttu-id="1d156-210">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="1d156-210">Nullable.</span></span>|
|<span data-ttu-id="1d156-211">assignments</span><span class="sxs-lookup"><span data-stu-id="1d156-211">assignments</span></span>|<span data-ttu-id="1d156-212">[educationAssignment](../resources/educationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="1d156-212">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="1d156-213">与此类关联的所有工作分配。</span><span class="sxs-lookup"><span data-stu-id="1d156-213">All assignments associated with this class.</span></span> <span data-ttu-id="1d156-214">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="1d156-214">Nullable.</span></span>|
|<span data-ttu-id="1d156-215">类别</span><span class="sxs-lookup"><span data-stu-id="1d156-215">categories</span></span>|<span data-ttu-id="1d156-216">[educationCategory](../resources/educationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="1d156-216">[educationCategory](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="1d156-217">与此类关联的所有类别。</span><span class="sxs-lookup"><span data-stu-id="1d156-217">All categories associated with this class.</span></span> <span data-ttu-id="1d156-218">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="1d156-218">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d156-219">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d156-219">JSON representation</span></span>

<span data-ttu-id="1d156-220">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d156-220">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "id": "String",
  "description": "String",
  "classCode": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "mailNickname": "String",
  "term": {"@odata.type": "microsoft.graph.educationTerm"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
