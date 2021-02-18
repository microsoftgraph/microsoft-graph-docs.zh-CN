---
title: educationClass 资源类型
description: 表示学校的课程。 **educationClass** 资源对应于 Microsoft 365 组并共享相同的 ID。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d699e137ad2a80c5a53aa258f986aad968734269
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292882"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="ad134-104">educationClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad134-104">educationClass resource type</span></span>

<span data-ttu-id="ad134-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad134-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad134-106">表示学校的课程。</span><span class="sxs-lookup"><span data-stu-id="ad134-106">Represents a class within a school.</span></span> <span data-ttu-id="ad134-107">**educationClass** 资源当前对应于 Microsoft 365 [组并]共享相同的 ID。</span><span class="sxs-lookup"><span data-stu-id="ad134-107">The **educationClass** resource currently corresponds to a Microsoft 365 [group] and shares the same ID.</span></span>
<span data-ttu-id="ad134-108">学生是课程的常规成员，教师是所有者并且具有适当的权利。</span><span class="sxs-lookup"><span data-stu-id="ad134-108">Students are regular members of the class, and Teachers are owners and have appropriate rights.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ad134-109">若要使 Microsoft 365 体验正常工作，教师必须是教师和成员集合的成员。</span><span class="sxs-lookup"><span data-stu-id="ad134-109">For Microsoft 365 experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>

## <a name="methods"></a><span data-ttu-id="ad134-110">方法</span><span class="sxs-lookup"><span data-stu-id="ad134-110">Methods</span></span>

