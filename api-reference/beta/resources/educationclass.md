---
title: educationClass 资源类型
description: 表示学校的课程。 **educationClass** 资源对应于 Office 365 组并共享同一个 ID。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 8a228c329427ae6b3f8da1a971817e88284be917
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750078"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="52c2e-104">educationClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="52c2e-104">educationClass resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52c2e-105">表示学校的课程。</span><span class="sxs-lookup"><span data-stu-id="52c2e-105">Represents a class within a school.</span></span> <span data-ttu-id="52c2e-106">**educationClass** 资源对应于 Office 365 组并共享同一个 ID。</span><span class="sxs-lookup"><span data-stu-id="52c2e-106">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="52c2e-107">学生是课程的正式成员，教师为所有者，且具有相应权限。</span><span class="sxs-lookup"><span data-stu-id="52c2e-107">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="52c2e-108">若要使 Office 365 体验正常工作, 教师必须是教师和成员集合的成员。</span><span class="sxs-lookup"><span data-stu-id="52c2e-108">For Office 365 experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>

## <a name="methods"></a><span data-ttu-id="52c2e-109">方法</span><span class="sxs-lookup"><span data-stu-id="52c2e-109">Methods</span></span>

| <span data-ttu-id="52c2e-110">方法</span><span class="sxs-lookup"><span data-stu-id="52c2e-110">Method</span></span>                                                                  | <span data-ttu-id="52c2e-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="52c2e-111">Return Type</span></span>                                    | <span data-ttu-id="52c2e-112">说明</span><span class="sxs-lookup"><span data-stu-id="52c2e-112">Description</span></span>                                                                               |
| :---------------------------------------------------------------------- | :--------------------------------------------- | :---------------------------------------------------------------------------------------- |
| [<span data-ttu-id="52c2e-113">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="52c2e-113">Get educationClass</span></span>](../api/educationclass-get.md)                      | <span data-ttu-id="52c2e-114">[educationClass]</span><span class="sxs-lookup"><span data-stu-id="52c2e-114">[educationClass]</span></span>                               | <span data-ttu-id="52c2e-115">读取 **educationClass** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="52c2e-115">Read properties and relationships of an **educationClass** object.</span></span>                        |
| [<span data-ttu-id="52c2e-116">Add member</span><span class="sxs-lookup"><span data-stu-id="52c2e-116">Add member</span></span>](../api/educationclass-post-members.md)                     | <span data-ttu-id="52c2e-117">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="52c2e-117">[educationUser]</span></span>                                | <span data-ttu-id="52c2e-118">通过发布到 members 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="52c2e-118">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>  |
| [<span data-ttu-id="52c2e-119">List members</span><span class="sxs-lookup"><span data-stu-id="52c2e-119">List members</span></span>](../api/educationclass-list-members.md)                   | <span data-ttu-id="52c2e-120">[educationUser] 集合</span><span class="sxs-lookup"><span data-stu-id="52c2e-120">[educationUser] collection</span></span>                     | <span data-ttu-id="52c2e-121">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="52c2e-121">Get an **educationUser** object collection.</span></span>                                               |
| [<span data-ttu-id="52c2e-122">Remove student</span><span class="sxs-lookup"><span data-stu-id="52c2e-122">Remove student</span></span>](../api/educationclass-delete-members.md)               | <span data-ttu-id="52c2e-123">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="52c2e-123">[educationUser]</span></span>                                | <span data-ttu-id="52c2e-124">通过成员导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="52c2e-124">Remove an **educationUser** from the class through the members navigation property.</span></span>       |
| [<span data-ttu-id="52c2e-125">List schools</span><span class="sxs-lookup"><span data-stu-id="52c2e-125">List schools</span></span>](../api/educationclass-list-schools.md)                   | <span data-ttu-id="52c2e-126">[educationSchool] 集合</span><span class="sxs-lookup"><span data-stu-id="52c2e-126">[educationSchool] collection</span></span>                   | <span data-ttu-id="52c2e-127">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="52c2e-127">Get an **educationSchool** object collection.</span></span>                                             |
| [<span data-ttu-id="52c2e-128">Add teacher</span><span class="sxs-lookup"><span data-stu-id="52c2e-128">Add teacher</span></span>](../api/educationclass-post-teachers.md)                   | <span data-ttu-id="52c2e-129">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="52c2e-129">[educationUser]</span></span>                                | <span data-ttu-id="52c2e-130">通过发布到 teachers 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="52c2e-130">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span> |
| [<span data-ttu-id="52c2e-131">List teachers</span><span class="sxs-lookup"><span data-stu-id="52c2e-131">List teachers</span></span>](../api/educationclass-list-teachers.md)                 | <span data-ttu-id="52c2e-132">[educationUser] 集合</span><span class="sxs-lookup"><span data-stu-id="52c2e-132">[educationUser] collection</span></span>                     | <span data-ttu-id="52c2e-133">获取课程的教师列表。</span><span class="sxs-lookup"><span data-stu-id="52c2e-133">Get a list of teachers for the class.</span></span>                                                     |
| [<span data-ttu-id="52c2e-134">Remove teacher</span><span class="sxs-lookup"><span data-stu-id="52c2e-134">Remove teacher</span></span>](../api/educationclass-delete-teachers.md)              | <span data-ttu-id="52c2e-135">[educationUser]</span><span class="sxs-lookup"><span data-stu-id="52c2e-135">[educationUser]</span></span>                                | <span data-ttu-id="52c2e-136">通过教师导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="52c2e-136">Remove an **educationUser** from the class through the teachers navigation property.</span></span>      |
| [<span data-ttu-id="52c2e-137">创建 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="52c2e-137">Create educationAssignment</span></span>](../api/educationclass-post-assignments.md) | <span data-ttu-id="52c2e-138">[educationAssignment]</span><span class="sxs-lookup"><span data-stu-id="52c2e-138">[educationAssignment]</span></span>                          | <span data-ttu-id="52c2e-139">通过发布到工作分配集合创建新的**educationAssignment** 。</span><span class="sxs-lookup"><span data-stu-id="52c2e-139">Create a new **educationAssignment** by posting to the assignments collection.</span></span>            |
| [<span data-ttu-id="52c2e-140">列出作业</span><span class="sxs-lookup"><span data-stu-id="52c2e-140">List assignments</span></span>](../api/educationclass-list-assignments.md)           | <span data-ttu-id="52c2e-141">[educationAssignment]集合</span><span class="sxs-lookup"><span data-stu-id="52c2e-141">[educationAssignment]collection</span></span>                | <span data-ttu-id="52c2e-142">获取**educationAssignment**对象集合。</span><span class="sxs-lookup"><span data-stu-id="52c2e-142">Get an **educationAssignment** object collection.</span></span>                                         |
| [<span data-ttu-id="52c2e-143">Get group</span><span class="sxs-lookup"><span data-stu-id="52c2e-143">Get group</span></span>](../api/educationclass-get-group.md)                         | <span data-ttu-id="52c2e-144">[组]</span><span class="sxs-lookup"><span data-stu-id="52c2e-144">[group]</span></span>                                        | <span data-ttu-id="52c2e-145">获得与此 **educationClass** 对应的 Office 365 **group**。</span><span class="sxs-lookup"><span data-stu-id="52c2e-145">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>                 |
| [<span data-ttu-id="52c2e-146">创建 educationCategory</span><span class="sxs-lookup"><span data-stu-id="52c2e-146">Create educationCategory</span></span>](../api/educationclass-post-category.md)      | <span data-ttu-id="52c2e-147">[educationCategory]</span><span class="sxs-lookup"><span data-stu-id="52c2e-147">[educationCategory]</span></span>                            | <span data-ttu-id="52c2e-148">为此类创建新的**educationCategory** 。</span><span class="sxs-lookup"><span data-stu-id="52c2e-148">Create a new **educationCategory** for this class.</span></span>                                        |
| [<span data-ttu-id="52c2e-149">List categories</span><span class="sxs-lookup"><span data-stu-id="52c2e-149">List categories</span></span>](../api/educationclass-list-categories.md)             | <span data-ttu-id="52c2e-150">[educationCategory]集合</span><span class="sxs-lookup"><span data-stu-id="52c2e-150">[educationCategory] collection</span></span>                 | <span data-ttu-id="52c2e-151">获取属于此类的**educationCategory**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="52c2e-151">Get a list of **educationCategory** objects belonging to this class.</span></span>                      |
| [<span data-ttu-id="52c2e-152">Update</span><span class="sxs-lookup"><span data-stu-id="52c2e-152">Update</span></span>](../api/educationclass-update.md)                               | <span data-ttu-id="52c2e-153">[educationClass]</span><span class="sxs-lookup"><span data-stu-id="52c2e-153">[educationClass]</span></span>                               | <span data-ttu-id="52c2e-154">更新 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="52c2e-154">Update **educationClass** object.</span></span>                                                         |
| [<span data-ttu-id="52c2e-155">删除</span><span class="sxs-lookup"><span data-stu-id="52c2e-155">Delete</span></span>](../api/educationclass-delete.md)                               | <span data-ttu-id="52c2e-156">无</span><span class="sxs-lookup"><span data-stu-id="52c2e-156">None</span></span>                                           | <span data-ttu-id="52c2e-157">删除 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="52c2e-157">Delete **educationClass** object.</span></span>                                                         |
| [<span data-ttu-id="52c2e-158">Delta</span><span class="sxs-lookup"><span data-stu-id="52c2e-158">Delta</span></span>](../api/educationclass-delta.md)                                 | <span data-ttu-id="52c2e-159">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="52c2e-159">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="52c2e-160">获取**educationClasses**的增量更改</span><span class="sxs-lookup"><span data-stu-id="52c2e-160">Get incremental changes for **educationClasses**</span></span>                                          |

