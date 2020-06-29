---
title: educationClass 资源类型
description: 表示学校的课程。 **EducationClass**资源对应于 Microsoft 365 组并共享相同的 ID。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 22f354ff86e055d40a7112cdc71a63fed5e5e5fb
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909686"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="91f97-104">educationClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="91f97-104">educationClass resource type</span></span>

<span data-ttu-id="91f97-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91f97-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91f97-106">表示学校的课程。</span><span class="sxs-lookup"><span data-stu-id="91f97-106">Represents a class within a school.</span></span> <span data-ttu-id="91f97-107">**EducationClass**资源对应于 Microsoft 365 组并共享相同的 ID。</span><span class="sxs-lookup"><span data-stu-id="91f97-107">The **educationClass** resource corresponds to the Microsoft 365 group and shares the same ID.</span></span> <span data-ttu-id="91f97-108">学生是课程的正式成员，教师为所有者，且具有相应权限。</span><span class="sxs-lookup"><span data-stu-id="91f97-108">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="91f97-109">为使 Microsoft 365 体验正常工作，教师必须是教师和成员集合的成员。</span><span class="sxs-lookup"><span data-stu-id="91f97-109">For Microsoft 365 experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>

## <a name="methods"></a><span data-ttu-id="91f97-110">方法</span><span class="sxs-lookup"><span data-stu-id="91f97-110">Methods</span></span>