| <span data-ttu-id="ad134-111">方法</span><span class="sxs-lookup"><span data-stu-id="ad134-111">Method</span></span>                                                                  | <span data-ttu-id="ad134-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="ad134-112">Return Type</span></span>                                    | <span data-ttu-id="ad134-113">说明</span><span class="sxs-lookup"><span data-stu-id="ad134-113">Description</span></span>                                                                               |
| :---------------------------------------------------------------------- | :--------------------------------------------- | :---------------------------------------------------------------------------------------- |
| [<span data-ttu-id="ad134-114">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="ad134-114">Get educationClass</span></span>](../api/educationclass-get.md)                      | <span data-ttu-id="ad134-115">[educationClass]</span><span class="sxs-lookup"><span data-stu-id="ad134-115">[educationClass]</span></span>                               | <span data-ttu-id="ad134-116">读取 **educationClass** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ad134-116">Read properties and relationships of an **educationClass** object.</span></span>                        |
| [<span data-ttu-id="ad134-117">Add member</span><span class="sxs-lookup"><span data-stu-id="ad134-117">Add member</span></span>](../api/educationclass-post-members.md)                     | <span data-ttu-id="ad134-118">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="ad134-118">[educationUser]</span></span>                                | <span data-ttu-id="ad134-119">通过发布到 members 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="ad134-119">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>  |
| [<span data-ttu-id="ad134-120">List members</span><span class="sxs-lookup"><span data-stu-id="ad134-120">List members</span></span>](../api/educationclass-list-members.md)                   | <span data-ttu-id="ad134-121">[educationUser] 集合</span><span class="sxs-lookup"><span data-stu-id="ad134-121">[educationUser] collection</span></span>                     | <span data-ttu-id="ad134-122">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ad134-122">Get an **educationUser** object collection.</span></span>                                               |
| [<span data-ttu-id="ad134-123">Remove student</span><span class="sxs-lookup"><span data-stu-id="ad134-123">Remove student</span></span>](../api/educationclass-delete-members.md)               | <span data-ttu-id="ad134-124">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="ad134-124">[educationUser]</span></span>                                | <span data-ttu-id="ad134-125">通过成员导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="ad134-125">Remove an **educationUser** from the class through the members navigation property.</span></span>       |
| [<span data-ttu-id="ad134-126">List schools</span><span class="sxs-lookup"><span data-stu-id="ad134-126">List schools</span></span>](../api/educationclass-list-schools.md)                   | <span data-ttu-id="ad134-127">[educationSchool] 集合</span><span class="sxs-lookup"><span data-stu-id="ad134-127">[educationSchool] collection</span></span>                   | <span data-ttu-id="ad134-128">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ad134-128">Get an **educationSchool** object collection.</span></span>                                             |
| [<span data-ttu-id="ad134-129">Add teacher</span><span class="sxs-lookup"><span data-stu-id="ad134-129">Add teacher</span></span>](../api/educationclass-post-teachers.md)                   | <span data-ttu-id="ad134-130">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="ad134-130">[educationUser]</span></span>                                | <span data-ttu-id="ad134-131">通过发布到 teachers 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="ad134-131">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span> |
| [<span data-ttu-id="ad134-132">List teachers</span><span class="sxs-lookup"><span data-stu-id="ad134-132">List teachers</span></span>](../api/educationclass-list-teachers.md)                 | <span data-ttu-id="ad134-133">[educationUser] 集合</span><span class="sxs-lookup"><span data-stu-id="ad134-133">[educationUser] collection</span></span>                     | <span data-ttu-id="ad134-134">获取课程的教师列表。</span><span class="sxs-lookup"><span data-stu-id="ad134-134">Get a list of teachers for the class.</span></span>                                                     |
| [<span data-ttu-id="ad134-135">Remove teacher</span><span class="sxs-lookup"><span data-stu-id="ad134-135">Remove teacher</span></span>](../api/educationclass-delete-teachers.md)              | <span data-ttu-id="ad134-136">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="ad134-136">[educationUser]</span></span>                                | <span data-ttu-id="ad134-137">通过教师导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="ad134-137">Remove an **educationUser** from the class through the teachers navigation property.</span></span>      |
| [<span data-ttu-id="ad134-138">创建 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="ad134-138">Create educationAssignment</span></span>](../api/educationclass-post-assignments.md) | <span data-ttu-id="ad134-139">[educationAssignment]</span><span class="sxs-lookup"><span data-stu-id="ad134-139">[educationAssignment]</span></span>                          | <span data-ttu-id="ad134-140">通过发布到作业集合创建新的 **educationAssignment。**</span><span class="sxs-lookup"><span data-stu-id="ad134-140">Create a new **educationAssignment** by posting to the assignments collection.</span></span>            |
| [<span data-ttu-id="ad134-141">列出作业</span><span class="sxs-lookup"><span data-stu-id="ad134-141">List assignments</span></span>](../api/educationclass-list-assignments.md)           | <span data-ttu-id="ad134-142">[educationAssignment]集合</span><span class="sxs-lookup"><span data-stu-id="ad134-142">[educationAssignment]collection</span></span>                | <span data-ttu-id="ad134-143">获取 **educationAssignment** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ad134-143">Get an **educationAssignment** object collection.</span></span>                                         |
| [<span data-ttu-id="ad134-144">Get group</span><span class="sxs-lookup"><span data-stu-id="ad134-144">Get group</span></span>](../api/educationclass-get-group.md)                         | <span data-ttu-id="ad134-145">[组]</span><span class="sxs-lookup"><span data-stu-id="ad134-145">[group]</span></span>                                        | <span data-ttu-id="ad134-146">获取对应于此 **educationClass\*\*\*\*的** Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="ad134-146">Get the Microsoft 365 **group** that corresponds to this **educationClass**.</span></span>              |
| [<span data-ttu-id="ad134-147">创建 educationCategory</span><span class="sxs-lookup"><span data-stu-id="ad134-147">Create educationCategory</span></span>](../api/educationclass-post-category.md)      | <span data-ttu-id="ad134-148">[educationCategory]</span><span class="sxs-lookup"><span data-stu-id="ad134-148">[educationCategory]</span></span>                            | <span data-ttu-id="ad134-149">为此课程 **创建新的 educationCategory。**</span><span class="sxs-lookup"><span data-stu-id="ad134-149">Create a new **educationCategory** for this class.</span></span>                                        |
| [<span data-ttu-id="ad134-150">List categories</span><span class="sxs-lookup"><span data-stu-id="ad134-150">List categories</span></span>](../api/educationclass-list-categories.md)             | <span data-ttu-id="ad134-151">[educationCategory] 集合</span><span class="sxs-lookup"><span data-stu-id="ad134-151">[educationCategory] collection</span></span>                 | <span data-ttu-id="ad134-152">获取属于 **此类的 educationCategory** 对象列表。</span><span class="sxs-lookup"><span data-stu-id="ad134-152">Get a list of **educationCategory** objects belonging to this class.</span></span>                      |
| [<span data-ttu-id="ad134-153">Update</span><span class="sxs-lookup"><span data-stu-id="ad134-153">Update</span></span>](../api/educationclass-update.md)                               | <span data-ttu-id="ad134-154">[educationClass]</span><span class="sxs-lookup"><span data-stu-id="ad134-154">[educationClass]</span></span>                               | <span data-ttu-id="ad134-155">更新 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="ad134-155">Update **educationClass** object.</span></span>                                                         |
| [<span data-ttu-id="ad134-156">删除</span><span class="sxs-lookup"><span data-stu-id="ad134-156">Delete</span></span>](../api/educationclass-delete.md)                               | <span data-ttu-id="ad134-157">无</span><span class="sxs-lookup"><span data-stu-id="ad134-157">None</span></span>                                           | <span data-ttu-id="ad134-158">删除 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="ad134-158">Delete **educationClass** object.</span></span>                                                         |
| [<span data-ttu-id="ad134-159">Delta</span><span class="sxs-lookup"><span data-stu-id="ad134-159">Delta</span></span>](../api/educationclass-delta.md)                                 | <span data-ttu-id="ad134-160">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ad134-160">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="ad134-161">获取 **educationClasses 的增量更改**</span><span class="sxs-lookup"><span data-stu-id="ad134-161">Get incremental changes for **educationClasses**</span></span>                                          |

