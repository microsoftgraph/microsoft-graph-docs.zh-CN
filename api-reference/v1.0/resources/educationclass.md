---
title: educationClass 资源类型
description: '表示学校的课程。 **EducationClass**资源对应于 Microsoft 365 组并共享相同的 ID。 学生是课程的正式成员，教师为所有者，且具有相应权限。 若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 57e3204e15755e9ec7ce0150f46c6f0409ca3120
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032689"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="f986a-106">educationClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="f986a-106">educationClass resource type</span></span>

<span data-ttu-id="f986a-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f986a-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f986a-108">表示学校的课程。</span><span class="sxs-lookup"><span data-stu-id="f986a-108">Represents a class within a school.</span></span> <span data-ttu-id="f986a-109">**EducationClass**资源对应于 Microsoft 365 组并共享相同的 ID。</span><span class="sxs-lookup"><span data-stu-id="f986a-109">The **educationClass** resource corresponds to the Microsoft 365 group and shares the same ID.</span></span> <span data-ttu-id="f986a-110">学生是课程的正式成员，教师为所有者，且具有相应权限。</span><span class="sxs-lookup"><span data-stu-id="f986a-110">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="f986a-111">若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。</span><span class="sxs-lookup"><span data-stu-id="f986a-111">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="f986a-112">方法</span><span class="sxs-lookup"><span data-stu-id="f986a-112">Methods</span></span>