| <span data-ttu-id="91f97-111">方法</span><span class="sxs-lookup"><span data-stu-id="91f97-111">Method</span></span>                                                                  | <span data-ttu-id="91f97-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="91f97-112">Return Type</span></span>                                    | <span data-ttu-id="91f97-113">说明</span><span class="sxs-lookup"><span data-stu-id="91f97-113">Description</span></span>                                                                               |
| :---------------------------------------------------------------------- | :--------------------------------------------- | :---------------------------------------------------------------------------------------- |
| [<span data-ttu-id="91f97-114">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="91f97-114">Get educationClass</span></span>](../api/educationclass-get.md)                      | <span data-ttu-id="91f97-115">[educationClass]</span><span class="sxs-lookup"><span data-stu-id="91f97-115">[educationClass]</span></span>                               | <span data-ttu-id="91f97-116">读取 **educationClass** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="91f97-116">Read properties and relationships of an **educationClass** object.</span></span>                        |
| [<span data-ttu-id="91f97-117">Add member</span><span class="sxs-lookup"><span data-stu-id="91f97-117">Add member</span></span>](../api/educationclass-post-members.md)                     | <span data-ttu-id="91f97-118">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="91f97-118">[educationUser]</span></span>                                | <span data-ttu-id="91f97-119">通过发布到 members 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="91f97-119">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>  |
| [<span data-ttu-id="91f97-120">List members</span><span class="sxs-lookup"><span data-stu-id="91f97-120">List members</span></span>](../api/educationclass-list-members.md)                   | <span data-ttu-id="91f97-121">[educationUser] 集合</span><span class="sxs-lookup"><span data-stu-id="91f97-121">[educationUser] collection</span></span>                     | <span data-ttu-id="91f97-122">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="91f97-122">Get an **educationUser** object collection.</span></span>                                               |
| [<span data-ttu-id="91f97-123">Remove student</span><span class="sxs-lookup"><span data-stu-id="91f97-123">Remove student</span></span>](../api/educationclass-delete-members.md)               | <span data-ttu-id="91f97-124">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="91f97-124">[educationUser]</span></span>                                | <span data-ttu-id="91f97-125">通过成员导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="91f97-125">Remove an **educationUser** from the class through the members navigation property.</span></span>       |
| [<span data-ttu-id="91f97-126">List schools</span><span class="sxs-lookup"><span data-stu-id="91f97-126">List schools</span></span>](../api/educationclass-list-schools.md)                   | <span data-ttu-id="91f97-127">[educationSchool] 集合</span><span class="sxs-lookup"><span data-stu-id="91f97-127">[educationSchool] collection</span></span>                   | <span data-ttu-id="91f97-128">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="91f97-128">Get an **educationSchool** object collection.</span></span>                                             |
| [<span data-ttu-id="91f97-129">Add teacher</span><span class="sxs-lookup"><span data-stu-id="91f97-129">Add teacher</span></span>](../api/educationclass-post-teachers.md)                   | <span data-ttu-id="91f97-130">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="91f97-130">[educationUser]</span></span>                                | <span data-ttu-id="91f97-131">通过发布到 teachers 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="91f97-131">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span> |
| [<span data-ttu-id="91f97-132">List teachers</span><span class="sxs-lookup"><span data-stu-id="91f97-132">List teachers</span></span>](../api/educationclass-list-teachers.md)                 | <span data-ttu-id="91f97-133">[educationUser] 集合</span><span class="sxs-lookup"><span data-stu-id="91f97-133">[educationUser] collection</span></span>                     | <span data-ttu-id="91f97-134">获取课程的教师列表。</span><span class="sxs-lookup"><span data-stu-id="91f97-134">Get a list of teachers for the class.</span></span>                                                     |
| [<span data-ttu-id="91f97-135">Remove teacher</span><span class="sxs-lookup"><span data-stu-id="91f97-135">Remove teacher</span></span>](../api/educationclass-delete-teachers.md)              | <span data-ttu-id="91f97-136">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="91f97-136">[educationUser]</span></span>                                | <span data-ttu-id="91f97-137">通过教师导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="91f97-137">Remove an **educationUser** from the class through the teachers navigation property.</span></span>      |
| [<span data-ttu-id="91f97-138">创建 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="91f97-138">Create educationAssignment</span></span>](../api/educationclass-post-assignments.md) | <span data-ttu-id="91f97-139">[educationAssignment]</span><span class="sxs-lookup"><span data-stu-id="91f97-139">[educationAssignment]</span></span>                          | <span data-ttu-id="91f97-140">通过发布到工作分配集合创建新的**educationAssignment** 。</span><span class="sxs-lookup"><span data-stu-id="91f97-140">Create a new **educationAssignment** by posting to the assignments collection.</span></span>            |
| [<span data-ttu-id="91f97-141">列出作业</span><span class="sxs-lookup"><span data-stu-id="91f97-141">List assignments</span></span>](../api/educationclass-list-assignments.md)           | <span data-ttu-id="91f97-142">[educationAssignment]集合</span><span class="sxs-lookup"><span data-stu-id="91f97-142">[educationAssignment]collection</span></span>                | <span data-ttu-id="91f97-143">获取**educationAssignment**对象集合。</span><span class="sxs-lookup"><span data-stu-id="91f97-143">Get an **educationAssignment** object collection.</span></span>                                         |
| [<span data-ttu-id="91f97-144">Get group</span><span class="sxs-lookup"><span data-stu-id="91f97-144">Get group</span></span>](../api/educationclass-get-group.md)                         | <span data-ttu-id="91f97-145">[组]</span><span class="sxs-lookup"><span data-stu-id="91f97-145">[group]</span></span>                                        | <span data-ttu-id="91f97-146">获取与此**educationClass**对应的 Microsoft 365**组**。</span><span class="sxs-lookup"><span data-stu-id="91f97-146">Get the Microsoft 365 **group** that corresponds to this **educationClass**.</span></span>                 |
| [<span data-ttu-id="91f97-147">创建 educationCategory</span><span class="sxs-lookup"><span data-stu-id="91f97-147">Create educationCategory</span></span>](../api/educationclass-post-category.md)      | <span data-ttu-id="91f97-148">[educationCategory]</span><span class="sxs-lookup"><span data-stu-id="91f97-148">[educationCategory]</span></span>                            | <span data-ttu-id="91f97-149">为此类创建新的**educationCategory** 。</span><span class="sxs-lookup"><span data-stu-id="91f97-149">Create a new **educationCategory** for this class.</span></span>                                        |
| [<span data-ttu-id="91f97-150">List categories</span><span class="sxs-lookup"><span data-stu-id="91f97-150">List categories</span></span>](../api/educationclass-list-categories.md)             | <span data-ttu-id="91f97-151">[educationCategory]集合</span><span class="sxs-lookup"><span data-stu-id="91f97-151">[educationCategory] collection</span></span>                 | <span data-ttu-id="91f97-152">获取属于此类的**educationCategory**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="91f97-152">Get a list of **educationCategory** objects belonging to this class.</span></span>                      |
| [<span data-ttu-id="91f97-153">Update</span><span class="sxs-lookup"><span data-stu-id="91f97-153">Update</span></span>](../api/educationclass-update.md)                               | <span data-ttu-id="91f97-154">[educationClass]</span><span class="sxs-lookup"><span data-stu-id="91f97-154">[educationClass]</span></span>                               | <span data-ttu-id="91f97-155">更新 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="91f97-155">Update **educationClass** object.</span></span>                                                         |
| [<span data-ttu-id="91f97-156">删除</span><span class="sxs-lookup"><span data-stu-id="91f97-156">Delete</span></span>](../api/educationclass-delete.md)                               | <span data-ttu-id="91f97-157">无</span><span class="sxs-lookup"><span data-stu-id="91f97-157">None</span></span>                                           | <span data-ttu-id="91f97-158">删除 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="91f97-158">Delete **educationClass** object.</span></span>                                                         |
| [<span data-ttu-id="91f97-159">Delta</span><span class="sxs-lookup"><span data-stu-id="91f97-159">Delta</span></span>](../api/educationclass-delta.md)                                 | <span data-ttu-id="91f97-160">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="91f97-160">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="91f97-161">获取**educationClasses**的增量更改</span><span class="sxs-lookup"><span data-stu-id="91f97-161">Get incremental changes for **educationClasses**</span></span>                                          |