## <a name="properties"></a><span data-ttu-id="ad134-162">属性</span><span class="sxs-lookup"><span data-stu-id="ad134-162">Properties</span></span>

| <span data-ttu-id="ad134-163">属性</span><span class="sxs-lookup"><span data-stu-id="ad134-163">Property</span></span>             | <span data-ttu-id="ad134-164">类型</span><span class="sxs-lookup"><span data-stu-id="ad134-164">Type</span></span>                                  | <span data-ttu-id="ad134-165">说明</span><span class="sxs-lookup"><span data-stu-id="ad134-165">Description</span></span>                                                                                                                                                          |
| :------------------- | :------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ad134-166">id</span><span class="sxs-lookup"><span data-stu-id="ad134-166">id</span></span>                   | <span data-ttu-id="ad134-167">String</span><span class="sxs-lookup"><span data-stu-id="ad134-167">String</span></span>                                | <span data-ttu-id="ad134-168">课程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ad134-168">Unique identifier for the class.</span></span>                                                                                                                                     |
| <span data-ttu-id="ad134-169">classCode</span><span class="sxs-lookup"><span data-stu-id="ad134-169">classCode</span></span>            | <span data-ttu-id="ad134-170">String</span><span class="sxs-lookup"><span data-stu-id="ad134-170">String</span></span>                                | <span data-ttu-id="ad134-171">学校用于标识课程的课程代码。</span><span class="sxs-lookup"><span data-stu-id="ad134-171">Class code used by the school to identify the class.</span></span>                                                                                                                 |
| <span data-ttu-id="ad134-172">课程</span><span class="sxs-lookup"><span data-stu-id="ad134-172">course</span></span>               | [<span data-ttu-id="ad134-173">educationCourse</span><span class="sxs-lookup"><span data-stu-id="ad134-173">educationCourse</span></span>](educationcourse.md) | <span data-ttu-id="ad134-174">课程的课程信息</span><span class="sxs-lookup"><span data-stu-id="ad134-174">Course information for the class</span></span>                                                                                                                                     |
| <span data-ttu-id="ad134-175">createdBy</span><span class="sxs-lookup"><span data-stu-id="ad134-175">createdBy</span></span>            | <span data-ttu-id="ad134-176">[identitySet]</span><span class="sxs-lookup"><span data-stu-id="ad134-176">[identitySet]</span></span>                         | <span data-ttu-id="ad134-177">创建了课程的实体</span><span class="sxs-lookup"><span data-stu-id="ad134-177">Entity who created the class</span></span>                                                                                                                                         |
| <span data-ttu-id="ad134-178">description</span><span class="sxs-lookup"><span data-stu-id="ad134-178">description</span></span>          | <span data-ttu-id="ad134-179">String</span><span class="sxs-lookup"><span data-stu-id="ad134-179">String</span></span>                                | <span data-ttu-id="ad134-180">课程说明。</span><span class="sxs-lookup"><span data-stu-id="ad134-180">Description of the class.</span></span>                                                                                                                                            |
| <span data-ttu-id="ad134-181">displayName</span><span class="sxs-lookup"><span data-stu-id="ad134-181">displayName</span></span>          | <span data-ttu-id="ad134-182">String</span><span class="sxs-lookup"><span data-stu-id="ad134-182">String</span></span>                                | <span data-ttu-id="ad134-183">课程名称。</span><span class="sxs-lookup"><span data-stu-id="ad134-183">Name of the class.</span></span>                                                                                                                                                   |
| <span data-ttu-id="ad134-184">externalId</span><span class="sxs-lookup"><span data-stu-id="ad134-184">externalId</span></span>           | <span data-ttu-id="ad134-185">String</span><span class="sxs-lookup"><span data-stu-id="ad134-185">String</span></span>                                | <span data-ttu-id="ad134-186">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="ad134-186">ID of the class from the syncing system.</span></span>                                                                                                                             |
| <span data-ttu-id="ad134-187">externalName</span><span class="sxs-lookup"><span data-stu-id="ad134-187">externalName</span></span>         | <span data-ttu-id="ad134-188">String</span><span class="sxs-lookup"><span data-stu-id="ad134-188">String</span></span>                                | <span data-ttu-id="ad134-189">同步系统中的课程名称。</span><span class="sxs-lookup"><span data-stu-id="ad134-189">Name of the class in the syncing system.</span></span>                                                                                                                             |
| <span data-ttu-id="ad134-190">externalSource</span><span class="sxs-lookup"><span data-stu-id="ad134-190">externalSource</span></span>       | <span data-ttu-id="ad134-191">String</span><span class="sxs-lookup"><span data-stu-id="ad134-191">String</span></span>                                | <span data-ttu-id="ad134-192">此资源的外部源类型由 (自动确定 `externalSourceDetail`) 。</span><span class="sxs-lookup"><span data-stu-id="ad134-192">The type of external source this resource was generated from (automatically determined from `externalSourceDetail`).</span></span> <span data-ttu-id="ad134-193">可能的值为： `sis`、 `lms`或 `manual`。</span><span class="sxs-lookup"><span data-stu-id="ad134-193">Possible values are: `sis`, `lms`, or `manual`.</span></span> |
| <span data-ttu-id="ad134-194">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="ad134-194">externalSourceDetail</span></span> | <span data-ttu-id="ad134-195">String</span><span class="sxs-lookup"><span data-stu-id="ad134-195">String</span></span>                                | <span data-ttu-id="ad134-196">生成这些资源的外部源的名称。</span><span class="sxs-lookup"><span data-stu-id="ad134-196">The name of the external source this resources was generated from.</span></span>                                                                                                   |
| <span data-ttu-id="ad134-197">grade</span><span class="sxs-lookup"><span data-stu-id="ad134-197">grade</span></span>                | <span data-ttu-id="ad134-198">String</span><span class="sxs-lookup"><span data-stu-id="ad134-198">String</span></span>                                | <span data-ttu-id="ad134-199">课程的级别。</span><span class="sxs-lookup"><span data-stu-id="ad134-199">Grade level of the class.</span></span>                                                                                                                                            |
| <span data-ttu-id="ad134-200">mailNickname</span><span class="sxs-lookup"><span data-stu-id="ad134-200">mailNickname</span></span>         | <span data-ttu-id="ad134-201">String</span><span class="sxs-lookup"><span data-stu-id="ad134-201">String</span></span>                                | <span data-ttu-id="ad134-202">向所有成员发送电子邮件的邮件名称（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="ad134-202">Mail name for sending email to all members, if this is enabled.</span></span>                                                                                                      |
| <span data-ttu-id="ad134-203">term</span><span class="sxs-lookup"><span data-stu-id="ad134-203">term</span></span>                 | <span data-ttu-id="ad134-204">[educationTerm]</span><span class="sxs-lookup"><span data-stu-id="ad134-204">[educationTerm]</span></span>                       | <span data-ttu-id="ad134-205">类的术语。</span><span class="sxs-lookup"><span data-stu-id="ad134-205">Term for the class.</span></span>                                                                                                                                                  |