## <a name="properties"></a><span data-ttu-id="52c2e-161">属性</span><span class="sxs-lookup"><span data-stu-id="52c2e-161">Properties</span></span>

| <span data-ttu-id="52c2e-162">属性</span><span class="sxs-lookup"><span data-stu-id="52c2e-162">Property</span></span>       | <span data-ttu-id="52c2e-163">类型</span><span class="sxs-lookup"><span data-stu-id="52c2e-163">Type</span></span>                                  | <span data-ttu-id="52c2e-164">说明</span><span class="sxs-lookup"><span data-stu-id="52c2e-164">Description</span></span>                                                                             |
| :------------- | :------------------------------------ | :-------------------------------------------------------------------------------------- |
| <span data-ttu-id="52c2e-165">id</span><span class="sxs-lookup"><span data-stu-id="52c2e-165">id</span></span>             | <span data-ttu-id="52c2e-166">字符串</span><span class="sxs-lookup"><span data-stu-id="52c2e-166">String</span></span>                                | <span data-ttu-id="52c2e-167">课程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="52c2e-167">Unique identifier for the class.</span></span>                                                        |
| <span data-ttu-id="52c2e-168">classCode</span><span class="sxs-lookup"><span data-stu-id="52c2e-168">classCode</span></span>      | <span data-ttu-id="52c2e-169">String</span><span class="sxs-lookup"><span data-stu-id="52c2e-169">String</span></span>                                | <span data-ttu-id="52c2e-170">学校用于标识课程的课程代码。</span><span class="sxs-lookup"><span data-stu-id="52c2e-170">Class code used by the school to identify the class.</span></span>                                    |
| <span data-ttu-id="52c2e-171">采取</span><span class="sxs-lookup"><span data-stu-id="52c2e-171">course</span></span>         | [<span data-ttu-id="52c2e-172">educationCourse</span><span class="sxs-lookup"><span data-stu-id="52c2e-172">educationCourse</span></span>](educationcourse.md) | <span data-ttu-id="52c2e-173">课堂课程信息</span><span class="sxs-lookup"><span data-stu-id="52c2e-173">Course information for the class</span></span>                                                        |
| <span data-ttu-id="52c2e-174">createdBy</span><span class="sxs-lookup"><span data-stu-id="52c2e-174">createdBy</span></span>      | <span data-ttu-id="52c2e-175">[identitySet]</span><span class="sxs-lookup"><span data-stu-id="52c2e-175">[identitySet]</span></span>                         | <span data-ttu-id="52c2e-176">创建了课程的实体</span><span class="sxs-lookup"><span data-stu-id="52c2e-176">Entity who created the class</span></span>                                                            |
| <span data-ttu-id="52c2e-177">说明</span><span class="sxs-lookup"><span data-stu-id="52c2e-177">description</span></span>    | <span data-ttu-id="52c2e-178">String</span><span class="sxs-lookup"><span data-stu-id="52c2e-178">String</span></span>                                | <span data-ttu-id="52c2e-179">课程说明。</span><span class="sxs-lookup"><span data-stu-id="52c2e-179">Description of the class.</span></span>                                                               |
| <span data-ttu-id="52c2e-180">displayName</span><span class="sxs-lookup"><span data-stu-id="52c2e-180">displayName</span></span>    | <span data-ttu-id="52c2e-181">String</span><span class="sxs-lookup"><span data-stu-id="52c2e-181">String</span></span>                                | <span data-ttu-id="52c2e-182">课程名称。</span><span class="sxs-lookup"><span data-stu-id="52c2e-182">Name of the class.</span></span>                                                                      |
| <span data-ttu-id="52c2e-183">externalId</span><span class="sxs-lookup"><span data-stu-id="52c2e-183">externalId</span></span>     | <span data-ttu-id="52c2e-184">String</span><span class="sxs-lookup"><span data-stu-id="52c2e-184">String</span></span>                                | <span data-ttu-id="52c2e-185">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="52c2e-185">ID of the class from the syncing system.</span></span>                                                |
| <span data-ttu-id="52c2e-186">externalName</span><span class="sxs-lookup"><span data-stu-id="52c2e-186">externalName</span></span>   | <span data-ttu-id="52c2e-187">String</span><span class="sxs-lookup"><span data-stu-id="52c2e-187">String</span></span>                                | <span data-ttu-id="52c2e-188">同步系统中的课程名称。</span><span class="sxs-lookup"><span data-stu-id="52c2e-188">Name of the class in the syncing system.</span></span>                                                |
| <span data-ttu-id="52c2e-189">externalSource</span><span class="sxs-lookup"><span data-stu-id="52c2e-189">externalSource</span></span> | <span data-ttu-id="52c2e-190">string</span><span class="sxs-lookup"><span data-stu-id="52c2e-190">string</span></span>                                | <span data-ttu-id="52c2e-191">此课程的创建方式。</span><span class="sxs-lookup"><span data-stu-id="52c2e-191">How this class was created.</span></span> <span data-ttu-id="52c2e-192">可取值为：`sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="52c2e-192">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span> |
| <span data-ttu-id="52c2e-193">mailNickname</span><span class="sxs-lookup"><span data-stu-id="52c2e-193">mailNickname</span></span>   | <span data-ttu-id="52c2e-194">字符串</span><span class="sxs-lookup"><span data-stu-id="52c2e-194">String</span></span>                                | <span data-ttu-id="52c2e-195">向所有成员发送电子邮件的邮件名称（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="52c2e-195">Mail name for sending email to all members, if this is enabled.</span></span>                         |
| <span data-ttu-id="52c2e-196">term</span><span class="sxs-lookup"><span data-stu-id="52c2e-196">term</span></span>           | <span data-ttu-id="52c2e-197">[educationTerm]</span><span class="sxs-lookup"><span data-stu-id="52c2e-197">[educationTerm]</span></span>                       | <span data-ttu-id="52c2e-198">类的术语。</span><span class="sxs-lookup"><span data-stu-id="52c2e-198">Term for the class.</span></span>                                                                     |

## <a name="relationships"></a><span data-ttu-id="52c2e-199">关系</span><span class="sxs-lookup"><span data-stu-id="52c2e-199">Relationships</span></span>

| <span data-ttu-id="52c2e-200">关系</span><span class="sxs-lookup"><span data-stu-id="52c2e-200">Relationship</span></span> | <span data-ttu-id="52c2e-201">类型</span><span class="sxs-lookup"><span data-stu-id="52c2e-201">Type</span></span>                             | <span data-ttu-id="52c2e-202">说明</span><span class="sxs-lookup"><span data-stu-id="52c2e-202">Description</span></span>                                               |
| :----------- | :------------------------------- | :-------------------------------------------------------- |
| <span data-ttu-id="52c2e-203">assignments</span><span class="sxs-lookup"><span data-stu-id="52c2e-203">assignments</span></span>  | <span data-ttu-id="52c2e-204">[educationAssignment]集合</span><span class="sxs-lookup"><span data-stu-id="52c2e-204">[educationAssignment] collection</span></span> | <span data-ttu-id="52c2e-205">与此类关联的所有工作分配。</span><span class="sxs-lookup"><span data-stu-id="52c2e-205">All assignments associated with this class.</span></span> <span data-ttu-id="52c2e-206">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="52c2e-206">Nullable.</span></span>     |
| <span data-ttu-id="52c2e-207">members</span><span class="sxs-lookup"><span data-stu-id="52c2e-207">members</span></span>      | <span data-ttu-id="52c2e-208">[educationUser] 集合</span><span class="sxs-lookup"><span data-stu-id="52c2e-208">[educationUser] collection</span></span>       | <span data-ttu-id="52c2e-209">课程中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="52c2e-209">All users in the class.</span></span> <span data-ttu-id="52c2e-210">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="52c2e-210">Nullable.</span></span>                         |
| <span data-ttu-id="52c2e-211">schools</span><span class="sxs-lookup"><span data-stu-id="52c2e-211">schools</span></span>      | <span data-ttu-id="52c2e-212">[educationSchool] 集合</span><span class="sxs-lookup"><span data-stu-id="52c2e-212">[educationSchool] collection</span></span>     | <span data-ttu-id="52c2e-213">与此课程相关的所有学校。</span><span class="sxs-lookup"><span data-stu-id="52c2e-213">All schools that this class is associated with.</span></span> <span data-ttu-id="52c2e-214">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="52c2e-214">Nullable.</span></span> |
| <span data-ttu-id="52c2e-215">teachers</span><span class="sxs-lookup"><span data-stu-id="52c2e-215">teachers</span></span>     | <span data-ttu-id="52c2e-216">[educationUser] 集合</span><span class="sxs-lookup"><span data-stu-id="52c2e-216">[educationUser] collection</span></span>       | <span data-ttu-id="52c2e-217">课程中的所有教师。</span><span class="sxs-lookup"><span data-stu-id="52c2e-217">All teachers in the class.</span></span> <span data-ttu-id="52c2e-218">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="52c2e-218">Nullable.</span></span>                      |

## <a name="json-representation"></a><span data-ttu-id="52c2e-219">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52c2e-219">JSON representation</span></span>

<span data-ttu-id="52c2e-220">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52c2e-220">The following is a JSON representation of the resource.</span></span>

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