## <a name="properties"></a><span data-ttu-id="91f97-162">属性</span><span class="sxs-lookup"><span data-stu-id="91f97-162">Properties</span></span>

| <span data-ttu-id="91f97-163">属性</span><span class="sxs-lookup"><span data-stu-id="91f97-163">Property</span></span>       | <span data-ttu-id="91f97-164">类型</span><span class="sxs-lookup"><span data-stu-id="91f97-164">Type</span></span>                                  | <span data-ttu-id="91f97-165">说明</span><span class="sxs-lookup"><span data-stu-id="91f97-165">Description</span></span>                                                                             |
| :------------- | :------------------------------------ | :-------------------------------------------------------------------------------------- |
| <span data-ttu-id="91f97-166">id</span><span class="sxs-lookup"><span data-stu-id="91f97-166">id</span></span>             | <span data-ttu-id="91f97-167">字符串</span><span class="sxs-lookup"><span data-stu-id="91f97-167">String</span></span>                                | <span data-ttu-id="91f97-168">课程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="91f97-168">Unique identifier for the class.</span></span>                                                        |
| <span data-ttu-id="91f97-169">classCode</span><span class="sxs-lookup"><span data-stu-id="91f97-169">classCode</span></span>      | <span data-ttu-id="91f97-170">String</span><span class="sxs-lookup"><span data-stu-id="91f97-170">String</span></span>                                | <span data-ttu-id="91f97-171">学校用于标识课程的课程代码。</span><span class="sxs-lookup"><span data-stu-id="91f97-171">Class code used by the school to identify the class.</span></span>                                    |
| <span data-ttu-id="91f97-172">采取</span><span class="sxs-lookup"><span data-stu-id="91f97-172">course</span></span>         | [<span data-ttu-id="91f97-173">educationCourse</span><span class="sxs-lookup"><span data-stu-id="91f97-173">educationCourse</span></span>](educationcourse.md) | <span data-ttu-id="91f97-174">课堂课程信息</span><span class="sxs-lookup"><span data-stu-id="91f97-174">Course information for the class</span></span>                                                        |
| <span data-ttu-id="91f97-175">createdBy</span><span class="sxs-lookup"><span data-stu-id="91f97-175">createdBy</span></span>      | <span data-ttu-id="91f97-176">[identitySet]</span><span class="sxs-lookup"><span data-stu-id="91f97-176">[identitySet]</span></span>                         | <span data-ttu-id="91f97-177">创建了课程的实体</span><span class="sxs-lookup"><span data-stu-id="91f97-177">Entity who created the class</span></span>                                                            |
| <span data-ttu-id="91f97-178">description</span><span class="sxs-lookup"><span data-stu-id="91f97-178">description</span></span>    | <span data-ttu-id="91f97-179">String</span><span class="sxs-lookup"><span data-stu-id="91f97-179">String</span></span>                                | <span data-ttu-id="91f97-180">课程说明。</span><span class="sxs-lookup"><span data-stu-id="91f97-180">Description of the class.</span></span>                                                               |
| <span data-ttu-id="91f97-181">displayName</span><span class="sxs-lookup"><span data-stu-id="91f97-181">displayName</span></span>    | <span data-ttu-id="91f97-182">String</span><span class="sxs-lookup"><span data-stu-id="91f97-182">String</span></span>                                | <span data-ttu-id="91f97-183">课程名称。</span><span class="sxs-lookup"><span data-stu-id="91f97-183">Name of the class.</span></span>                                                                      |
| <span data-ttu-id="91f97-184">externalId</span><span class="sxs-lookup"><span data-stu-id="91f97-184">externalId</span></span>     | <span data-ttu-id="91f97-185">String</span><span class="sxs-lookup"><span data-stu-id="91f97-185">String</span></span>                                | <span data-ttu-id="91f97-186">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="91f97-186">ID of the class from the syncing system.</span></span>                                                |
| <span data-ttu-id="91f97-187">externalName</span><span class="sxs-lookup"><span data-stu-id="91f97-187">externalName</span></span>   | <span data-ttu-id="91f97-188">String</span><span class="sxs-lookup"><span data-stu-id="91f97-188">String</span></span>                                | <span data-ttu-id="91f97-189">同步系统中的课程名称。</span><span class="sxs-lookup"><span data-stu-id="91f97-189">Name of the class in the syncing system.</span></span>                                                |
| <span data-ttu-id="91f97-190">externalSource</span><span class="sxs-lookup"><span data-stu-id="91f97-190">externalSource</span></span> | <span data-ttu-id="91f97-191">String</span><span class="sxs-lookup"><span data-stu-id="91f97-191">String</span></span>                                | <span data-ttu-id="91f97-192">此课程的创建方式。</span><span class="sxs-lookup"><span data-stu-id="91f97-192">How this class was created.</span></span> <span data-ttu-id="91f97-193">可取值为：`sis`、`manual`、`lms`。</span><span class="sxs-lookup"><span data-stu-id="91f97-193">Possible values are: `sis`, `manual`, `lms`.</span></span> |
| <span data-ttu-id="91f97-194">grade</span><span class="sxs-lookup"><span data-stu-id="91f97-194">grade</span></span>          | <span data-ttu-id="91f97-195">String</span><span class="sxs-lookup"><span data-stu-id="91f97-195">String</span></span>                                | <span data-ttu-id="91f97-196">课程的年级级别。</span><span class="sxs-lookup"><span data-stu-id="91f97-196">Grade level of the class.</span></span>                                                               |
| <span data-ttu-id="91f97-197">mailNickname</span><span class="sxs-lookup"><span data-stu-id="91f97-197">mailNickname</span></span>   | <span data-ttu-id="91f97-198">字符串</span><span class="sxs-lookup"><span data-stu-id="91f97-198">String</span></span>                                | <span data-ttu-id="91f97-199">向所有成员发送电子邮件的邮件名称（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="91f97-199">Mail name for sending email to all members, if this is enabled.</span></span>                         |
| <span data-ttu-id="91f97-200">term</span><span class="sxs-lookup"><span data-stu-id="91f97-200">term</span></span>           | <span data-ttu-id="91f97-201">[educationTerm]</span><span class="sxs-lookup"><span data-stu-id="91f97-201">[educationTerm]</span></span>                       | <span data-ttu-id="91f97-202">类的术语。</span><span class="sxs-lookup"><span data-stu-id="91f97-202">Term for the class.</span></span>                                                                     |