## <a name="relationships"></a><span data-ttu-id="ad134-206">关系</span><span class="sxs-lookup"><span data-stu-id="ad134-206">Relationships</span></span>

| <span data-ttu-id="ad134-207">关系</span><span class="sxs-lookup"><span data-stu-id="ad134-207">Relationship</span></span> | <span data-ttu-id="ad134-208">类型</span><span class="sxs-lookup"><span data-stu-id="ad134-208">Type</span></span>                             | <span data-ttu-id="ad134-209">说明</span><span class="sxs-lookup"><span data-stu-id="ad134-209">Description</span></span>                                               |
| :----------- | :------------------------------- | :-------------------------------------------------------- |
| <span data-ttu-id="ad134-210">assignments</span><span class="sxs-lookup"><span data-stu-id="ad134-210">assignments</span></span>  | <span data-ttu-id="ad134-211">[educationAssignment] 集合</span><span class="sxs-lookup"><span data-stu-id="ad134-211">[educationAssignment] collection</span></span> | <span data-ttu-id="ad134-212">与此类关联的所有工作分配。</span><span class="sxs-lookup"><span data-stu-id="ad134-212">All assignments associated with this class.</span></span> <span data-ttu-id="ad134-213">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="ad134-213">Nullable.</span></span>     |
| <span data-ttu-id="ad134-214">members</span><span class="sxs-lookup"><span data-stu-id="ad134-214">members</span></span>      | <span data-ttu-id="ad134-215">[educationUser] 集合</span><span class="sxs-lookup"><span data-stu-id="ad134-215">[educationUser] collection</span></span>       | <span data-ttu-id="ad134-216">课程中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="ad134-216">All users in the class.</span></span> <span data-ttu-id="ad134-217">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="ad134-217">Nullable.</span></span>                         |
| <span data-ttu-id="ad134-218">schools</span><span class="sxs-lookup"><span data-stu-id="ad134-218">schools</span></span>      | <span data-ttu-id="ad134-219">[educationSchool] 集合</span><span class="sxs-lookup"><span data-stu-id="ad134-219">[educationSchool] collection</span></span>     | <span data-ttu-id="ad134-220">与此课程相关的所有学校。</span><span class="sxs-lookup"><span data-stu-id="ad134-220">All schools that this class is associated with.</span></span> <span data-ttu-id="ad134-221">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="ad134-221">Nullable.</span></span> |
| <span data-ttu-id="ad134-222">teachers</span><span class="sxs-lookup"><span data-stu-id="ad134-222">teachers</span></span>     | <span data-ttu-id="ad134-223">[educationUser] 集合</span><span class="sxs-lookup"><span data-stu-id="ad134-223">[educationUser] collection</span></span>       | <span data-ttu-id="ad134-224">课程中的所有教师。</span><span class="sxs-lookup"><span data-stu-id="ad134-224">All teachers in the class.</span></span> <span data-ttu-id="ad134-225">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="ad134-225">Nullable.</span></span>                      |

## <a name="json-representation"></a><span data-ttu-id="ad134-226">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad134-226">JSON representation</span></span>

<span data-ttu-id="ad134-227">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad134-227">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "classCode": "String",
  "course": { "@odata.type": "microsoft.graph.educationCourse" },
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "grade": "string",
  "id": "String (identifier)",
  "mailNickname": "String",
  "term": { "@odata.type": "microsoft.graph.educationTerm" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.educationClass",
  "description": "educationUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]

}-->

[educationclass]: educationclass.md
[educationuser]: educationuser.md
[educationassignment]: educationassignment.md
[educationcourse]: educationcourse.md
[educationcategory]: educationcategory.md
[educationschool]: educationschool.md
[educationterm]: educationterm.md
[identityset]: identityset.md
[组]: group.md
[group]: group.md