| <span data-ttu-id="f986a-113">方法</span><span class="sxs-lookup"><span data-stu-id="f986a-113">Method</span></span>           | <span data-ttu-id="f986a-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="f986a-114">Return Type</span></span>    |<span data-ttu-id="f986a-115">说明</span><span class="sxs-lookup"><span data-stu-id="f986a-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f986a-116">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="f986a-116">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="f986a-117">educationClass</span><span class="sxs-lookup"><span data-stu-id="f986a-117">educationClass</span></span>](educationclass.md) |<span data-ttu-id="f986a-118">读取 **educationClass** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f986a-118">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="f986a-119">Add member</span><span class="sxs-lookup"><span data-stu-id="f986a-119">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="f986a-120">educationUser</span><span class="sxs-lookup"><span data-stu-id="f986a-120">educationUser</span></span>](educationuser.md)| <span data-ttu-id="f986a-121">通过发布到 members 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="f986a-121">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="f986a-122">List members</span><span class="sxs-lookup"><span data-stu-id="f986a-122">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="f986a-123">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f986a-123">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="f986a-124">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f986a-124">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="f986a-125">Remove student</span><span class="sxs-lookup"><span data-stu-id="f986a-125">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="f986a-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="f986a-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="f986a-127">通过成员导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="f986a-127">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="f986a-128">List schools</span><span class="sxs-lookup"><span data-stu-id="f986a-128">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="f986a-129">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f986a-129">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="f986a-130">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f986a-130">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="f986a-131">Add teacher</span><span class="sxs-lookup"><span data-stu-id="f986a-131">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="f986a-132">educationUser</span><span class="sxs-lookup"><span data-stu-id="f986a-132">educationUser</span></span>](educationuser.md)| <span data-ttu-id="f986a-133">通过发布到 teachers 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="f986a-133">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="f986a-134">List teachers</span><span class="sxs-lookup"><span data-stu-id="f986a-134">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="f986a-135">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f986a-135">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="f986a-136">获取课程的教师列表。</span><span class="sxs-lookup"><span data-stu-id="f986a-136">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="f986a-137">Remove teacher</span><span class="sxs-lookup"><span data-stu-id="f986a-137">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="f986a-138">educationUser</span><span class="sxs-lookup"><span data-stu-id="f986a-138">educationUser</span></span>](educationuser.md)| <span data-ttu-id="f986a-139">通过教师导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="f986a-139">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="f986a-140">Get group</span><span class="sxs-lookup"><span data-stu-id="f986a-140">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="f986a-141">组</span><span class="sxs-lookup"><span data-stu-id="f986a-141">group</span></span>](group.md)| <span data-ttu-id="f986a-142">获取与此**educationClass**对应的 Microsoft 365**组**。</span><span class="sxs-lookup"><span data-stu-id="f986a-142">Get the Microsoft 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="f986a-143">Update</span><span class="sxs-lookup"><span data-stu-id="f986a-143">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="f986a-144">educationClass</span><span class="sxs-lookup"><span data-stu-id="f986a-144">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="f986a-145">更新 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="f986a-145">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="f986a-146">删除</span><span class="sxs-lookup"><span data-stu-id="f986a-146">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="f986a-147">无</span><span class="sxs-lookup"><span data-stu-id="f986a-147">None</span></span> |<span data-ttu-id="f986a-148">删除 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="f986a-148">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f986a-149">属性</span><span class="sxs-lookup"><span data-stu-id="f986a-149">Properties</span></span>
| <span data-ttu-id="f986a-150">属性</span><span class="sxs-lookup"><span data-stu-id="f986a-150">Property</span></span>     | <span data-ttu-id="f986a-151">类型</span><span class="sxs-lookup"><span data-stu-id="f986a-151">Type</span></span>   |<span data-ttu-id="f986a-152">说明</span><span class="sxs-lookup"><span data-stu-id="f986a-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f986a-153">id</span><span class="sxs-lookup"><span data-stu-id="f986a-153">id</span></span>| <span data-ttu-id="f986a-154">String</span><span class="sxs-lookup"><span data-stu-id="f986a-154">String</span></span>| <span data-ttu-id="f986a-155">课程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f986a-155">Unique identifier for the class.</span></span>|
|<span data-ttu-id="f986a-156">description</span><span class="sxs-lookup"><span data-stu-id="f986a-156">description</span></span>|<span data-ttu-id="f986a-157">String</span><span class="sxs-lookup"><span data-stu-id="f986a-157">String</span></span>| <span data-ttu-id="f986a-158">课程说明。</span><span class="sxs-lookup"><span data-stu-id="f986a-158">Description of the class.</span></span>|
|<span data-ttu-id="f986a-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f986a-159">displayName</span></span>|<span data-ttu-id="f986a-160">String</span><span class="sxs-lookup"><span data-stu-id="f986a-160">String</span></span>| <span data-ttu-id="f986a-161">课程名称。</span><span class="sxs-lookup"><span data-stu-id="f986a-161">Name of the class.</span></span>|
|<span data-ttu-id="f986a-162">mailNickname</span><span class="sxs-lookup"><span data-stu-id="f986a-162">mailNickname</span></span>|<span data-ttu-id="f986a-163">String</span><span class="sxs-lookup"><span data-stu-id="f986a-163">String</span></span>| <span data-ttu-id="f986a-164">向所有成员发送电子邮件的邮件名称（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="f986a-164">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="f986a-165">createdBy</span><span class="sxs-lookup"><span data-stu-id="f986a-165">createdBy</span></span>|[<span data-ttu-id="f986a-166">identitySet</span><span class="sxs-lookup"><span data-stu-id="f986a-166">identitySet</span></span>](identityset.md)| <span data-ttu-id="f986a-167">创建了课程的实体</span><span class="sxs-lookup"><span data-stu-id="f986a-167">Entity who created the class</span></span> |
|<span data-ttu-id="f986a-168">classCode</span><span class="sxs-lookup"><span data-stu-id="f986a-168">classCode</span></span>|<span data-ttu-id="f986a-169">String</span><span class="sxs-lookup"><span data-stu-id="f986a-169">String</span></span>| <span data-ttu-id="f986a-170">学校用于标识课程的课程代码。</span><span class="sxs-lookup"><span data-stu-id="f986a-170">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="f986a-171">externalId</span><span class="sxs-lookup"><span data-stu-id="f986a-171">externalId</span></span>|<span data-ttu-id="f986a-172">String</span><span class="sxs-lookup"><span data-stu-id="f986a-172">String</span></span>| <span data-ttu-id="f986a-173">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="f986a-173">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="f986a-174">externalName</span><span class="sxs-lookup"><span data-stu-id="f986a-174">externalName</span></span>|<span data-ttu-id="f986a-175">String</span><span class="sxs-lookup"><span data-stu-id="f986a-175">String</span></span>|<span data-ttu-id="f986a-176">同步系统中的课程名称。</span><span class="sxs-lookup"><span data-stu-id="f986a-176">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="f986a-177">externalSource</span><span class="sxs-lookup"><span data-stu-id="f986a-177">externalSource</span></span>|<span data-ttu-id="f986a-178">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="f986a-178">educationExternalSource</span></span>| <span data-ttu-id="f986a-179">此课程的创建方式。</span><span class="sxs-lookup"><span data-stu-id="f986a-179">How this class was created.</span></span> <span data-ttu-id="f986a-180">可能的值包括 `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="f986a-180">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f986a-181">term</span><span class="sxs-lookup"><span data-stu-id="f986a-181">term</span></span>|[<span data-ttu-id="f986a-182">educationTerm</span><span class="sxs-lookup"><span data-stu-id="f986a-182">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="f986a-183">此课程的学期。</span><span class="sxs-lookup"><span data-stu-id="f986a-183">Term for this class.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f986a-184">关系</span><span class="sxs-lookup"><span data-stu-id="f986a-184">Relationships</span></span>
| <span data-ttu-id="f986a-185">关系</span><span class="sxs-lookup"><span data-stu-id="f986a-185">Relationship</span></span> | <span data-ttu-id="f986a-186">类型</span><span class="sxs-lookup"><span data-stu-id="f986a-186">Type</span></span>   |<span data-ttu-id="f986a-187">说明</span><span class="sxs-lookup"><span data-stu-id="f986a-187">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f986a-188">成员</span><span class="sxs-lookup"><span data-stu-id="f986a-188">members</span></span>|<span data-ttu-id="f986a-189">[educationUser](../resources/educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f986a-189">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="f986a-190">课程中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="f986a-190">All users in the class.</span></span> <span data-ttu-id="f986a-191">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="f986a-191">Nullable.</span></span>|
|<span data-ttu-id="f986a-192">schools</span><span class="sxs-lookup"><span data-stu-id="f986a-192">schools</span></span>|<span data-ttu-id="f986a-193">[educationSchool](../resources/educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f986a-193">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="f986a-194">与此课程相关的所有学校。</span><span class="sxs-lookup"><span data-stu-id="f986a-194">All schools that this class is associated with.</span></span> <span data-ttu-id="f986a-195">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="f986a-195">Nullable.</span></span>|
|<span data-ttu-id="f986a-196">teachers</span><span class="sxs-lookup"><span data-stu-id="f986a-196">teachers</span></span>|<span data-ttu-id="f986a-197">[educationUser](../resources/educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f986a-197">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="f986a-198">课程中的所有教师。</span><span class="sxs-lookup"><span data-stu-id="f986a-198">All teachers in the class.</span></span> <span data-ttu-id="f986a-199">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="f986a-199">Nullable.</span></span>|
|<span data-ttu-id="f986a-200">group</span><span class="sxs-lookup"><span data-stu-id="f986a-200">group</span></span>|[<span data-ttu-id="f986a-201">组</span><span class="sxs-lookup"><span data-stu-id="f986a-201">group</span></span>](../resources/group.md)| <span data-ttu-id="f986a-202">与此类对应的目录组。</span><span class="sxs-lookup"><span data-stu-id="f986a-202">The directory group corresponding to this class.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f986a-203">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f986a-203">JSON representation</span></span>

<span data-ttu-id="f986a-204">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f986a-204">The following is a JSON representation of the resource.</span></span>

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

