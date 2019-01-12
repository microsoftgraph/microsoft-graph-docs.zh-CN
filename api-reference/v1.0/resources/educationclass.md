---
title: educationClass 资源类型
description: '表示学校的课程。 **educationClass** 资源对应于 Office 365 组并共享同一个 ID。 学生是课程的正式成员，教师为所有者，且具有相应权限。 若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: c5b145d12dd99293eef9c338ff840d5781c5ef3f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933986"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="898a3-106">educationClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="898a3-106">educationClass resource type</span></span>

<span data-ttu-id="898a3-107">表示学校的课程。</span><span class="sxs-lookup"><span data-stu-id="898a3-107">Represents a class within a school.</span></span> <span data-ttu-id="898a3-108">**educationClass** 资源对应于 Office 365 组并共享同一个 ID。</span><span class="sxs-lookup"><span data-stu-id="898a3-108">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="898a3-109">学生是课程的正式成员，教师为所有者，且具有相应权限。</span><span class="sxs-lookup"><span data-stu-id="898a3-109">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="898a3-110">若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。</span><span class="sxs-lookup"><span data-stu-id="898a3-110">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="898a3-111">方法</span><span class="sxs-lookup"><span data-stu-id="898a3-111">Methods</span></span>

| <span data-ttu-id="898a3-112">方法</span><span class="sxs-lookup"><span data-stu-id="898a3-112">Method</span></span>           | <span data-ttu-id="898a3-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="898a3-113">Return Type</span></span>    |<span data-ttu-id="898a3-114">说明</span><span class="sxs-lookup"><span data-stu-id="898a3-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="898a3-115">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="898a3-115">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="898a3-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="898a3-116">educationClass</span></span>](educationclass.md) |<span data-ttu-id="898a3-117">读取 **educationClass** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="898a3-117">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="898a3-118">Add member</span><span class="sxs-lookup"><span data-stu-id="898a3-118">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="898a3-119">educationUser</span><span class="sxs-lookup"><span data-stu-id="898a3-119">educationUser</span></span>](educationuser.md)| <span data-ttu-id="898a3-120">通过发布到 members 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="898a3-120">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="898a3-121">List members</span><span class="sxs-lookup"><span data-stu-id="898a3-121">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="898a3-122">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="898a3-122">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="898a3-123">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="898a3-123">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="898a3-124">Remove student</span><span class="sxs-lookup"><span data-stu-id="898a3-124">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="898a3-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="898a3-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="898a3-126">通过成员导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="898a3-126">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="898a3-127">List schools</span><span class="sxs-lookup"><span data-stu-id="898a3-127">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="898a3-128">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="898a3-128">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="898a3-129">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="898a3-129">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="898a3-130">Add teacher</span><span class="sxs-lookup"><span data-stu-id="898a3-130">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="898a3-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="898a3-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="898a3-132">通过发布到 teachers 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="898a3-132">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="898a3-133">List teachers</span><span class="sxs-lookup"><span data-stu-id="898a3-133">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="898a3-134">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="898a3-134">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="898a3-135">获取课程的教师列表。</span><span class="sxs-lookup"><span data-stu-id="898a3-135">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="898a3-136">Remove teacher</span><span class="sxs-lookup"><span data-stu-id="898a3-136">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="898a3-137">educationUser</span><span class="sxs-lookup"><span data-stu-id="898a3-137">educationUser</span></span>](educationuser.md)| <span data-ttu-id="898a3-138">通过教师导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="898a3-138">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="898a3-139">Get group</span><span class="sxs-lookup"><span data-stu-id="898a3-139">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="898a3-140">group</span><span class="sxs-lookup"><span data-stu-id="898a3-140">group</span></span>](group.md)| <span data-ttu-id="898a3-141">获得与此 **educationClass** 对应的 Office 365 **group**。</span><span class="sxs-lookup"><span data-stu-id="898a3-141">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="898a3-142">Update</span><span class="sxs-lookup"><span data-stu-id="898a3-142">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="898a3-143">educationClass</span><span class="sxs-lookup"><span data-stu-id="898a3-143">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="898a3-144">更新 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="898a3-144">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="898a3-145">Delete</span><span class="sxs-lookup"><span data-stu-id="898a3-145">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="898a3-146">无</span><span class="sxs-lookup"><span data-stu-id="898a3-146">None</span></span> |<span data-ttu-id="898a3-147">删除 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="898a3-147">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="898a3-148">属性</span><span class="sxs-lookup"><span data-stu-id="898a3-148">Properties</span></span>
| <span data-ttu-id="898a3-149">属性</span><span class="sxs-lookup"><span data-stu-id="898a3-149">Property</span></span>     | <span data-ttu-id="898a3-150">类型</span><span class="sxs-lookup"><span data-stu-id="898a3-150">Type</span></span>   |<span data-ttu-id="898a3-151">说明</span><span class="sxs-lookup"><span data-stu-id="898a3-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="898a3-152">id</span><span class="sxs-lookup"><span data-stu-id="898a3-152">id</span></span>| <span data-ttu-id="898a3-153">String</span><span class="sxs-lookup"><span data-stu-id="898a3-153">String</span></span>| <span data-ttu-id="898a3-154">课程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="898a3-154">Unique identifier for the class.</span></span>|
|<span data-ttu-id="898a3-155">description</span><span class="sxs-lookup"><span data-stu-id="898a3-155">description</span></span>|<span data-ttu-id="898a3-156">String</span><span class="sxs-lookup"><span data-stu-id="898a3-156">String</span></span>| <span data-ttu-id="898a3-157">课程说明。</span><span class="sxs-lookup"><span data-stu-id="898a3-157">Description of the class.</span></span>|
|<span data-ttu-id="898a3-158">displayName</span><span class="sxs-lookup"><span data-stu-id="898a3-158">displayName</span></span>|<span data-ttu-id="898a3-159">String</span><span class="sxs-lookup"><span data-stu-id="898a3-159">String</span></span>| <span data-ttu-id="898a3-160">课程名称。</span><span class="sxs-lookup"><span data-stu-id="898a3-160">Name of the class.</span></span>|
|<span data-ttu-id="898a3-161">mailNickname</span><span class="sxs-lookup"><span data-stu-id="898a3-161">mailNickname</span></span>|<span data-ttu-id="898a3-162">String</span><span class="sxs-lookup"><span data-stu-id="898a3-162">String</span></span>| <span data-ttu-id="898a3-163">向所有成员发送电子邮件的邮件名称（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="898a3-163">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="898a3-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="898a3-164">createdBy</span></span>|[<span data-ttu-id="898a3-165">identitySet</span><span class="sxs-lookup"><span data-stu-id="898a3-165">identitySet</span></span>](identityset.md)| <span data-ttu-id="898a3-166">创建了课程的实体</span><span class="sxs-lookup"><span data-stu-id="898a3-166">Entity who created the class</span></span> |
|<span data-ttu-id="898a3-167">classCode</span><span class="sxs-lookup"><span data-stu-id="898a3-167">classCode</span></span>|<span data-ttu-id="898a3-168">String</span><span class="sxs-lookup"><span data-stu-id="898a3-168">String</span></span>| <span data-ttu-id="898a3-169">学校用于标识课程的课程代码。</span><span class="sxs-lookup"><span data-stu-id="898a3-169">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="898a3-170">externalId</span><span class="sxs-lookup"><span data-stu-id="898a3-170">externalId</span></span>|<span data-ttu-id="898a3-171">String</span><span class="sxs-lookup"><span data-stu-id="898a3-171">String</span></span>| <span data-ttu-id="898a3-172">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="898a3-172">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="898a3-173">externalName</span><span class="sxs-lookup"><span data-stu-id="898a3-173">externalName</span></span>|<span data-ttu-id="898a3-174">String</span><span class="sxs-lookup"><span data-stu-id="898a3-174">String</span></span>|<span data-ttu-id="898a3-175">同步系统中的课程名称。</span><span class="sxs-lookup"><span data-stu-id="898a3-175">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="898a3-176">externalSource</span><span class="sxs-lookup"><span data-stu-id="898a3-176">externalSource</span></span>|<span data-ttu-id="898a3-177">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="898a3-177">educationExternalSource</span></span>| <span data-ttu-id="898a3-178">此课程的创建方式。</span><span class="sxs-lookup"><span data-stu-id="898a3-178">How this class was created.</span></span> <span data-ttu-id="898a3-179">可能的值为： `sis`， `manual`， `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="898a3-179">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="898a3-180">term</span><span class="sxs-lookup"><span data-stu-id="898a3-180">term</span></span>|[<span data-ttu-id="898a3-181">educationTerm</span><span class="sxs-lookup"><span data-stu-id="898a3-181">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="898a3-182">此课程的学期。</span><span class="sxs-lookup"><span data-stu-id="898a3-182">Term for this class.</span></span>|

## <a name="relationships"></a><span data-ttu-id="898a3-183">关系</span><span class="sxs-lookup"><span data-stu-id="898a3-183">Relationships</span></span>
| <span data-ttu-id="898a3-184">关系</span><span class="sxs-lookup"><span data-stu-id="898a3-184">Relationship</span></span> | <span data-ttu-id="898a3-185">类型</span><span class="sxs-lookup"><span data-stu-id="898a3-185">Type</span></span>   |<span data-ttu-id="898a3-186">说明</span><span class="sxs-lookup"><span data-stu-id="898a3-186">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="898a3-187">members</span><span class="sxs-lookup"><span data-stu-id="898a3-187">members</span></span>|<span data-ttu-id="898a3-188">[educationUser](../resources/educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="898a3-188">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="898a3-189">课程中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="898a3-189">All users in the class.</span></span> <span data-ttu-id="898a3-190">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="898a3-190">Nullable.</span></span>|
|<span data-ttu-id="898a3-191">schools</span><span class="sxs-lookup"><span data-stu-id="898a3-191">schools</span></span>|<span data-ttu-id="898a3-192">[educationSchool](../resources/educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="898a3-192">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="898a3-193">与此课程相关的所有学校。</span><span class="sxs-lookup"><span data-stu-id="898a3-193">All schools that this class is associated with.</span></span> <span data-ttu-id="898a3-194">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="898a3-194">Nullable.</span></span>|
|<span data-ttu-id="898a3-195">teachers</span><span class="sxs-lookup"><span data-stu-id="898a3-195">teachers</span></span>|<span data-ttu-id="898a3-196">[educationUser](../resources/educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="898a3-196">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="898a3-197">课程中的所有教师。</span><span class="sxs-lookup"><span data-stu-id="898a3-197">All teachers in the class.</span></span> <span data-ttu-id="898a3-198">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="898a3-198">Nullable.</span></span>|
|<span data-ttu-id="898a3-199">group</span><span class="sxs-lookup"><span data-stu-id="898a3-199">group</span></span>|[<span data-ttu-id="898a3-200">组</span><span class="sxs-lookup"><span data-stu-id="898a3-200">group</span></span>](../resources/group.md)| <span data-ttu-id="898a3-201">对应于此类 directory 组。</span><span class="sxs-lookup"><span data-stu-id="898a3-201">The directory group corresponding to this class.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="898a3-202">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="898a3-202">JSON representation</span></span>

<span data-ttu-id="898a3-203">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="898a3-203">The following is a JSON representation of the resource.</span></span>

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
