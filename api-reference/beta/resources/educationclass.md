---
title: educationClass 资源类型
description: '表示学校的课程。 **educationClass** 资源对应于 Office 365 组并共享同一个 ID。 学生是课程的正式成员，教师为所有者，且具有相应权限。 若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: dfce83c99ec886a01c2c52c3bae58c91b12fa0b0
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536167"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="53bde-106">educationClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="53bde-106">educationClass resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53bde-107">表示学校的课程。</span><span class="sxs-lookup"><span data-stu-id="53bde-107">Represents a class within a school.</span></span> <span data-ttu-id="53bde-108">**educationClass** 资源对应于 Office 365 组并共享同一个 ID。</span><span class="sxs-lookup"><span data-stu-id="53bde-108">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="53bde-109">学生是课程的正式成员，教师为所有者，且具有相应权限。</span><span class="sxs-lookup"><span data-stu-id="53bde-109">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="53bde-110">若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。</span><span class="sxs-lookup"><span data-stu-id="53bde-110">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="53bde-111">方法</span><span class="sxs-lookup"><span data-stu-id="53bde-111">Methods</span></span>

| <span data-ttu-id="53bde-112">方法</span><span class="sxs-lookup"><span data-stu-id="53bde-112">Method</span></span>           | <span data-ttu-id="53bde-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="53bde-113">Return Type</span></span>    |<span data-ttu-id="53bde-114">说明</span><span class="sxs-lookup"><span data-stu-id="53bde-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="53bde-115">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="53bde-115">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="53bde-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="53bde-116">educationClass</span></span>](educationclass.md) |<span data-ttu-id="53bde-117">读取 **educationClass** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="53bde-117">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="53bde-118">Add member</span><span class="sxs-lookup"><span data-stu-id="53bde-118">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="53bde-119">educationUser</span><span class="sxs-lookup"><span data-stu-id="53bde-119">educationUser</span></span>](educationuser.md)| <span data-ttu-id="53bde-120">通过发布到 members 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="53bde-120">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="53bde-121">List members</span><span class="sxs-lookup"><span data-stu-id="53bde-121">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="53bde-122">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="53bde-122">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="53bde-123">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="53bde-123">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="53bde-124">Remove student</span><span class="sxs-lookup"><span data-stu-id="53bde-124">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="53bde-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="53bde-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="53bde-126">通过成员导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="53bde-126">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="53bde-127">List schools</span><span class="sxs-lookup"><span data-stu-id="53bde-127">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="53bde-128">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="53bde-128">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="53bde-129">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="53bde-129">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="53bde-130">Add teacher</span><span class="sxs-lookup"><span data-stu-id="53bde-130">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="53bde-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="53bde-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="53bde-132">通过发布到 teachers 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="53bde-132">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="53bde-133">List teachers</span><span class="sxs-lookup"><span data-stu-id="53bde-133">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="53bde-134">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="53bde-134">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="53bde-135">获取课程的教师列表。</span><span class="sxs-lookup"><span data-stu-id="53bde-135">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="53bde-136">Remove teacher</span><span class="sxs-lookup"><span data-stu-id="53bde-136">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="53bde-137">educationUser</span><span class="sxs-lookup"><span data-stu-id="53bde-137">educationUser</span></span>](educationuser.md)| <span data-ttu-id="53bde-138">通过教师导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="53bde-138">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="53bde-139">创建 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="53bde-139">Create educationAssignment</span></span>](../api/educationclass-post-assignments.md) |[<span data-ttu-id="53bde-140">educationAssignment</span><span class="sxs-lookup"><span data-stu-id="53bde-140">educationAssignment</span></span>](../resources/educationassignment.md)| <span data-ttu-id="53bde-141">通过发布到工作分配集合创建新的**educationAssignment** 。</span><span class="sxs-lookup"><span data-stu-id="53bde-141">Create a new **educationAssignment** by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="53bde-142">列出作业</span><span class="sxs-lookup"><span data-stu-id="53bde-142">List assignments</span></span>](../api/educationclass-list-assignments.md) |<span data-ttu-id="53bde-143">[educationAssignment](../resources/educationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="53bde-143">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="53bde-144">获取**educationAssignment**对象集合。</span><span class="sxs-lookup"><span data-stu-id="53bde-144">Get an **educationAssignment** object collection.</span></span>|
|[<span data-ttu-id="53bde-145">Get group</span><span class="sxs-lookup"><span data-stu-id="53bde-145">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="53bde-146">组</span><span class="sxs-lookup"><span data-stu-id="53bde-146">group</span></span>](group.md)| <span data-ttu-id="53bde-147">获得与此 **educationClass** 对应的 Office 365 **group**。</span><span class="sxs-lookup"><span data-stu-id="53bde-147">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="53bde-148">创建 educationCategory</span><span class="sxs-lookup"><span data-stu-id="53bde-148">Create educationCategory</span></span>](../api/educationclass-post-category.md) | [<span data-ttu-id="53bde-149">educationCategory</span><span class="sxs-lookup"><span data-stu-id="53bde-149">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="53bde-150">为此类创建新的**educationCategory** 。</span><span class="sxs-lookup"><span data-stu-id="53bde-150">Create a new **educationCategory** for this class.</span></span>|
|[<span data-ttu-id="53bde-151">List categories</span><span class="sxs-lookup"><span data-stu-id="53bde-151">List categories</span></span>](../api/educationclass-list-categories.md) | <span data-ttu-id="53bde-152">[educationCategory](educationcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="53bde-152">[educationCategory](educationcategory.md) collection</span></span> | <span data-ttu-id="53bde-153">获取属于此类的**educationCategory**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="53bde-153">Get a list of **educationCategory** objects belonging to this class.</span></span>|
|[<span data-ttu-id="53bde-154">Update</span><span class="sxs-lookup"><span data-stu-id="53bde-154">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="53bde-155">educationClass</span><span class="sxs-lookup"><span data-stu-id="53bde-155">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="53bde-156">更新 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="53bde-156">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="53bde-157">删除</span><span class="sxs-lookup"><span data-stu-id="53bde-157">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="53bde-158">无</span><span class="sxs-lookup"><span data-stu-id="53bde-158">None</span></span> |<span data-ttu-id="53bde-159">删除 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="53bde-159">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="53bde-160">属性</span><span class="sxs-lookup"><span data-stu-id="53bde-160">Properties</span></span>
| <span data-ttu-id="53bde-161">属性</span><span class="sxs-lookup"><span data-stu-id="53bde-161">Property</span></span>     | <span data-ttu-id="53bde-162">类型</span><span class="sxs-lookup"><span data-stu-id="53bde-162">Type</span></span>   |<span data-ttu-id="53bde-163">说明</span><span class="sxs-lookup"><span data-stu-id="53bde-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53bde-164">id</span><span class="sxs-lookup"><span data-stu-id="53bde-164">id</span></span>| <span data-ttu-id="53bde-165">字符串</span><span class="sxs-lookup"><span data-stu-id="53bde-165">String</span></span>| <span data-ttu-id="53bde-166">课程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="53bde-166">Unique identifier for the class.</span></span>|
|<span data-ttu-id="53bde-167">说明</span><span class="sxs-lookup"><span data-stu-id="53bde-167">description</span></span>|<span data-ttu-id="53bde-168">String</span><span class="sxs-lookup"><span data-stu-id="53bde-168">String</span></span>| <span data-ttu-id="53bde-169">课程说明。</span><span class="sxs-lookup"><span data-stu-id="53bde-169">Description of the class.</span></span>|
|<span data-ttu-id="53bde-170">displayName</span><span class="sxs-lookup"><span data-stu-id="53bde-170">displayName</span></span>|<span data-ttu-id="53bde-171">String</span><span class="sxs-lookup"><span data-stu-id="53bde-171">String</span></span>| <span data-ttu-id="53bde-172">课程名称。</span><span class="sxs-lookup"><span data-stu-id="53bde-172">Name of the class.</span></span>|
|<span data-ttu-id="53bde-173">mailNickname</span><span class="sxs-lookup"><span data-stu-id="53bde-173">mailNickname</span></span>|<span data-ttu-id="53bde-174">字符串</span><span class="sxs-lookup"><span data-stu-id="53bde-174">String</span></span>| <span data-ttu-id="53bde-175">向所有成员发送电子邮件的邮件名称（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="53bde-175">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="53bde-176">createdBy</span><span class="sxs-lookup"><span data-stu-id="53bde-176">createdBy</span></span>|[<span data-ttu-id="53bde-177">identitySet</span><span class="sxs-lookup"><span data-stu-id="53bde-177">identitySet</span></span>](identityset.md)| <span data-ttu-id="53bde-178">创建了课程的实体</span><span class="sxs-lookup"><span data-stu-id="53bde-178">Entity who created the class</span></span> |
|<span data-ttu-id="53bde-179">classCode</span><span class="sxs-lookup"><span data-stu-id="53bde-179">classCode</span></span>|<span data-ttu-id="53bde-180">String</span><span class="sxs-lookup"><span data-stu-id="53bde-180">String</span></span>| <span data-ttu-id="53bde-181">学校用于标识课程的课程代码。</span><span class="sxs-lookup"><span data-stu-id="53bde-181">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="53bde-182">externalId</span><span class="sxs-lookup"><span data-stu-id="53bde-182">externalId</span></span>|<span data-ttu-id="53bde-183">String</span><span class="sxs-lookup"><span data-stu-id="53bde-183">String</span></span>| <span data-ttu-id="53bde-184">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="53bde-184">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="53bde-185">externalName</span><span class="sxs-lookup"><span data-stu-id="53bde-185">externalName</span></span>|<span data-ttu-id="53bde-186">String</span><span class="sxs-lookup"><span data-stu-id="53bde-186">String</span></span>|<span data-ttu-id="53bde-187">同步系统中的课程名称。</span><span class="sxs-lookup"><span data-stu-id="53bde-187">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="53bde-188">externalSource</span><span class="sxs-lookup"><span data-stu-id="53bde-188">externalSource</span></span>|<span data-ttu-id="53bde-189">string</span><span class="sxs-lookup"><span data-stu-id="53bde-189">string</span></span>| <span data-ttu-id="53bde-190">此课程的创建方式。</span><span class="sxs-lookup"><span data-stu-id="53bde-190">How this class was created.</span></span> <span data-ttu-id="53bde-191">可取值为：`sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="53bde-191">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="53bde-192">term</span><span class="sxs-lookup"><span data-stu-id="53bde-192">term</span></span>|[<span data-ttu-id="53bde-193">educationTerm</span><span class="sxs-lookup"><span data-stu-id="53bde-193">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="53bde-194">此课程的学期。</span><span class="sxs-lookup"><span data-stu-id="53bde-194">Term for this class.</span></span>|


## <a name="relationships"></a><span data-ttu-id="53bde-195">关系</span><span class="sxs-lookup"><span data-stu-id="53bde-195">Relationships</span></span>
| <span data-ttu-id="53bde-196">关系</span><span class="sxs-lookup"><span data-stu-id="53bde-196">Relationship</span></span> | <span data-ttu-id="53bde-197">类型</span><span class="sxs-lookup"><span data-stu-id="53bde-197">Type</span></span>   |<span data-ttu-id="53bde-198">说明</span><span class="sxs-lookup"><span data-stu-id="53bde-198">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53bde-199">成员</span><span class="sxs-lookup"><span data-stu-id="53bde-199">members</span></span>|<span data-ttu-id="53bde-200">[educationUser](../resources/educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="53bde-200">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="53bde-201">课程中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="53bde-201">All users in the class.</span></span> <span data-ttu-id="53bde-202">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="53bde-202">Nullable.</span></span>|
|<span data-ttu-id="53bde-203">schools</span><span class="sxs-lookup"><span data-stu-id="53bde-203">schools</span></span>|<span data-ttu-id="53bde-204">[educationSchool](../resources/educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="53bde-204">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="53bde-205">与此课程相关的所有学校。</span><span class="sxs-lookup"><span data-stu-id="53bde-205">All schools that this class is associated with.</span></span> <span data-ttu-id="53bde-206">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="53bde-206">Nullable.</span></span>|
|<span data-ttu-id="53bde-207">teachers</span><span class="sxs-lookup"><span data-stu-id="53bde-207">teachers</span></span>|<span data-ttu-id="53bde-208">[educationUser](../resources/educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="53bde-208">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="53bde-209">课程中的所有教师。</span><span class="sxs-lookup"><span data-stu-id="53bde-209">All teachers in the class.</span></span> <span data-ttu-id="53bde-210">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="53bde-210">Nullable.</span></span>|
|<span data-ttu-id="53bde-211">assignments</span><span class="sxs-lookup"><span data-stu-id="53bde-211">assignments</span></span>|<span data-ttu-id="53bde-212">[educationAssignment](../resources/educationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="53bde-212">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="53bde-213">与此类关联的所有工作分配。</span><span class="sxs-lookup"><span data-stu-id="53bde-213">All assignments associated with this class.</span></span> <span data-ttu-id="53bde-214">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="53bde-214">Nullable.</span></span>|
|<span data-ttu-id="53bde-215">categories</span><span class="sxs-lookup"><span data-stu-id="53bde-215">categories</span></span>|<span data-ttu-id="53bde-216">[educationCategory](../resources/educationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="53bde-216">[educationCategory](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="53bde-217">与此类关联的所有类别。</span><span class="sxs-lookup"><span data-stu-id="53bde-217">All categories associated with this class.</span></span> <span data-ttu-id="53bde-218">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="53bde-218">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53bde-219">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53bde-219">JSON representation</span></span>

<span data-ttu-id="53bde-220">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53bde-220">The following is a JSON representation of the resource.</span></span>

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
