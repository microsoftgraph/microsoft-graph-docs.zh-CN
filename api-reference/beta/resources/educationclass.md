---
title: educationClass 资源类型
description: '表示学校的课程。 **educationClass** 资源对应于 Office 365 组并共享同一个 ID。 学生是课程的正式成员，教师为所有者，且具有相应权限。 若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 5a4bbc0560f2a40b5a438ec8276bbcf984a22721
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526730"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="df466-106">educationClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="df466-106">educationClass resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df466-107">表示学校的课程。</span><span class="sxs-lookup"><span data-stu-id="df466-107">Represents a class within a school.</span></span> <span data-ttu-id="df466-108">**educationClass** 资源对应于 Office 365 组并共享同一个 ID。</span><span class="sxs-lookup"><span data-stu-id="df466-108">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="df466-109">学生是课程的正式成员，教师为所有者，且具有相应权限。</span><span class="sxs-lookup"><span data-stu-id="df466-109">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="df466-110">若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。</span><span class="sxs-lookup"><span data-stu-id="df466-110">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="df466-111">方法</span><span class="sxs-lookup"><span data-stu-id="df466-111">Methods</span></span>

| <span data-ttu-id="df466-112">方法</span><span class="sxs-lookup"><span data-stu-id="df466-112">Method</span></span>           | <span data-ttu-id="df466-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="df466-113">Return Type</span></span>    |<span data-ttu-id="df466-114">说明</span><span class="sxs-lookup"><span data-stu-id="df466-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="df466-115">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="df466-115">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="df466-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="df466-116">educationClass</span></span>](educationclass.md) |<span data-ttu-id="df466-117">读取 **educationClass** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="df466-117">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="df466-118">Add member</span><span class="sxs-lookup"><span data-stu-id="df466-118">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="df466-119">educationUser</span><span class="sxs-lookup"><span data-stu-id="df466-119">educationUser</span></span>](educationuser.md)| <span data-ttu-id="df466-120">通过发布到 members 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="df466-120">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="df466-121">List members</span><span class="sxs-lookup"><span data-stu-id="df466-121">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="df466-122">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="df466-122">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="df466-123">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="df466-123">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="df466-124">Remove student</span><span class="sxs-lookup"><span data-stu-id="df466-124">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="df466-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="df466-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="df466-126">通过成员导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="df466-126">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="df466-127">List schools</span><span class="sxs-lookup"><span data-stu-id="df466-127">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="df466-128">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="df466-128">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="df466-129">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="df466-129">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="df466-130">Add teacher</span><span class="sxs-lookup"><span data-stu-id="df466-130">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="df466-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="df466-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="df466-132">通过发布到 teachers 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="df466-132">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="df466-133">List teachers</span><span class="sxs-lookup"><span data-stu-id="df466-133">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="df466-134">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="df466-134">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="df466-135">获取课程的教师列表。</span><span class="sxs-lookup"><span data-stu-id="df466-135">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="df466-136">Remove teacher</span><span class="sxs-lookup"><span data-stu-id="df466-136">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="df466-137">educationUser</span><span class="sxs-lookup"><span data-stu-id="df466-137">educationUser</span></span>](educationuser.md)| <span data-ttu-id="df466-138">通过教师导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="df466-138">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="df466-139">创建 educationAssignment</span><span class="sxs-lookup"><span data-stu-id="df466-139">Create educationAssignment</span></span>](../api/educationclass-post-assignments.md) |[<span data-ttu-id="df466-140">educationAssignment</span><span class="sxs-lookup"><span data-stu-id="df466-140">educationAssignment</span></span>](../resources/educationassignment.md)| <span data-ttu-id="df466-141">通过发布到 assignments 集合中创建新**educationAssignment** 。</span><span class="sxs-lookup"><span data-stu-id="df466-141">Create a new **educationAssignment** by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="df466-142">列表分配</span><span class="sxs-lookup"><span data-stu-id="df466-142">List assignments</span></span>](../api/educationclass-list-assignments.md) |<span data-ttu-id="df466-143">[educationAssignment](../resources/educationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="df466-143">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="df466-144">获取**educationAssignment**对象集合。</span><span class="sxs-lookup"><span data-stu-id="df466-144">Get an **educationAssignment** object collection.</span></span>|
|[<span data-ttu-id="df466-145">Get group</span><span class="sxs-lookup"><span data-stu-id="df466-145">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="df466-146">group</span><span class="sxs-lookup"><span data-stu-id="df466-146">group</span></span>](group.md)| <span data-ttu-id="df466-147">获得与此 **educationClass** 对应的 Office 365 **group**。</span><span class="sxs-lookup"><span data-stu-id="df466-147">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="df466-148">Update</span><span class="sxs-lookup"><span data-stu-id="df466-148">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="df466-149">educationClass</span><span class="sxs-lookup"><span data-stu-id="df466-149">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="df466-150">更新 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="df466-150">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="df466-151">Delete</span><span class="sxs-lookup"><span data-stu-id="df466-151">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="df466-152">无</span><span class="sxs-lookup"><span data-stu-id="df466-152">None</span></span> |<span data-ttu-id="df466-153">删除 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="df466-153">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="df466-154">属性</span><span class="sxs-lookup"><span data-stu-id="df466-154">Properties</span></span>
| <span data-ttu-id="df466-155">属性</span><span class="sxs-lookup"><span data-stu-id="df466-155">Property</span></span>     | <span data-ttu-id="df466-156">类型</span><span class="sxs-lookup"><span data-stu-id="df466-156">Type</span></span>   |<span data-ttu-id="df466-157">说明</span><span class="sxs-lookup"><span data-stu-id="df466-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df466-158">id</span><span class="sxs-lookup"><span data-stu-id="df466-158">id</span></span>| <span data-ttu-id="df466-159">字串符号</span><span class="sxs-lookup"><span data-stu-id="df466-159">String</span></span>| <span data-ttu-id="df466-160">课程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="df466-160">Unique identifier for the class.</span></span>|
|<span data-ttu-id="df466-161">description</span><span class="sxs-lookup"><span data-stu-id="df466-161">description</span></span>|<span data-ttu-id="df466-162">字符串</span><span class="sxs-lookup"><span data-stu-id="df466-162">String</span></span>| <span data-ttu-id="df466-163">课程说明。</span><span class="sxs-lookup"><span data-stu-id="df466-163">Description of the class.</span></span>|
|<span data-ttu-id="df466-164">displayName</span><span class="sxs-lookup"><span data-stu-id="df466-164">displayName</span></span>|<span data-ttu-id="df466-165">String</span><span class="sxs-lookup"><span data-stu-id="df466-165">String</span></span>| <span data-ttu-id="df466-166">课程名称。</span><span class="sxs-lookup"><span data-stu-id="df466-166">Name of the class.</span></span>|
|<span data-ttu-id="df466-167">mailNickname</span><span class="sxs-lookup"><span data-stu-id="df466-167">mailNickname</span></span>|<span data-ttu-id="df466-168">String</span><span class="sxs-lookup"><span data-stu-id="df466-168">String</span></span>| <span data-ttu-id="df466-169">向所有成员发送电子邮件的邮件名称（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="df466-169">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="df466-170">createdBy</span><span class="sxs-lookup"><span data-stu-id="df466-170">createdBy</span></span>|[<span data-ttu-id="df466-171">identitySet</span><span class="sxs-lookup"><span data-stu-id="df466-171">identitySet</span></span>](identityset.md)| <span data-ttu-id="df466-172">创建了课程的实体</span><span class="sxs-lookup"><span data-stu-id="df466-172">Entity who created the class</span></span> |
|<span data-ttu-id="df466-173">classCode</span><span class="sxs-lookup"><span data-stu-id="df466-173">classCode</span></span>|<span data-ttu-id="df466-174">String</span><span class="sxs-lookup"><span data-stu-id="df466-174">String</span></span>| <span data-ttu-id="df466-175">学校用于标识课程的课程代码。</span><span class="sxs-lookup"><span data-stu-id="df466-175">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="df466-176">externalId</span><span class="sxs-lookup"><span data-stu-id="df466-176">externalId</span></span>|<span data-ttu-id="df466-177">String</span><span class="sxs-lookup"><span data-stu-id="df466-177">String</span></span>| <span data-ttu-id="df466-178">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="df466-178">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="df466-179">externalName</span><span class="sxs-lookup"><span data-stu-id="df466-179">externalName</span></span>|<span data-ttu-id="df466-180">String</span><span class="sxs-lookup"><span data-stu-id="df466-180">String</span></span>|<span data-ttu-id="df466-181">同步系统中的课程名称。</span><span class="sxs-lookup"><span data-stu-id="df466-181">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="df466-182">externalSource</span><span class="sxs-lookup"><span data-stu-id="df466-182">externalSource</span></span>|<span data-ttu-id="df466-183">string</span><span class="sxs-lookup"><span data-stu-id="df466-183">string</span></span>| <span data-ttu-id="df466-184">此课程的创建方式。</span><span class="sxs-lookup"><span data-stu-id="df466-184">How this class was created.</span></span> <span data-ttu-id="df466-185">可取值为：`sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="df466-185">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="df466-186">term</span><span class="sxs-lookup"><span data-stu-id="df466-186">term</span></span>|[<span data-ttu-id="df466-187">educationTerm</span><span class="sxs-lookup"><span data-stu-id="df466-187">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="df466-188">此课程的学期。</span><span class="sxs-lookup"><span data-stu-id="df466-188">Term for this class.</span></span>|


## <a name="relationships"></a><span data-ttu-id="df466-189">关系</span><span class="sxs-lookup"><span data-stu-id="df466-189">Relationships</span></span>
| <span data-ttu-id="df466-190">关系</span><span class="sxs-lookup"><span data-stu-id="df466-190">Relationship</span></span> | <span data-ttu-id="df466-191">类型</span><span class="sxs-lookup"><span data-stu-id="df466-191">Type</span></span>   |<span data-ttu-id="df466-192">说明</span><span class="sxs-lookup"><span data-stu-id="df466-192">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df466-193">members</span><span class="sxs-lookup"><span data-stu-id="df466-193">members</span></span>|<span data-ttu-id="df466-194">[educationUser](../resources/educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="df466-194">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="df466-195">课程中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="df466-195">All users in the class.</span></span> <span data-ttu-id="df466-196">可为空。</span><span class="sxs-lookup"><span data-stu-id="df466-196">Nullable.</span></span>|
|<span data-ttu-id="df466-197">schools</span><span class="sxs-lookup"><span data-stu-id="df466-197">schools</span></span>|<span data-ttu-id="df466-198">[educationSchool](../resources/educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="df466-198">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="df466-199">与此课程相关的所有学校。</span><span class="sxs-lookup"><span data-stu-id="df466-199">All schools that this class is associated with.</span></span> <span data-ttu-id="df466-200">可为空。</span><span class="sxs-lookup"><span data-stu-id="df466-200">Nullable.</span></span>|
|<span data-ttu-id="df466-201">teachers</span><span class="sxs-lookup"><span data-stu-id="df466-201">teachers</span></span>|<span data-ttu-id="df466-202">[educationUser](../resources/educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="df466-202">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="df466-203">课程中的所有教师。</span><span class="sxs-lookup"><span data-stu-id="df466-203">All teachers in the class.</span></span> <span data-ttu-id="df466-204">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="df466-204">Nullable.</span></span>|
|<span data-ttu-id="df466-205">assignments</span><span class="sxs-lookup"><span data-stu-id="df466-205">assignments</span></span>|<span data-ttu-id="df466-206">[educationAssignment](../resources/educationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="df466-206">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="df466-207">与此类关联的所有工作分配。</span><span class="sxs-lookup"><span data-stu-id="df466-207">All assignments associated with this class.</span></span> <span data-ttu-id="df466-208">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="df466-208">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="df466-209">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df466-209">JSON representation</span></span>

<span data-ttu-id="df466-210">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df466-210">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationclass.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
