---
title: educationSchool 资源类型
description: '一种表示学校的资源，用于管理所表示学校的课程、教师和学生。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 2549d8babd000a36f0ff3ccd38541ef3c1b2e466
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925817"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="6fd1a-103">educationSchool 资源类型</span><span class="sxs-lookup"><span data-stu-id="6fd1a-103">educationSchool resource type</span></span>

<span data-ttu-id="6fd1a-104">一种表示学校的资源，用于管理所表示学校的课程、教师和学生。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-104">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  


## <a name="methods"></a><span data-ttu-id="6fd1a-105">方法</span><span class="sxs-lookup"><span data-stu-id="6fd1a-105">Methods</span></span>

| <span data-ttu-id="6fd1a-106">方法</span><span class="sxs-lookup"><span data-stu-id="6fd1a-106">Method</span></span>           | <span data-ttu-id="6fd1a-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="6fd1a-107">Return Type</span></span>    |<span data-ttu-id="6fd1a-108">说明</span><span class="sxs-lookup"><span data-stu-id="6fd1a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6fd1a-109">Get</span><span class="sxs-lookup"><span data-stu-id="6fd1a-109">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="6fd1a-110">educationSchool</span><span class="sxs-lookup"><span data-stu-id="6fd1a-110">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="6fd1a-111">读取 **educationSchool** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-111">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="6fd1a-112">Add class</span><span class="sxs-lookup"><span data-stu-id="6fd1a-112">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="6fd1a-113">educationClass</span><span class="sxs-lookup"><span data-stu-id="6fd1a-113">educationClass</span></span>](educationclass.md)| <span data-ttu-id="6fd1a-114">通过发布到课程导航属性，为学校添加一个新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-114">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="6fd1a-115">List classes</span><span class="sxs-lookup"><span data-stu-id="6fd1a-115">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="6fd1a-116">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6fd1a-116">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="6fd1a-117">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-117">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="6fd1a-118">Remove class</span><span class="sxs-lookup"><span data-stu-id="6fd1a-118">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="6fd1a-119">educationClass</span><span class="sxs-lookup"><span data-stu-id="6fd1a-119">educationClass</span></span>](educationclass.md)| <span data-ttu-id="6fd1a-120">通过课程导航属性从学校删除 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-120">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="6fd1a-121">Add user</span><span class="sxs-lookup"><span data-stu-id="6fd1a-121">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="6fd1a-122">educationUser</span><span class="sxs-lookup"><span data-stu-id="6fd1a-122">educationUser</span></span>](educationuser.md)| <span data-ttu-id="6fd1a-123">通过发布到 **users** 导航属性，为学校添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-123">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="6fd1a-124">List users</span><span class="sxs-lookup"><span data-stu-id="6fd1a-124">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="6fd1a-125">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6fd1a-125">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="6fd1a-126">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-126">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="6fd1a-127">Remove user</span><span class="sxs-lookup"><span data-stu-id="6fd1a-127">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="6fd1a-128">educationUser</span><span class="sxs-lookup"><span data-stu-id="6fd1a-128">educationUser</span></span>](educationuser.md)| <span data-ttu-id="6fd1a-129">通过 **users** 导航属性从学校删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-129">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="6fd1a-130">Update</span><span class="sxs-lookup"><span data-stu-id="6fd1a-130">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="6fd1a-131">educationSchool</span><span class="sxs-lookup"><span data-stu-id="6fd1a-131">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="6fd1a-132">更新 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-132">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="6fd1a-133">Delete</span><span class="sxs-lookup"><span data-stu-id="6fd1a-133">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="6fd1a-134">无</span><span class="sxs-lookup"><span data-stu-id="6fd1a-134">None</span></span> |<span data-ttu-id="6fd1a-135">删除 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-135">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6fd1a-136">属性</span><span class="sxs-lookup"><span data-stu-id="6fd1a-136">Properties</span></span>
| <span data-ttu-id="6fd1a-137">属性</span><span class="sxs-lookup"><span data-stu-id="6fd1a-137">Property</span></span>     | <span data-ttu-id="6fd1a-138">类型</span><span class="sxs-lookup"><span data-stu-id="6fd1a-138">Type</span></span>   |<span data-ttu-id="6fd1a-139">说明</span><span class="sxs-lookup"><span data-stu-id="6fd1a-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6fd1a-140">id</span><span class="sxs-lookup"><span data-stu-id="6fd1a-140">id</span></span>|<span data-ttu-id="6fd1a-141">String</span><span class="sxs-lookup"><span data-stu-id="6fd1a-141">String</span></span>|<span data-ttu-id="6fd1a-142">该学校的 GUID。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-142">GUID of this school.</span></span>|
|<span data-ttu-id="6fd1a-143">displayName</span><span class="sxs-lookup"><span data-stu-id="6fd1a-143">displayName</span></span>| <span data-ttu-id="6fd1a-144">String</span><span class="sxs-lookup"><span data-stu-id="6fd1a-144">String</span></span>| <span data-ttu-id="6fd1a-145">学校的显示名称。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-145">Display name of the school.</span></span>| 
|<span data-ttu-id="6fd1a-146">description</span><span class="sxs-lookup"><span data-stu-id="6fd1a-146">description</span></span>| <span data-ttu-id="6fd1a-147">String</span><span class="sxs-lookup"><span data-stu-id="6fd1a-147">String</span></span> | <span data-ttu-id="6fd1a-148">学校描述。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-148">Description of the school.</span></span>| 
|<span data-ttu-id="6fd1a-149">status</span><span class="sxs-lookup"><span data-stu-id="6fd1a-149">status</span></span>| <span data-ttu-id="6fd1a-150">string</span><span class="sxs-lookup"><span data-stu-id="6fd1a-150">string</span></span>| <span data-ttu-id="6fd1a-151">只读。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-151">Read-Only.</span></span> <span data-ttu-id="6fd1a-152">可能的值为： `inactive`， `active`， `expired`， `deleteable`。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-152">The possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="6fd1a-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="6fd1a-153">externalSource</span></span>| <span data-ttu-id="6fd1a-154">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="6fd1a-154">educationExternalSource</span></span>| <span data-ttu-id="6fd1a-155">只读。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-155">Read-Only.</span></span>  <span data-ttu-id="6fd1a-156">可能的值为： `sis`， `manual`， `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-156">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="6fd1a-157">principalEmail</span><span class="sxs-lookup"><span data-stu-id="6fd1a-157">principalEmail</span></span>| <span data-ttu-id="6fd1a-158">String</span><span class="sxs-lookup"><span data-stu-id="6fd1a-158">String</span></span>| <span data-ttu-id="6fd1a-159">主体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-159">Email address of the principal.</span></span>|
|<span data-ttu-id="6fd1a-160">principalName</span><span class="sxs-lookup"><span data-stu-id="6fd1a-160">principalName</span></span>| <span data-ttu-id="6fd1a-161">String</span><span class="sxs-lookup"><span data-stu-id="6fd1a-161">String</span></span> | <span data-ttu-id="6fd1a-162">主体名称。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-162">Name of the principal.</span></span>|
|<span data-ttu-id="6fd1a-163">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="6fd1a-163">externalPrincipalId</span></span>| <span data-ttu-id="6fd1a-164">String</span><span class="sxs-lookup"><span data-stu-id="6fd1a-164">String</span></span> | <span data-ttu-id="6fd1a-165">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-165">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="6fd1a-166">highestGrade</span><span class="sxs-lookup"><span data-stu-id="6fd1a-166">highestGrade</span></span>|<span data-ttu-id="6fd1a-167">String</span><span class="sxs-lookup"><span data-stu-id="6fd1a-167">String</span></span>| <span data-ttu-id="6fd1a-168">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-168">Highest grade taught.</span></span> |
|<span data-ttu-id="6fd1a-169">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="6fd1a-169">lowestGrade</span></span>|<span data-ttu-id="6fd1a-170">String</span><span class="sxs-lookup"><span data-stu-id="6fd1a-170">String</span></span>| <span data-ttu-id="6fd1a-171">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-171">Lowest grade taught.</span></span> |
|<span data-ttu-id="6fd1a-172">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="6fd1a-172">schoolNumber</span></span>|<span data-ttu-id="6fd1a-173">String</span><span class="sxs-lookup"><span data-stu-id="6fd1a-173">String</span></span>| <span data-ttu-id="6fd1a-174">学校编号。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-174">School Number.</span></span>|
|<span data-ttu-id="6fd1a-175">externalId</span><span class="sxs-lookup"><span data-stu-id="6fd1a-175">externalId</span></span>|<span data-ttu-id="6fd1a-176">String</span><span class="sxs-lookup"><span data-stu-id="6fd1a-176">String</span></span>| <span data-ttu-id="6fd1a-177">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-177">ID of school in syncing system.</span></span> |
|<span data-ttu-id="6fd1a-178">phone</span><span class="sxs-lookup"><span data-stu-id="6fd1a-178">phone</span></span>|<span data-ttu-id="6fd1a-179">String</span><span class="sxs-lookup"><span data-stu-id="6fd1a-179">String</span></span>| <span data-ttu-id="6fd1a-180">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-180">Phone number of school.</span></span> |
|<span data-ttu-id="6fd1a-181">fax</span><span class="sxs-lookup"><span data-stu-id="6fd1a-181">fax</span></span>|<span data-ttu-id="6fd1a-182">String</span><span class="sxs-lookup"><span data-stu-id="6fd1a-182">String</span></span>| <span data-ttu-id="6fd1a-183">学校传真号码。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-183">Fax number of school.</span></span> |
|<span data-ttu-id="6fd1a-184">address</span><span class="sxs-lookup"><span data-stu-id="6fd1a-184">address</span></span>|[<span data-ttu-id="6fd1a-185">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="6fd1a-185">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="6fd1a-186">学校地址。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-186">Address of the school.</span></span>|
|<span data-ttu-id="6fd1a-187">createdBy</span><span class="sxs-lookup"><span data-stu-id="6fd1a-187">createdBy</span></span>|[<span data-ttu-id="6fd1a-188">identitySet</span><span class="sxs-lookup"><span data-stu-id="6fd1a-188">identitySet</span></span>](identityset.md)|<span data-ttu-id="6fd1a-189">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-189">Entity who created the school.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fd1a-190">关系</span><span class="sxs-lookup"><span data-stu-id="6fd1a-190">Relationships</span></span>
| <span data-ttu-id="6fd1a-191">关系</span><span class="sxs-lookup"><span data-stu-id="6fd1a-191">Relationship</span></span> | <span data-ttu-id="6fd1a-192">类型</span><span class="sxs-lookup"><span data-stu-id="6fd1a-192">Type</span></span>   |<span data-ttu-id="6fd1a-193">说明</span><span class="sxs-lookup"><span data-stu-id="6fd1a-193">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6fd1a-194">classes</span><span class="sxs-lookup"><span data-stu-id="6fd1a-194">classes</span></span>|<span data-ttu-id="6fd1a-195">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6fd1a-195">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="6fd1a-196">在学校教授的课程。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-196">Classes taught at the school.</span></span> <span data-ttu-id="6fd1a-197">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-197">Nullable.</span></span>|
|<span data-ttu-id="6fd1a-198">users</span><span class="sxs-lookup"><span data-stu-id="6fd1a-198">users</span></span>|<span data-ttu-id="6fd1a-199">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6fd1a-199">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="6fd1a-200">学校中的用户。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-200">Users in the school.</span></span> <span data-ttu-id="6fd1a-201">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-201">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fd1a-202">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6fd1a-202">JSON representation</span></span>

<span data-ttu-id="6fd1a-203">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fd1a-203">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.educationOrganization",
  "@odata.type": "microsoft.graph.educationSchool"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "highestGrade": "String",
  "lowestGrade": "String",
  "schoolNumber": "String",
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalId": "String",
  "fax": "String",
  "phone": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
