---
title: educationSchool 资源类型
description: '学校。 **educationSchool** 资源当前对应于 administrativeUnit 资源并共享同一 ID。  '
ms.openlocfilehash: 6a478428874c7c600f60a6924dc06be5f4e3ba11
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046892"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="b215e-104">educationSchool 资源类型</span><span class="sxs-lookup"><span data-stu-id="b215e-104">educationSchool resource type</span></span>

> <span data-ttu-id="b215e-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b215e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b215e-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b215e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b215e-107">学校。</span><span class="sxs-lookup"><span data-stu-id="b215e-107">A school.</span></span> <span data-ttu-id="b215e-108">**educationSchool** 资源当前对应于 [administrativeUnit](administrativeunit.md) 资源并共享同一 ID。</span><span class="sxs-lookup"><span data-stu-id="b215e-108">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>  

<span data-ttu-id="b215e-109">此资源是 [educationOrganization](educationorganization.md) 的子类型。</span><span class="sxs-lookup"><span data-stu-id="b215e-109">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>




## <a name="methods"></a><span data-ttu-id="b215e-110">方法</span><span class="sxs-lookup"><span data-stu-id="b215e-110">Methods</span></span>

| <span data-ttu-id="b215e-111">方法</span><span class="sxs-lookup"><span data-stu-id="b215e-111">Method</span></span>           | <span data-ttu-id="b215e-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="b215e-112">Return Type</span></span>    |<span data-ttu-id="b215e-113">说明</span><span class="sxs-lookup"><span data-stu-id="b215e-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b215e-114">Get</span><span class="sxs-lookup"><span data-stu-id="b215e-114">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="b215e-115">educationSchool</span><span class="sxs-lookup"><span data-stu-id="b215e-115">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="b215e-116">读取 **educationSchool** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b215e-116">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="b215e-117">Add class</span><span class="sxs-lookup"><span data-stu-id="b215e-117">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="b215e-118">educationClass</span><span class="sxs-lookup"><span data-stu-id="b215e-118">educationClass</span></span>](educationclass.md)| <span data-ttu-id="b215e-119">通过发布到课程导航属性，为学校添加一个新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="b215e-119">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="b215e-120">List classes</span><span class="sxs-lookup"><span data-stu-id="b215e-120">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="b215e-121">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b215e-121">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="b215e-122">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b215e-122">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="b215e-123">Remove class</span><span class="sxs-lookup"><span data-stu-id="b215e-123">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="b215e-124">educationClass</span><span class="sxs-lookup"><span data-stu-id="b215e-124">educationClass</span></span>](educationclass.md)| <span data-ttu-id="b215e-125">通过课程导航属性从学校删除 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="b215e-125">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="b215e-126">Add user</span><span class="sxs-lookup"><span data-stu-id="b215e-126">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="b215e-127">educationUser</span><span class="sxs-lookup"><span data-stu-id="b215e-127">educationUser</span></span>](educationuser.md)| <span data-ttu-id="b215e-128">通过发布到 **users** 导航属性，为学校添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="b215e-128">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="b215e-129">List users</span><span class="sxs-lookup"><span data-stu-id="b215e-129">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="b215e-130">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b215e-130">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="b215e-131">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b215e-131">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="b215e-132">Remove user</span><span class="sxs-lookup"><span data-stu-id="b215e-132">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="b215e-133">educationUser</span><span class="sxs-lookup"><span data-stu-id="b215e-133">educationUser</span></span>](educationuser.md)| <span data-ttu-id="b215e-134">通过 **users** 导航属性从学校删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="b215e-134">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="b215e-135">Get administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="b215e-135">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) |[<span data-ttu-id="b215e-136">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="b215e-136">administrativeUnit</span></span>](administrativeunit.md)| <span data-ttu-id="b215e-137">获取与此 **educationSchool** 对应的 **administrativeUnit**。</span><span class="sxs-lookup"><span data-stu-id="b215e-137">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="b215e-138">Update</span><span class="sxs-lookup"><span data-stu-id="b215e-138">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="b215e-139">educationSchool</span><span class="sxs-lookup"><span data-stu-id="b215e-139">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="b215e-140">更新 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="b215e-140">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="b215e-141">Delete</span><span class="sxs-lookup"><span data-stu-id="b215e-141">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="b215e-142">无</span><span class="sxs-lookup"><span data-stu-id="b215e-142">None</span></span> |<span data-ttu-id="b215e-143">删除 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="b215e-143">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b215e-144">属性</span><span class="sxs-lookup"><span data-stu-id="b215e-144">Properties</span></span>
| <span data-ttu-id="b215e-145">属性</span><span class="sxs-lookup"><span data-stu-id="b215e-145">Property</span></span>     | <span data-ttu-id="b215e-146">类型</span><span class="sxs-lookup"><span data-stu-id="b215e-146">Type</span></span>   |<span data-ttu-id="b215e-147">说明</span><span class="sxs-lookup"><span data-stu-id="b215e-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b215e-148">id</span><span class="sxs-lookup"><span data-stu-id="b215e-148">id</span></span>|<span data-ttu-id="b215e-149">String</span><span class="sxs-lookup"><span data-stu-id="b215e-149">String</span></span>|<span data-ttu-id="b215e-150">该学校的 GUID。</span><span class="sxs-lookup"><span data-stu-id="b215e-150">GUID of this school.</span></span>|
|<span data-ttu-id="b215e-151">displayName</span><span class="sxs-lookup"><span data-stu-id="b215e-151">displayName</span></span>| <span data-ttu-id="b215e-152">String</span><span class="sxs-lookup"><span data-stu-id="b215e-152">String</span></span>| <span data-ttu-id="b215e-153">学校的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b215e-153">Display name of the school.</span></span>| 
|<span data-ttu-id="b215e-154">description</span><span class="sxs-lookup"><span data-stu-id="b215e-154">description</span></span>| <span data-ttu-id="b215e-155">String</span><span class="sxs-lookup"><span data-stu-id="b215e-155">String</span></span> | <span data-ttu-id="b215e-156">学校描述。</span><span class="sxs-lookup"><span data-stu-id="b215e-156">Description of the school.</span></span>| 
|<span data-ttu-id="b215e-157">status</span><span class="sxs-lookup"><span data-stu-id="b215e-157">status</span></span>| <span data-ttu-id="b215e-158">string</span><span class="sxs-lookup"><span data-stu-id="b215e-158">string</span></span>| <span data-ttu-id="b215e-159">只读。</span><span class="sxs-lookup"><span data-stu-id="b215e-159">Read-Only.</span></span> <span data-ttu-id="b215e-160">可取值为：`inactive`、`active`、`expired`、`deleteable`。</span><span class="sxs-lookup"><span data-stu-id="b215e-160">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="b215e-161">externalSource</span><span class="sxs-lookup"><span data-stu-id="b215e-161">externalSource</span></span>| <span data-ttu-id="b215e-162">string</span><span class="sxs-lookup"><span data-stu-id="b215e-162">string</span></span>| <span data-ttu-id="b215e-163">只读。</span><span class="sxs-lookup"><span data-stu-id="b215e-163">Read-Only.</span></span>  <span data-ttu-id="b215e-164">可取值为：`sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b215e-164">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b215e-165">principalEmail</span><span class="sxs-lookup"><span data-stu-id="b215e-165">principalEmail</span></span>| <span data-ttu-id="b215e-166">String</span><span class="sxs-lookup"><span data-stu-id="b215e-166">String</span></span>| <span data-ttu-id="b215e-167">主体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b215e-167">Email address of the principal.</span></span>|
|<span data-ttu-id="b215e-168">principalName</span><span class="sxs-lookup"><span data-stu-id="b215e-168">principalName</span></span>| <span data-ttu-id="b215e-169">String</span><span class="sxs-lookup"><span data-stu-id="b215e-169">String</span></span> | <span data-ttu-id="b215e-170">主体名称。</span><span class="sxs-lookup"><span data-stu-id="b215e-170">Name of the principal.</span></span>|
|<span data-ttu-id="b215e-171">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="b215e-171">externalPrincipalId</span></span>| <span data-ttu-id="b215e-172">String</span><span class="sxs-lookup"><span data-stu-id="b215e-172">String</span></span> | <span data-ttu-id="b215e-173">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="b215e-173">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="b215e-174">highestGrade</span><span class="sxs-lookup"><span data-stu-id="b215e-174">highestGrade</span></span>|<span data-ttu-id="b215e-175">String</span><span class="sxs-lookup"><span data-stu-id="b215e-175">String</span></span>| <span data-ttu-id="b215e-176">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="b215e-176">Highest grade taught.</span></span> |
|<span data-ttu-id="b215e-177">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="b215e-177">lowestGrade</span></span>|<span data-ttu-id="b215e-178">String</span><span class="sxs-lookup"><span data-stu-id="b215e-178">String</span></span>| <span data-ttu-id="b215e-179">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="b215e-179">Lowest grade taught.</span></span> |
|<span data-ttu-id="b215e-180">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="b215e-180">schoolNumber</span></span>|<span data-ttu-id="b215e-181">String</span><span class="sxs-lookup"><span data-stu-id="b215e-181">String</span></span>| <span data-ttu-id="b215e-182">学校编号。</span><span class="sxs-lookup"><span data-stu-id="b215e-182">School Number.</span></span>|
|<span data-ttu-id="b215e-183">externalId</span><span class="sxs-lookup"><span data-stu-id="b215e-183">externalId</span></span>|<span data-ttu-id="b215e-184">String</span><span class="sxs-lookup"><span data-stu-id="b215e-184">String</span></span>| <span data-ttu-id="b215e-185">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="b215e-185">ID of school in syncing system.</span></span> |
|<span data-ttu-id="b215e-186">phone</span><span class="sxs-lookup"><span data-stu-id="b215e-186">phone</span></span>|<span data-ttu-id="b215e-187">String</span><span class="sxs-lookup"><span data-stu-id="b215e-187">String</span></span>| <span data-ttu-id="b215e-188">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="b215e-188">Phone number of school.</span></span> |
|<span data-ttu-id="b215e-189">fax</span><span class="sxs-lookup"><span data-stu-id="b215e-189">fax</span></span>|<span data-ttu-id="b215e-190">String</span><span class="sxs-lookup"><span data-stu-id="b215e-190">String</span></span>| <span data-ttu-id="b215e-191">学校传真号码。</span><span class="sxs-lookup"><span data-stu-id="b215e-191">Fax number of school.</span></span> |
|<span data-ttu-id="b215e-192">address</span><span class="sxs-lookup"><span data-stu-id="b215e-192">address</span></span>|[<span data-ttu-id="b215e-193">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="b215e-193">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="b215e-194">学校地址。</span><span class="sxs-lookup"><span data-stu-id="b215e-194">Address of the school.</span></span>|
|<span data-ttu-id="b215e-195">createdBy</span><span class="sxs-lookup"><span data-stu-id="b215e-195">createdBy</span></span>|[<span data-ttu-id="b215e-196">identitySet</span><span class="sxs-lookup"><span data-stu-id="b215e-196">identitySet</span></span>](identityset.md)|<span data-ttu-id="b215e-197">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="b215e-197">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="b215e-198">关系</span><span class="sxs-lookup"><span data-stu-id="b215e-198">Relationships</span></span>
| <span data-ttu-id="b215e-199">关系</span><span class="sxs-lookup"><span data-stu-id="b215e-199">Relationship</span></span> | <span data-ttu-id="b215e-200">类型</span><span class="sxs-lookup"><span data-stu-id="b215e-200">Type</span></span>   |<span data-ttu-id="b215e-201">说明</span><span class="sxs-lookup"><span data-stu-id="b215e-201">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b215e-202">classes</span><span class="sxs-lookup"><span data-stu-id="b215e-202">classes</span></span>|<span data-ttu-id="b215e-203">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b215e-203">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="b215e-204">在学校教授的课程。</span><span class="sxs-lookup"><span data-stu-id="b215e-204">Classes taught at the school.</span></span> <span data-ttu-id="b215e-205">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="b215e-205">Nullable.</span></span>|
|<span data-ttu-id="b215e-206">users</span><span class="sxs-lookup"><span data-stu-id="b215e-206">users</span></span>|<span data-ttu-id="b215e-207">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b215e-207">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="b215e-208">学校中的用户。</span><span class="sxs-lookup"><span data-stu-id="b215e-208">Users in the school.</span></span> <span data-ttu-id="b215e-209">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="b215e-209">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b215e-210">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b215e-210">JSON representation</span></span>

<span data-ttu-id="b215e-211">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b215e-211">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
