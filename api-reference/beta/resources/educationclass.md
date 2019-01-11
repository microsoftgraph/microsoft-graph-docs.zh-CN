---
title: educationClass 资源类型
description: '表示学校的课程。 **educationClass** 资源对应于 Office 365 组并共享同一个 ID。 学生是课程的正式成员，教师为所有者，且具有相应权限。 若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。  '
localization_priority: Normal
ms.openlocfilehash: 1c657a1eba131a9bcfa8dd4f84e2ba2141a4750a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866785"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="78f55-106">educationClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="78f55-106">educationClass resource type</span></span>

> <span data-ttu-id="78f55-107">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="78f55-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78f55-108">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="78f55-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78f55-109">表示学校的课程。</span><span class="sxs-lookup"><span data-stu-id="78f55-109">Represents a class within a school.</span></span> <span data-ttu-id="78f55-110">**educationClass** 资源对应于 Office 365 组并共享同一个 ID。</span><span class="sxs-lookup"><span data-stu-id="78f55-110">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="78f55-111">学生是课程的正式成员，教师为所有者，且具有相应权限。</span><span class="sxs-lookup"><span data-stu-id="78f55-111">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="78f55-112">若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。</span><span class="sxs-lookup"><span data-stu-id="78f55-112">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="78f55-113">方法</span><span class="sxs-lookup"><span data-stu-id="78f55-113">Methods</span></span>

