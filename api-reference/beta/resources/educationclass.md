---
title: educationClass 资源类型
description: 表示学校的课程。 **educationClass** 资源对应于 Office 365 组并共享同一个 ID。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0bc9fa375e3f22087fbf268933370d8a6222654e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006365"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="328d0-104">educationClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="328d0-104">educationClass resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="328d0-105">表示学校的课程。</span><span class="sxs-lookup"><span data-stu-id="328d0-105">Represents a class within a school.</span></span> <span data-ttu-id="328d0-106">**educationClass** 资源对应于 Office 365 组并共享同一个 ID。</span><span class="sxs-lookup"><span data-stu-id="328d0-106">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="328d0-107">学生是课程的正式成员，教师为所有者，且具有相应权限。</span><span class="sxs-lookup"><span data-stu-id="328d0-107">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="328d0-108">若要使 Office 365 体验正常工作, 教师必须是教师和成员集合的成员。</span><span class="sxs-lookup"><span data-stu-id="328d0-108">For Office 365 experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>

## <a name="methods"></a><span data-ttu-id="328d0-109">方法</span><span class="sxs-lookup"><span data-stu-id="328d0-109">Methods</span></span>

| <span data-ttu-id="328d0-110">方法</span><span class="sxs-lookup"><span data-stu-id="328d0-110">Method</span></span>                                                                  | <span data-ttu-id="328d0-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="328d0-111">Return Type</span></span>                                    | <span data-ttu-id="328d0-112">说明</span><span class="sxs-lookup"><span data-stu-id="328d0-112">Description</span></span>                                                                               |
| :---------------------------------------------------------------------- | :--------------------------------------------- | :---------------------------------------------------------------------------------------- |
| [<span data-ttu-id="328d0-113">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="328d0-113">Get educationClass</span></span>](../api/educationclass-get.md)                      | <span data-ttu-id="328d0-114">[educationClass]</span><span class="sxs-lookup"><span data-stu-id="328d0-114">[educationClass]</span></span>                               | <span data-ttu-id="328d0-115">读取 **educationClass** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="328d0-115">Read properties and relationships of an **educationClass** object.</span></span>                        |
| [<span data-ttu-id="328d0-116">Add member</span><span class="sxs-lookup"><span data-stu-id="328d0-116">Add member</span></span>](../api/educationclass-post-members.md)                     | <span data-ttu-id="328d0-117">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="328d0-117">[educationUser]</span></span>                                | <span data-ttu-id="328d0-118">通过发布到 members 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="328d0-118">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>  |
| [<span data-ttu-id="328d0-119">List members</span><span class="sxs-lookup"><span data-stu-id="328d0-119">List members</span></span>](../api/educationclass-list-members.md)                   | <span data-ttu-id="328d0-120">[educationUser] 集合</span><span class="sxs-lookup"><span data-stu-id="328d0-120">[educationUser] collection</span></span>                     | <span data-ttu-id="328d0-121">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="328d0-121">Get an **educationUser** object collection.</span></span>                                               |
| [<span data-ttu-id="328d0-122">Remove student</span><span class="sxs-lookup"><span data-stu-id="328d0-122">Remove student</span></span>](../api/educationclass-delete-members.md)               | <span data-ttu-id="328d0-123">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="328d0-123">[educationUser]</span></span>                                | <span data-ttu-id="328d0-124">通过成员导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="328d0-124">Remove an **educationUser** from the class through the members navigation property.</span></span>       |
| [<span data-ttu-id="328d0-125">List schools</span><span class="sxs-lookup"><span data-stu-id="328d0-125">List schools</span></span>](../api/educationclass-list-schools.md)                   | <span data-ttu-id="328d0-126">[educationSchool] 集合</span><span class="sxs-lookup"><span data-stu-id="328d0-126">[educationSchool] collection</span></span>                   | <span data-ttu-id="328d0-127">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="328d0-127">Get an **educationSchool** object collection.</span></span>                                             |
| [<span data-ttu-id="328d0-128">Add teacher</span><span class="sxs-lookup"><span data-stu-id="328d0-128">Add teacher</span></span>](../api/educationclass-post-teachers.md)                   | <span data-ttu-id="328d0-129">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="328d0-129">[educationUser]</span></span>                                | <span data-ttu-id="328d0-130">通过发布到 teachers 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="328d0-130">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span> |
| [<span data-ttu-id="328d0-131">List teachers</span><span class="sxs-lookup"><span data-stu-id="328d0-131">List teachers</span></span>](../api/educationclass-list-teachers.md)                 | <span data-ttu-id="328d0-132">[educationUser] 集合</span><span class="sxs-lookup"><span data-stu-id="328d0-132">[educationUser] collection</span></span>                     | <span data-ttu-id="328d0-133">获取课程的教师列表。</span><span class="sxs-lookup"><span data-stu-id="328d0-133">Get a list of teachers for the class.</span></span>                                                     |
| [<span data-ttu-id="328d0-134">Remove teacher</span><span class="sxs-lookup"><span data-stu-id="328d0-134">Remove teacher</span></span>](../api/educationclass-delete-teachers.md)              | <span data-ttu-id="328d0-135">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="328d0-135">[educationUser]</span></span>                                | <span data-ttu-id="328d0-136">通过教师导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="328d0-136">Remove an **educationUser** from the class through the teachers navigation property.</span></span>      |
| [<span data-ttu-id="328d0-137">创建 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="328d0-137">Create educationAssignment</span></span>](../api/educationclass-post-assignments.md) | <span data-ttu-id="328d0-138">[educationAssignment]</span><span class="sxs-lookup"><span data-stu-id="328d0-138">[educationAssignment]</span></span>                          | <span data-ttu-id="328d0-139">通过发布到工作分配集合创建新的**educationAssignment** 。</span><span class="sxs-lookup"><span data-stu-id="328d0-139">Create a new **educationAssignment** by posting to the assignments collection.</span></span>            |
| [<span data-ttu-id="328d0-140">列出作业</span><span class="sxs-lookup"><span data-stu-id="328d0-140">List assignments</span></span>](../api/educationclass-list-assignments.md)           | <span data-ttu-id="328d0-141">[educationAssignment]集合</span><span class="sxs-lookup"><span data-stu-id="328d0-141">[educationAssignment]collection</span></span>                | <span data-ttu-id="328d0-142">获取**educationAssignment**对象集合。</span><span class="sxs-lookup"><span data-stu-id="328d0-142">Get an **educationAssignment** object collection.</span></span>                                         |
| [<span data-ttu-id="328d0-143">Get group</span><span class="sxs-lookup"><span data-stu-id="328d0-143">Get group</span></span>](../api/educationclass-get-group.md)                         | <span data-ttu-id="328d0-144">[组]</span><span class="sxs-lookup"><span data-stu-id="328d0-144">[group]</span></span>                                        | <span data-ttu-id="328d0-145">获得与此 **educationClass** 对应的 Office 365 **group**。</span><span class="sxs-lookup"><span data-stu-id="328d0-145">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>                 |
| [<span data-ttu-id="328d0-146">创建 educationCategory</span><span class="sxs-lookup"><span data-stu-id="328d0-146">Create educationCategory</span></span>](../api/educationclass-post-category.md)      | <span data-ttu-id="328d0-147">[educationCategory]</span><span class="sxs-lookup"><span data-stu-id="328d0-147">[educationCategory]</span></span>                            | <span data-ttu-id="328d0-148">为此类创建新的**educationCategory** 。</span><span class="sxs-lookup"><span data-stu-id="328d0-148">Create a new **educationCategory** for this class.</span></span>                                        |
| [<span data-ttu-id="328d0-149">List categories</span><span class="sxs-lookup"><span data-stu-id="328d0-149">List categories</span></span>](../api/educationclass-list-categories.md)             | <span data-ttu-id="328d0-150">[educationCategory]集合</span><span class="sxs-lookup"><span data-stu-id="328d0-150">[educationCategory] collection</span></span>                 | <span data-ttu-id="328d0-151">获取属于此类的**educationCategory**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="328d0-151">Get a list of **educationCategory** objects belonging to this class.</span></span>                      |
| [<span data-ttu-id="328d0-152">Update</span><span class="sxs-lookup"><span data-stu-id="328d0-152">Update</span></span>](../api/educationclass-update.md)                               | <span data-ttu-id="328d0-153">[educationClass]</span><span class="sxs-lookup"><span data-stu-id="328d0-153">[educationClass]</span></span>                               | <span data-ttu-id="328d0-154">更新 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="328d0-154">Update **educationClass** object.</span></span>                                                         |
| [<span data-ttu-id="328d0-155">删除</span><span class="sxs-lookup"><span data-stu-id="328d0-155">Delete</span></span>](../api/educationclass-delete.md)                               | <span data-ttu-id="328d0-156">无</span><span class="sxs-lookup"><span data-stu-id="328d0-156">None</span></span>                                           | <span data-ttu-id="328d0-157">删除 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="328d0-157">Delete **educationClass** object.</span></span>                                                         |
| [<span data-ttu-id="328d0-158">Delta</span><span class="sxs-lookup"><span data-stu-id="328d0-158">Delta</span></span>](../api/educationclass-delta.md)                                 | <span data-ttu-id="328d0-159">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="328d0-159">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="328d0-160">获取**educationClasses**的增量更改</span><span class="sxs-lookup"><span data-stu-id="328d0-160">Get incremental changes for **educationClasses**</span></span>                                          |