## <a name="relationships"></a><span data-ttu-id="91f97-203">关系</span><span class="sxs-lookup"><span data-stu-id="91f97-203">Relationships</span></span>

| <span data-ttu-id="91f97-204">关系</span><span class="sxs-lookup"><span data-stu-id="91f97-204">Relationship</span></span> | <span data-ttu-id="91f97-205">类型</span><span class="sxs-lookup"><span data-stu-id="91f97-205">Type</span></span>                             | <span data-ttu-id="91f97-206">说明</span><span class="sxs-lookup"><span data-stu-id="91f97-206">Description</span></span>                                               |
| :----------- | :------------------------------- | :-------------------------------------------------------- |
| <span data-ttu-id="91f97-207">assignments</span><span class="sxs-lookup"><span data-stu-id="91f97-207">assignments</span></span>  | <span data-ttu-id="91f97-208">[educationAssignment]集合</span><span class="sxs-lookup"><span data-stu-id="91f97-208">[educationAssignment] collection</span></span> | <span data-ttu-id="91f97-209">与此类关联的所有工作分配。</span><span class="sxs-lookup"><span data-stu-id="91f97-209">All assignments associated with this class.</span></span> <span data-ttu-id="91f97-210">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="91f97-210">Nullable.</span></span>     |
| <span data-ttu-id="91f97-211">members</span><span class="sxs-lookup"><span data-stu-id="91f97-211">members</span></span>      | <span data-ttu-id="91f97-212">[educationUser] 集合</span><span class="sxs-lookup"><span data-stu-id="91f97-212">[educationUser] collection</span></span>       | <span data-ttu-id="91f97-213">课程中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="91f97-213">All users in the class.</span></span> <span data-ttu-id="91f97-214">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="91f97-214">Nullable.</span></span>                         |
| <span data-ttu-id="91f97-215">schools</span><span class="sxs-lookup"><span data-stu-id="91f97-215">schools</span></span>      | <span data-ttu-id="91f97-216">[educationSchool] 集合</span><span class="sxs-lookup"><span data-stu-id="91f97-216">[educationSchool] collection</span></span>     | <span data-ttu-id="91f97-217">与此课程相关的所有学校。</span><span class="sxs-lookup"><span data-stu-id="91f97-217">All schools that this class is associated with.</span></span> <span data-ttu-id="91f97-218">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="91f97-218">Nullable.</span></span> |
| <span data-ttu-id="91f97-219">teachers</span><span class="sxs-lookup"><span data-stu-id="91f97-219">teachers</span></span>     | <span data-ttu-id="91f97-220">[educationUser] 集合</span><span class="sxs-lookup"><span data-stu-id="91f97-220">[educationUser] collection</span></span>       | <span data-ttu-id="91f97-221">课程中的所有教师。</span><span class="sxs-lookup"><span data-stu-id="91f97-221">All teachers in the class.</span></span> <span data-ttu-id="91f97-222">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="91f97-222">Nullable.</span></span>                      |

## <a name="json-representation"></a><span data-ttu-id="91f97-223">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91f97-223">JSON representation</span></span>

<span data-ttu-id="91f97-224">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91f97-224">The following is a JSON representation of the resource.</span></span>

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
    "Error: Resource educationClass has documented navigation properties, but we thought it was a complex type!",
    "Resource educationClass has documented navigation properties, but we thought it was a complex type!"
  ]

}-->

[educationclass]: educationclass.md
[educationuser]: educationuser.md
[educationassignment]: educationassignment.md
[educationcourse]: educationcourse.md
[educationcategory]: educationcategory.md
[educationschool]: educationschool.md
[educationterm]: educationterm.md
[了解 identityset]: identityset.md
[identityset]: identityset.md
[组]: group.md
[group]: group.md
