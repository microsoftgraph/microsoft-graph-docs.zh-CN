---
title: educationClass 资源类型
description: '表示学校的课程。 **educationClass** 资源对应于 Office 365 组并共享同一个 ID。 学生是课程的正式成员，教师为所有者，且具有相应权限。 若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。  '
localization_priority: Normal
ms.openlocfilehash: 97cf3b63cfb25a4c50df03c9c10212bd774c8b61
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831842"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="0388e-106">educationClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="0388e-106">educationClass resource type</span></span>

<span data-ttu-id="0388e-107">表示学校的课程。</span><span class="sxs-lookup"><span data-stu-id="0388e-107">Represents a class within a school.</span></span> <span data-ttu-id="0388e-108">**educationClass** 资源对应于 Office 365 组并共享同一个 ID。</span><span class="sxs-lookup"><span data-stu-id="0388e-108">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="0388e-109">学生是课程的正式成员，教师为所有者，且具有相应权限。</span><span class="sxs-lookup"><span data-stu-id="0388e-109">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="0388e-110">若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。</span><span class="sxs-lookup"><span data-stu-id="0388e-110">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="0388e-111">方法</span><span class="sxs-lookup"><span data-stu-id="0388e-111">Methods</span></span>

| <span data-ttu-id="0388e-112">方法</span><span class="sxs-lookup"><span data-stu-id="0388e-112">Method</span></span>           | <span data-ttu-id="0388e-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="0388e-113">Return Type</span></span>    |<span data-ttu-id="0388e-114">说明</span><span class="sxs-lookup"><span data-stu-id="0388e-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0388e-115">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="0388e-115">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="0388e-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="0388e-116">educationClass</span></span>](educationclass.md) |<span data-ttu-id="0388e-117">读取 **educationClass** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0388e-117">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="0388e-118">Add member</span><span class="sxs-lookup"><span data-stu-id="0388e-118">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="0388e-119">educationUser</span><span class="sxs-lookup"><span data-stu-id="0388e-119">educationUser</span></span>](educationuser.md)| <span data-ttu-id="0388e-120">通过发布到 members 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="0388e-120">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="0388e-121">List members</span><span class="sxs-lookup"><span data-stu-id="0388e-121">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="0388e-122">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0388e-122">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="0388e-123">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0388e-123">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="0388e-124">Remove student</span><span class="sxs-lookup"><span data-stu-id="0388e-124">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="0388e-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="0388e-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="0388e-126">通过成员导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="0388e-126">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="0388e-127">List schools</span><span class="sxs-lookup"><span data-stu-id="0388e-127">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="0388e-128">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0388e-128">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="0388e-129">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0388e-129">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="0388e-130">Add teacher</span><span class="sxs-lookup"><span data-stu-id="0388e-130">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="0388e-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="0388e-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="0388e-132">通过发布到 teachers 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="0388e-132">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="0388e-133">List teachers</span><span class="sxs-lookup"><span data-stu-id="0388e-133">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="0388e-134">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0388e-134">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="0388e-135">获取课程的教师列表。</span><span class="sxs-lookup"><span data-stu-id="0388e-135">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="0388e-136">Remove teacher</span><span class="sxs-lookup"><span data-stu-id="0388e-136">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="0388e-137">educationUser</span><span class="sxs-lookup"><span data-stu-id="0388e-137">educationUser</span></span>](educationuser.md)| <span data-ttu-id="0388e-138">通过教师导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="0388e-138">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="0388e-139">Get group</span><span class="sxs-lookup"><span data-stu-id="0388e-139">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="0388e-140">group</span><span class="sxs-lookup"><span data-stu-id="0388e-140">group</span></span>](group.md)| <span data-ttu-id="0388e-141">获得与此 **educationClass** 对应的 Office 365 **group**。</span><span class="sxs-lookup"><span data-stu-id="0388e-141">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="0388e-142">Update</span><span class="sxs-lookup"><span data-stu-id="0388e-142">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="0388e-143">educationClass</span><span class="sxs-lookup"><span data-stu-id="0388e-143">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="0388e-144">更新 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="0388e-144">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="0388e-145">Delete</span><span class="sxs-lookup"><span data-stu-id="0388e-145">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="0388e-146">无</span><span class="sxs-lookup"><span data-stu-id="0388e-146">None</span></span> |<span data-ttu-id="0388e-147">删除 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="0388e-147">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0388e-148">属性</span><span class="sxs-lookup"><span data-stu-id="0388e-148">Properties</span></span>
| <span data-ttu-id="0388e-149">属性</span><span class="sxs-lookup"><span data-stu-id="0388e-149">Property</span></span>     | <span data-ttu-id="0388e-150">类型</span><span class="sxs-lookup"><span data-stu-id="0388e-150">Type</span></span>   |<span data-ttu-id="0388e-151">说明</span><span class="sxs-lookup"><span data-stu-id="0388e-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0388e-152">id</span><span class="sxs-lookup"><span data-stu-id="0388e-152">id</span></span>| <span data-ttu-id="0388e-153">String</span><span class="sxs-lookup"><span data-stu-id="0388e-153">String</span></span>| <span data-ttu-id="0388e-154">课程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0388e-154">Unique identifier for the class.</span></span>|
|<span data-ttu-id="0388e-155">description</span><span class="sxs-lookup"><span data-stu-id="0388e-155">description</span></span>|<span data-ttu-id="0388e-156">String</span><span class="sxs-lookup"><span data-stu-id="0388e-156">String</span></span>| <span data-ttu-id="0388e-157">课程说明。</span><span class="sxs-lookup"><span data-stu-id="0388e-157">Description of the class.</span></span>|
|<span data-ttu-id="0388e-158">displayName</span><span class="sxs-lookup"><span data-stu-id="0388e-158">displayName</span></span>|<span data-ttu-id="0388e-159">String</span><span class="sxs-lookup"><span data-stu-id="0388e-159">String</span></span>| <span data-ttu-id="0388e-160">课程名称。</span><span class="sxs-lookup"><span data-stu-id="0388e-160">Name of the class.</span></span>|
|<span data-ttu-id="0388e-161">mailNickname</span><span class="sxs-lookup"><span data-stu-id="0388e-161">mailNickname</span></span>|<span data-ttu-id="0388e-162">String</span><span class="sxs-lookup"><span data-stu-id="0388e-162">String</span></span>| <span data-ttu-id="0388e-163">向所有成员发送电子邮件的邮件名称（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="0388e-163">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="0388e-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="0388e-164">createdBy</span></span>|[<span data-ttu-id="0388e-165">identitySet</span><span class="sxs-lookup"><span data-stu-id="0388e-165">identitySet</span></span>](identityset.md)| <span data-ttu-id="0388e-166">创建了课程的实体</span><span class="sxs-lookup"><span data-stu-id="0388e-166">Entity who created the class</span></span> |
|<span data-ttu-id="0388e-167">classCode</span><span class="sxs-lookup"><span data-stu-id="0388e-167">classCode</span></span>|<span data-ttu-id="0388e-168">String</span><span class="sxs-lookup"><span data-stu-id="0388e-168">String</span></span>| <span data-ttu-id="0388e-169">学校用于标识课程的课程代码。</span><span class="sxs-lookup"><span data-stu-id="0388e-169">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="0388e-170">externalId</span><span class="sxs-lookup"><span data-stu-id="0388e-170">externalId</span></span>|<span data-ttu-id="0388e-171">String</span><span class="sxs-lookup"><span data-stu-id="0388e-171">String</span></span>| <span data-ttu-id="0388e-172">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="0388e-172">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="0388e-173">externalName</span><span class="sxs-lookup"><span data-stu-id="0388e-173">externalName</span></span>|<span data-ttu-id="0388e-174">String</span><span class="sxs-lookup"><span data-stu-id="0388e-174">String</span></span>|<span data-ttu-id="0388e-175">同步系统中的课程名称。</span><span class="sxs-lookup"><span data-stu-id="0388e-175">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="0388e-176">externalSource</span><span class="sxs-lookup"><span data-stu-id="0388e-176">externalSource</span></span>|<span data-ttu-id="0388e-177">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="0388e-177">educationExternalSource</span></span>| <span data-ttu-id="0388e-178">此课程的创建方式。</span><span class="sxs-lookup"><span data-stu-id="0388e-178">How this class was created.</span></span> <span data-ttu-id="0388e-179">可能的值为： `sis`， `manual`， `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0388e-179">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0388e-180">term</span><span class="sxs-lookup"><span data-stu-id="0388e-180">term</span></span>|[<span data-ttu-id="0388e-181">educationTerm</span><span class="sxs-lookup"><span data-stu-id="0388e-181">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="0388e-182">此课程的学期。</span><span class="sxs-lookup"><span data-stu-id="0388e-182">Term for this class.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0388e-183">关系</span><span class="sxs-lookup"><span data-stu-id="0388e-183">Relationships</span></span>
| <span data-ttu-id="0388e-184">关系</span><span class="sxs-lookup"><span data-stu-id="0388e-184">Relationship</span></span> | <span data-ttu-id="0388e-185">类型</span><span class="sxs-lookup"><span data-stu-id="0388e-185">Type</span></span>   |<span data-ttu-id="0388e-186">说明</span><span class="sxs-lookup"><span data-stu-id="0388e-186">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0388e-187">members</span><span class="sxs-lookup"><span data-stu-id="0388e-187">members</span></span>|<span data-ttu-id="0388e-188">[educationUser](../resources/educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0388e-188">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="0388e-189">课程中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="0388e-189">All users in the class.</span></span> <span data-ttu-id="0388e-190">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="0388e-190">Nullable.</span></span>|
|<span data-ttu-id="0388e-191">schools</span><span class="sxs-lookup"><span data-stu-id="0388e-191">schools</span></span>|<span data-ttu-id="0388e-192">[educationSchool](../resources/educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0388e-192">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="0388e-193">与此课程相关的所有学校。</span><span class="sxs-lookup"><span data-stu-id="0388e-193">All schools that this class is associated with.</span></span> <span data-ttu-id="0388e-194">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="0388e-194">Nullable.</span></span>|
|<span data-ttu-id="0388e-195">teachers</span><span class="sxs-lookup"><span data-stu-id="0388e-195">teachers</span></span>|<span data-ttu-id="0388e-196">[educationUser](../resources/educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0388e-196">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="0388e-197">课程中的所有教师。</span><span class="sxs-lookup"><span data-stu-id="0388e-197">All teachers in the class.</span></span> <span data-ttu-id="0388e-198">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="0388e-198">Nullable.</span></span>|
|<span data-ttu-id="0388e-199">group</span><span class="sxs-lookup"><span data-stu-id="0388e-199">group</span></span>|[<span data-ttu-id="0388e-200">组</span><span class="sxs-lookup"><span data-stu-id="0388e-200">group</span></span>](../resources/group.md)| <span data-ttu-id="0388e-201">对应于此类 directory 组。</span><span class="sxs-lookup"><span data-stu-id="0388e-201">The directory group corresponding to this class.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0388e-202">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0388e-202">JSON representation</span></span>

<span data-ttu-id="0388e-203">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0388e-203">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