## <a name="properties"></a><span data-ttu-id="328d0-161">属性</span><span class="sxs-lookup"><span data-stu-id="328d0-161">Properties</span></span>

| <span data-ttu-id="328d0-162">属性</span><span class="sxs-lookup"><span data-stu-id="328d0-162">Property</span></span>       | <span data-ttu-id="328d0-163">类型</span><span class="sxs-lookup"><span data-stu-id="328d0-163">Type</span></span>                                  | <span data-ttu-id="328d0-164">说明</span><span class="sxs-lookup"><span data-stu-id="328d0-164">Description</span></span>                                                                             |
| :------------- | :------------------------------------ | :-------------------------------------------------------------------------------------- |
| <span data-ttu-id="328d0-165">id</span><span class="sxs-lookup"><span data-stu-id="328d0-165">id</span></span>             | <span data-ttu-id="328d0-166">字符串</span><span class="sxs-lookup"><span data-stu-id="328d0-166">String</span></span>                                | <span data-ttu-id="328d0-167">课程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="328d0-167">Unique identifier for the class.</span></span>                                                        |
| <span data-ttu-id="328d0-168">classCode</span><span class="sxs-lookup"><span data-stu-id="328d0-168">classCode</span></span>      | <span data-ttu-id="328d0-169">String</span><span class="sxs-lookup"><span data-stu-id="328d0-169">String</span></span>                                | <span data-ttu-id="328d0-170">学校用于标识课程的课程代码。</span><span class="sxs-lookup"><span data-stu-id="328d0-170">Class code used by the school to identify the class.</span></span>                                    |
| <span data-ttu-id="328d0-171">采取</span><span class="sxs-lookup"><span data-stu-id="328d0-171">course</span></span>         | [<span data-ttu-id="328d0-172">educationCourse</span><span class="sxs-lookup"><span data-stu-id="328d0-172">educationCourse</span></span>](educationcourse.md) | <span data-ttu-id="328d0-173">课堂课程信息</span><span class="sxs-lookup"><span data-stu-id="328d0-173">Course information for the class</span></span>                                                        |
| <span data-ttu-id="328d0-174">createdBy</span><span class="sxs-lookup"><span data-stu-id="328d0-174">createdBy</span></span>      | <span data-ttu-id="328d0-175">[identitySet]</span><span class="sxs-lookup"><span data-stu-id="328d0-175">[identitySet]</span></span>                         | <span data-ttu-id="328d0-176">创建了课程的实体</span><span class="sxs-lookup"><span data-stu-id="328d0-176">Entity who created the class</span></span>                                                            |
| <span data-ttu-id="328d0-177">说明</span><span class="sxs-lookup"><span data-stu-id="328d0-177">description</span></span>    | <span data-ttu-id="328d0-178">String</span><span class="sxs-lookup"><span data-stu-id="328d0-178">String</span></span>                                | <span data-ttu-id="328d0-179">课程说明。</span><span class="sxs-lookup"><span data-stu-id="328d0-179">Description of the class.</span></span>                                                               |
| <span data-ttu-id="328d0-180">displayName</span><span class="sxs-lookup"><span data-stu-id="328d0-180">displayName</span></span>    | <span data-ttu-id="328d0-181">String</span><span class="sxs-lookup"><span data-stu-id="328d0-181">String</span></span>                                | <span data-ttu-id="328d0-182">课程名称。</span><span class="sxs-lookup"><span data-stu-id="328d0-182">Name of the class.</span></span>                                                                      |
| <span data-ttu-id="328d0-183">externalId</span><span class="sxs-lookup"><span data-stu-id="328d0-183">externalId</span></span>     | <span data-ttu-id="328d0-184">String</span><span class="sxs-lookup"><span data-stu-id="328d0-184">String</span></span>                                | <span data-ttu-id="328d0-185">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="328d0-185">ID of the class from the syncing system.</span></span>                                                |
| <span data-ttu-id="328d0-186">externalName</span><span class="sxs-lookup"><span data-stu-id="328d0-186">externalName</span></span>   | <span data-ttu-id="328d0-187">String</span><span class="sxs-lookup"><span data-stu-id="328d0-187">String</span></span>                                | <span data-ttu-id="328d0-188">同步系统中的课程名称。</span><span class="sxs-lookup"><span data-stu-id="328d0-188">Name of the class in the syncing system.</span></span>                                                |
| <span data-ttu-id="328d0-189">externalSource</span><span class="sxs-lookup"><span data-stu-id="328d0-189">externalSource</span></span> | <span data-ttu-id="328d0-190">string</span><span class="sxs-lookup"><span data-stu-id="328d0-190">string</span></span>                                | <span data-ttu-id="328d0-191">此课程的创建方式。</span><span class="sxs-lookup"><span data-stu-id="328d0-191">How this class was created.</span></span> <span data-ttu-id="328d0-192">可取值为：`sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="328d0-192">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span> |
| <span data-ttu-id="328d0-193">mailNickname</span><span class="sxs-lookup"><span data-stu-id="328d0-193">mailNickname</span></span>   | <span data-ttu-id="328d0-194">字符串</span><span class="sxs-lookup"><span data-stu-id="328d0-194">String</span></span>                                | <span data-ttu-id="328d0-195">向所有成员发送电子邮件的邮件名称（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="328d0-195">Mail name for sending email to all members, if this is enabled.</span></span>                         |
| <span data-ttu-id="328d0-196">term</span><span class="sxs-lookup"><span data-stu-id="328d0-196">term</span></span>           | <span data-ttu-id="328d0-197">[educationTerm]</span><span class="sxs-lookup"><span data-stu-id="328d0-197">[educationTerm]</span></span>                       | <span data-ttu-id="328d0-198">类的术语。</span><span class="sxs-lookup"><span data-stu-id="328d0-198">Term for the class.</span></span>                                                                     |

## <a name="relationships"></a><span data-ttu-id="328d0-199">关系</span><span class="sxs-lookup"><span data-stu-id="328d0-199">Relationships</span></span>

| <span data-ttu-id="328d0-200">关系</span><span class="sxs-lookup"><span data-stu-id="328d0-200">Relationship</span></span> | <span data-ttu-id="328d0-201">类型</span><span class="sxs-lookup"><span data-stu-id="328d0-201">Type</span></span>                             | <span data-ttu-id="328d0-202">说明</span><span class="sxs-lookup"><span data-stu-id="328d0-202">Description</span></span>                                               |
| :----------- | :------------------------------- | :-------------------------------------------------------- |
| <span data-ttu-id="328d0-203">assignments</span><span class="sxs-lookup"><span data-stu-id="328d0-203">assignments</span></span>  | <span data-ttu-id="328d0-204">[educationAssignment]集合</span><span class="sxs-lookup"><span data-stu-id="328d0-204">[educationAssignment] collection</span></span> | <span data-ttu-id="328d0-205">与此类关联的所有工作分配。</span><span class="sxs-lookup"><span data-stu-id="328d0-205">All assignments associated with this class.</span></span> <span data-ttu-id="328d0-206">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="328d0-206">Nullable.</span></span>     |
| <span data-ttu-id="328d0-207">members</span><span class="sxs-lookup"><span data-stu-id="328d0-207">members</span></span>      | <span data-ttu-id="328d0-208">[educationUser] 集合</span><span class="sxs-lookup"><span data-stu-id="328d0-208">[educationUser] collection</span></span>       | <span data-ttu-id="328d0-209">课程中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="328d0-209">All users in the class.</span></span> <span data-ttu-id="328d0-210">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="328d0-210">Nullable.</span></span>                         |
| <span data-ttu-id="328d0-211">schools</span><span class="sxs-lookup"><span data-stu-id="328d0-211">schools</span></span>      | <span data-ttu-id="328d0-212">[educationSchool] 集合</span><span class="sxs-lookup"><span data-stu-id="328d0-212">[educationSchool] collection</span></span>     | <span data-ttu-id="328d0-213">与此课程相关的所有学校。</span><span class="sxs-lookup"><span data-stu-id="328d0-213">All schools that this class is associated with.</span></span> <span data-ttu-id="328d0-214">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="328d0-214">Nullable.</span></span> |
| <span data-ttu-id="328d0-215">teachers</span><span class="sxs-lookup"><span data-stu-id="328d0-215">teachers</span></span>     | <span data-ttu-id="328d0-216">[educationUser] 集合</span><span class="sxs-lookup"><span data-stu-id="328d0-216">[educationUser] collection</span></span>       | <span data-ttu-id="328d0-217">课程中的所有教师。</span><span class="sxs-lookup"><span data-stu-id="328d0-217">All teachers in the class.</span></span> <span data-ttu-id="328d0-218">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="328d0-218">Nullable.</span></span>                      |

## <a name="json-representation"></a><span data-ttu-id="328d0-219">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="328d0-219">JSON representation</span></span>

<span data-ttu-id="328d0-220">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="328d0-220">The following is a JSON representation of the resource.</span></span>

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