| <span data-ttu-id="78f55-114">方法</span><span class="sxs-lookup"><span data-stu-id="78f55-114">Method</span></span>           | <span data-ttu-id="78f55-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="78f55-115">Return Type</span></span>    |<span data-ttu-id="78f55-116">说明</span><span class="sxs-lookup"><span data-stu-id="78f55-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="78f55-117">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="78f55-117">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="78f55-118">educationClass</span><span class="sxs-lookup"><span data-stu-id="78f55-118">educationClass</span></span>](educationclass.md) |<span data-ttu-id="78f55-119">读取 **educationClass** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="78f55-119">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="78f55-120">Add member</span><span class="sxs-lookup"><span data-stu-id="78f55-120">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="78f55-121">educationUser</span><span class="sxs-lookup"><span data-stu-id="78f55-121">educationUser</span></span>](educationuser.md)| <span data-ttu-id="78f55-122">通过发布到 members 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="78f55-122">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="78f55-123">List members</span><span class="sxs-lookup"><span data-stu-id="78f55-123">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="78f55-124">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="78f55-124">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="78f55-125">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="78f55-125">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="78f55-126">Remove student</span><span class="sxs-lookup"><span data-stu-id="78f55-126">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="78f55-127">educationUser</span><span class="sxs-lookup"><span data-stu-id="78f55-127">educationUser</span></span>](educationuser.md)| <span data-ttu-id="78f55-128">通过成员导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="78f55-128">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="78f55-129">List schools</span><span class="sxs-lookup"><span data-stu-id="78f55-129">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="78f55-130">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="78f55-130">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="78f55-131">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="78f55-131">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="78f55-132">Add teacher</span><span class="sxs-lookup"><span data-stu-id="78f55-132">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="78f55-133">educationUser</span><span class="sxs-lookup"><span data-stu-id="78f55-133">educationUser</span></span>](educationuser.md)| <span data-ttu-id="78f55-134">通过发布到 teachers 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="78f55-134">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="78f55-135">List teachers</span><span class="sxs-lookup"><span data-stu-id="78f55-135">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="78f55-136">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="78f55-136">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="78f55-137">获取课程的教师列表。</span><span class="sxs-lookup"><span data-stu-id="78f55-137">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="78f55-138">Remove teacher</span><span class="sxs-lookup"><span data-stu-id="78f55-138">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="78f55-139">educationUser</span><span class="sxs-lookup"><span data-stu-id="78f55-139">educationUser</span></span>](educationuser.md)| <span data-ttu-id="78f55-140">通过教师导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="78f55-140">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="78f55-141">创建 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="78f55-141">Create educationAssignment</span></span>](../api/educationclass-post-assignments.md) |[<span data-ttu-id="78f55-142">educationAssignment</span><span class="sxs-lookup"><span data-stu-id="78f55-142">educationAssignment</span></span>](../resources/educationassignment.md)| <span data-ttu-id="78f55-143">通过发布到 assignments 集合中创建新**educationAssignment** 。</span><span class="sxs-lookup"><span data-stu-id="78f55-143">Create a new **educationAssignment** by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="78f55-144">列表分配</span><span class="sxs-lookup"><span data-stu-id="78f55-144">List assignments</span></span>](../api/educationclass-list-assignments.md) |<span data-ttu-id="78f55-145">[educationAssignment](../resources/educationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="78f55-145">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="78f55-146">获取**educationAssignment**对象集合。</span><span class="sxs-lookup"><span data-stu-id="78f55-146">Get an **educationAssignment** object collection.</span></span>|
|[<span data-ttu-id="78f55-147">获取组</span><span class="sxs-lookup"><span data-stu-id="78f55-147">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="78f55-148">group</span><span class="sxs-lookup"><span data-stu-id="78f55-148">group</span></span>](group.md)| <span data-ttu-id="78f55-149">获得与此 **educationClass** 对应的 Office 365 **group**。</span><span class="sxs-lookup"><span data-stu-id="78f55-149">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="78f55-150">Update</span><span class="sxs-lookup"><span data-stu-id="78f55-150">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="78f55-151">educationClass</span><span class="sxs-lookup"><span data-stu-id="78f55-151">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="78f55-152">更新 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="78f55-152">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="78f55-153">Delete</span><span class="sxs-lookup"><span data-stu-id="78f55-153">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="78f55-154">无</span><span class="sxs-lookup"><span data-stu-id="78f55-154">None</span></span> |<span data-ttu-id="78f55-155">删除 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="78f55-155">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="78f55-156">属性</span><span class="sxs-lookup"><span data-stu-id="78f55-156">Properties</span></span>
| <span data-ttu-id="78f55-157">属性</span><span class="sxs-lookup"><span data-stu-id="78f55-157">Property</span></span>     | <span data-ttu-id="78f55-158">类型</span><span class="sxs-lookup"><span data-stu-id="78f55-158">Type</span></span>   |<span data-ttu-id="78f55-159">说明</span><span class="sxs-lookup"><span data-stu-id="78f55-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78f55-160">id</span><span class="sxs-lookup"><span data-stu-id="78f55-160">id</span></span>| <span data-ttu-id="78f55-161">String</span><span class="sxs-lookup"><span data-stu-id="78f55-161">String</span></span>| <span data-ttu-id="78f55-162">课程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="78f55-162">Unique identifier for the class.</span></span>|
|<span data-ttu-id="78f55-163">description</span><span class="sxs-lookup"><span data-stu-id="78f55-163">description</span></span>|<span data-ttu-id="78f55-164">String</span><span class="sxs-lookup"><span data-stu-id="78f55-164">String</span></span>| <span data-ttu-id="78f55-165">课程说明。</span><span class="sxs-lookup"><span data-stu-id="78f55-165">Description of the class.</span></span>|
|<span data-ttu-id="78f55-166">displayName</span><span class="sxs-lookup"><span data-stu-id="78f55-166">displayName</span></span>|<span data-ttu-id="78f55-167">String</span><span class="sxs-lookup"><span data-stu-id="78f55-167">String</span></span>| <span data-ttu-id="78f55-168">课程名称。</span><span class="sxs-lookup"><span data-stu-id="78f55-168">Name of the class.</span></span>|
|<span data-ttu-id="78f55-169">mailNickname</span><span class="sxs-lookup"><span data-stu-id="78f55-169">mailNickname</span></span>|<span data-ttu-id="78f55-170">String</span><span class="sxs-lookup"><span data-stu-id="78f55-170">String</span></span>| <span data-ttu-id="78f55-171">向所有成员发送电子邮件的邮件名称（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="78f55-171">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="78f55-172">createdBy</span><span class="sxs-lookup"><span data-stu-id="78f55-172">createdBy</span></span>|[<span data-ttu-id="78f55-173">identitySet</span><span class="sxs-lookup"><span data-stu-id="78f55-173">identitySet</span></span>](identityset.md)| <span data-ttu-id="78f55-174">创建了课程的实体</span><span class="sxs-lookup"><span data-stu-id="78f55-174">Entity who created the class</span></span> |
|<span data-ttu-id="78f55-175">classCode</span><span class="sxs-lookup"><span data-stu-id="78f55-175">classCode</span></span>|<span data-ttu-id="78f55-176">String</span><span class="sxs-lookup"><span data-stu-id="78f55-176">String</span></span>| <span data-ttu-id="78f55-177">学校用于标识课程的课程代码。</span><span class="sxs-lookup"><span data-stu-id="78f55-177">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="78f55-178">externalId</span><span class="sxs-lookup"><span data-stu-id="78f55-178">externalId</span></span>|<span data-ttu-id="78f55-179">String</span><span class="sxs-lookup"><span data-stu-id="78f55-179">String</span></span>| <span data-ttu-id="78f55-180">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="78f55-180">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="78f55-181">externalName</span><span class="sxs-lookup"><span data-stu-id="78f55-181">externalName</span></span>|<span data-ttu-id="78f55-182">String</span><span class="sxs-lookup"><span data-stu-id="78f55-182">String</span></span>|<span data-ttu-id="78f55-183">同步系统中的课程名称。</span><span class="sxs-lookup"><span data-stu-id="78f55-183">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="78f55-184">externalSource</span><span class="sxs-lookup"><span data-stu-id="78f55-184">externalSource</span></span>|<span data-ttu-id="78f55-185">string</span><span class="sxs-lookup"><span data-stu-id="78f55-185">string</span></span>| <span data-ttu-id="78f55-186">此课程的创建方式。</span><span class="sxs-lookup"><span data-stu-id="78f55-186">How this class was created.</span></span> <span data-ttu-id="78f55-187">可取值为：`sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="78f55-187">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="78f55-188">term</span><span class="sxs-lookup"><span data-stu-id="78f55-188">term</span></span>|[<span data-ttu-id="78f55-189">educationTerm</span><span class="sxs-lookup"><span data-stu-id="78f55-189">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="78f55-190">此课程的学期。</span><span class="sxs-lookup"><span data-stu-id="78f55-190">Term for this class.</span></span>|


## <a name="relationships"></a><span data-ttu-id="78f55-191">关系</span><span class="sxs-lookup"><span data-stu-id="78f55-191">Relationships</span></span>
| <span data-ttu-id="78f55-192">关系</span><span class="sxs-lookup"><span data-stu-id="78f55-192">Relationship</span></span> | <span data-ttu-id="78f55-193">类型</span><span class="sxs-lookup"><span data-stu-id="78f55-193">Type</span></span>   |<span data-ttu-id="78f55-194">说明</span><span class="sxs-lookup"><span data-stu-id="78f55-194">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78f55-195">members</span><span class="sxs-lookup"><span data-stu-id="78f55-195">members</span></span>|<span data-ttu-id="78f55-196">[educationUser](../resources/educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="78f55-196">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="78f55-197">课程中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="78f55-197">All users in the class.</span></span> <span data-ttu-id="78f55-198">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="78f55-198">Nullable.</span></span>|
|<span data-ttu-id="78f55-199">schools</span><span class="sxs-lookup"><span data-stu-id="78f55-199">schools</span></span>|<span data-ttu-id="78f55-200">[educationSchool](../resources/educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="78f55-200">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="78f55-201">与此课程相关的所有学校。</span><span class="sxs-lookup"><span data-stu-id="78f55-201">All schools that this class is associated with.</span></span> <span data-ttu-id="78f55-202">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="78f55-202">Nullable.</span></span>|
|<span data-ttu-id="78f55-203">teachers</span><span class="sxs-lookup"><span data-stu-id="78f55-203">teachers</span></span>|<span data-ttu-id="78f55-204">[educationUser](../resources/educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="78f55-204">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="78f55-205">课程中的所有教师。</span><span class="sxs-lookup"><span data-stu-id="78f55-205">All teachers in the class.</span></span> <span data-ttu-id="78f55-206">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="78f55-206">Nullable.</span></span>|
|<span data-ttu-id="78f55-207">assignments</span><span class="sxs-lookup"><span data-stu-id="78f55-207">assignments</span></span>|<span data-ttu-id="78f55-208">[educationAssignment](../resources/educationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="78f55-208">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="78f55-209">与此类关联的所有工作分配。</span><span class="sxs-lookup"><span data-stu-id="78f55-209">All assignments associated with this class.</span></span> <span data-ttu-id="78f55-210">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="78f55-210">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="78f55-211">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78f55-211">JSON representation</span></span>

<span data-ttu-id="78f55-212">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78f55-212">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
  "term": {"@odata.type": "microsoft.graph.education.term"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
