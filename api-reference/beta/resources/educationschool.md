---
title: educationSchool 资源类型
description: '学校。 **educationSchool** 资源当前对应于 administrativeUnit 资源并共享同一 ID。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 17a5c3ad2f28e802bb6cad3a97d1cb723b3407d6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918243"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="79001-104">educationSchool 资源类型</span><span class="sxs-lookup"><span data-stu-id="79001-104">educationSchool resource type</span></span>

> <span data-ttu-id="79001-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="79001-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79001-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="79001-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79001-107">学校。</span><span class="sxs-lookup"><span data-stu-id="79001-107">A school.</span></span> <span data-ttu-id="79001-108">**educationSchool** 资源当前对应于 [administrativeUnit](administrativeunit.md) 资源并共享同一 ID。</span><span class="sxs-lookup"><span data-stu-id="79001-108">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>  

<span data-ttu-id="79001-109">此资源是 [educationOrganization](educationorganization.md) 的子类型。</span><span class="sxs-lookup"><span data-stu-id="79001-109">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>




## <a name="methods"></a><span data-ttu-id="79001-110">方法</span><span class="sxs-lookup"><span data-stu-id="79001-110">Methods</span></span>

| <span data-ttu-id="79001-111">方法</span><span class="sxs-lookup"><span data-stu-id="79001-111">Method</span></span>           | <span data-ttu-id="79001-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="79001-112">Return Type</span></span>    |<span data-ttu-id="79001-113">说明</span><span class="sxs-lookup"><span data-stu-id="79001-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="79001-114">Get</span><span class="sxs-lookup"><span data-stu-id="79001-114">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="79001-115">educationSchool</span><span class="sxs-lookup"><span data-stu-id="79001-115">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="79001-116">读取 **educationSchool** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="79001-116">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="79001-117">Add class</span><span class="sxs-lookup"><span data-stu-id="79001-117">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="79001-118">educationClass</span><span class="sxs-lookup"><span data-stu-id="79001-118">educationClass</span></span>](educationclass.md)| <span data-ttu-id="79001-119">通过发布到课程导航属性，为学校添加一个新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="79001-119">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="79001-120">List classes</span><span class="sxs-lookup"><span data-stu-id="79001-120">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="79001-121">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="79001-121">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="79001-122">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="79001-122">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="79001-123">Remove class</span><span class="sxs-lookup"><span data-stu-id="79001-123">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="79001-124">educationClass</span><span class="sxs-lookup"><span data-stu-id="79001-124">educationClass</span></span>](educationclass.md)| <span data-ttu-id="79001-125">通过课程导航属性从学校删除 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="79001-125">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="79001-126">Add user</span><span class="sxs-lookup"><span data-stu-id="79001-126">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="79001-127">educationUser</span><span class="sxs-lookup"><span data-stu-id="79001-127">educationUser</span></span>](educationuser.md)| <span data-ttu-id="79001-128">通过发布到 **users** 导航属性，为学校添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="79001-128">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="79001-129">List users</span><span class="sxs-lookup"><span data-stu-id="79001-129">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="79001-130">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="79001-130">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="79001-131">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="79001-131">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="79001-132">Remove user</span><span class="sxs-lookup"><span data-stu-id="79001-132">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="79001-133">educationUser</span><span class="sxs-lookup"><span data-stu-id="79001-133">educationUser</span></span>](educationuser.md)| <span data-ttu-id="79001-134">通过 **users** 导航属性从学校删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="79001-134">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="79001-135">Get administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="79001-135">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) |[<span data-ttu-id="79001-136">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="79001-136">administrativeUnit</span></span>](administrativeunit.md)| <span data-ttu-id="79001-137">获取与此 **educationSchool** 对应的 **administrativeUnit**。</span><span class="sxs-lookup"><span data-stu-id="79001-137">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="79001-138">Update</span><span class="sxs-lookup"><span data-stu-id="79001-138">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="79001-139">educationSchool</span><span class="sxs-lookup"><span data-stu-id="79001-139">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="79001-140">更新 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="79001-140">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="79001-141">Delete</span><span class="sxs-lookup"><span data-stu-id="79001-141">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="79001-142">无</span><span class="sxs-lookup"><span data-stu-id="79001-142">None</span></span> |<span data-ttu-id="79001-143">删除 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="79001-143">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="79001-144">属性</span><span class="sxs-lookup"><span data-stu-id="79001-144">Properties</span></span>
| <span data-ttu-id="79001-145">属性</span><span class="sxs-lookup"><span data-stu-id="79001-145">Property</span></span>     | <span data-ttu-id="79001-146">类型</span><span class="sxs-lookup"><span data-stu-id="79001-146">Type</span></span>   |<span data-ttu-id="79001-147">说明</span><span class="sxs-lookup"><span data-stu-id="79001-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79001-148">id</span><span class="sxs-lookup"><span data-stu-id="79001-148">id</span></span>|<span data-ttu-id="79001-149">String</span><span class="sxs-lookup"><span data-stu-id="79001-149">String</span></span>|<span data-ttu-id="79001-150">该学校的 GUID。</span><span class="sxs-lookup"><span data-stu-id="79001-150">GUID of this school.</span></span>|
|<span data-ttu-id="79001-151">displayName</span><span class="sxs-lookup"><span data-stu-id="79001-151">displayName</span></span>| <span data-ttu-id="79001-152">String</span><span class="sxs-lookup"><span data-stu-id="79001-152">String</span></span>| <span data-ttu-id="79001-153">学校的显示名称。</span><span class="sxs-lookup"><span data-stu-id="79001-153">Display name of the school.</span></span>| 
|<span data-ttu-id="79001-154">description</span><span class="sxs-lookup"><span data-stu-id="79001-154">description</span></span>| <span data-ttu-id="79001-155">String</span><span class="sxs-lookup"><span data-stu-id="79001-155">String</span></span> | <span data-ttu-id="79001-156">学校描述。</span><span class="sxs-lookup"><span data-stu-id="79001-156">Description of the school.</span></span>| 
|<span data-ttu-id="79001-157">status</span><span class="sxs-lookup"><span data-stu-id="79001-157">status</span></span>| <span data-ttu-id="79001-158">string</span><span class="sxs-lookup"><span data-stu-id="79001-158">string</span></span>| <span data-ttu-id="79001-159">只读。</span><span class="sxs-lookup"><span data-stu-id="79001-159">Read-Only.</span></span> <span data-ttu-id="79001-160">可取值为：`inactive`、`active`、`expired`、`deleteable`。</span><span class="sxs-lookup"><span data-stu-id="79001-160">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="79001-161">externalSource</span><span class="sxs-lookup"><span data-stu-id="79001-161">externalSource</span></span>| <span data-ttu-id="79001-162">string</span><span class="sxs-lookup"><span data-stu-id="79001-162">string</span></span>| <span data-ttu-id="79001-163">只读。</span><span class="sxs-lookup"><span data-stu-id="79001-163">Read-Only.</span></span>  <span data-ttu-id="79001-164">可取值为：`sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="79001-164">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="79001-165">principalEmail</span><span class="sxs-lookup"><span data-stu-id="79001-165">principalEmail</span></span>| <span data-ttu-id="79001-166">String</span><span class="sxs-lookup"><span data-stu-id="79001-166">String</span></span>| <span data-ttu-id="79001-167">主体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="79001-167">Email address of the principal.</span></span>|
|<span data-ttu-id="79001-168">principalName</span><span class="sxs-lookup"><span data-stu-id="79001-168">principalName</span></span>| <span data-ttu-id="79001-169">String</span><span class="sxs-lookup"><span data-stu-id="79001-169">String</span></span> | <span data-ttu-id="79001-170">主体名称。</span><span class="sxs-lookup"><span data-stu-id="79001-170">Name of the principal.</span></span>|
|<span data-ttu-id="79001-171">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="79001-171">externalPrincipalId</span></span>| <span data-ttu-id="79001-172">String</span><span class="sxs-lookup"><span data-stu-id="79001-172">String</span></span> | <span data-ttu-id="79001-173">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="79001-173">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="79001-174">highestGrade</span><span class="sxs-lookup"><span data-stu-id="79001-174">highestGrade</span></span>|<span data-ttu-id="79001-175">String</span><span class="sxs-lookup"><span data-stu-id="79001-175">String</span></span>| <span data-ttu-id="79001-176">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="79001-176">Highest grade taught.</span></span> |
|<span data-ttu-id="79001-177">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="79001-177">lowestGrade</span></span>|<span data-ttu-id="79001-178">String</span><span class="sxs-lookup"><span data-stu-id="79001-178">String</span></span>| <span data-ttu-id="79001-179">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="79001-179">Lowest grade taught.</span></span> |
|<span data-ttu-id="79001-180">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="79001-180">schoolNumber</span></span>|<span data-ttu-id="79001-181">String</span><span class="sxs-lookup"><span data-stu-id="79001-181">String</span></span>| <span data-ttu-id="79001-182">学校编号。</span><span class="sxs-lookup"><span data-stu-id="79001-182">School Number.</span></span>|
|<span data-ttu-id="79001-183">externalId</span><span class="sxs-lookup"><span data-stu-id="79001-183">externalId</span></span>|<span data-ttu-id="79001-184">String</span><span class="sxs-lookup"><span data-stu-id="79001-184">String</span></span>| <span data-ttu-id="79001-185">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="79001-185">ID of school in syncing system.</span></span> |
|<span data-ttu-id="79001-186">phone</span><span class="sxs-lookup"><span data-stu-id="79001-186">phone</span></span>|<span data-ttu-id="79001-187">String</span><span class="sxs-lookup"><span data-stu-id="79001-187">String</span></span>| <span data-ttu-id="79001-188">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="79001-188">Phone number of school.</span></span> |
|<span data-ttu-id="79001-189">fax</span><span class="sxs-lookup"><span data-stu-id="79001-189">fax</span></span>|<span data-ttu-id="79001-190">String</span><span class="sxs-lookup"><span data-stu-id="79001-190">String</span></span>| <span data-ttu-id="79001-191">学校传真号码。</span><span class="sxs-lookup"><span data-stu-id="79001-191">Fax number of school.</span></span> |
|<span data-ttu-id="79001-192">address</span><span class="sxs-lookup"><span data-stu-id="79001-192">address</span></span>|[<span data-ttu-id="79001-193">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="79001-193">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="79001-194">学校地址。</span><span class="sxs-lookup"><span data-stu-id="79001-194">Address of the school.</span></span>|
|<span data-ttu-id="79001-195">createdBy</span><span class="sxs-lookup"><span data-stu-id="79001-195">createdBy</span></span>|[<span data-ttu-id="79001-196">identitySet</span><span class="sxs-lookup"><span data-stu-id="79001-196">identitySet</span></span>](identityset.md)|<span data-ttu-id="79001-197">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="79001-197">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="79001-198">关系</span><span class="sxs-lookup"><span data-stu-id="79001-198">Relationships</span></span>
| <span data-ttu-id="79001-199">关系</span><span class="sxs-lookup"><span data-stu-id="79001-199">Relationship</span></span> | <span data-ttu-id="79001-200">类型</span><span class="sxs-lookup"><span data-stu-id="79001-200">Type</span></span>   |<span data-ttu-id="79001-201">说明</span><span class="sxs-lookup"><span data-stu-id="79001-201">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79001-202">classes</span><span class="sxs-lookup"><span data-stu-id="79001-202">classes</span></span>|<span data-ttu-id="79001-203">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="79001-203">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="79001-204">在学校教授的课程。</span><span class="sxs-lookup"><span data-stu-id="79001-204">Classes taught at the school.</span></span> <span data-ttu-id="79001-205">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="79001-205">Nullable.</span></span>|
|<span data-ttu-id="79001-206">users</span><span class="sxs-lookup"><span data-stu-id="79001-206">users</span></span>|<span data-ttu-id="79001-207">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="79001-207">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="79001-208">学校中的用户。</span><span class="sxs-lookup"><span data-stu-id="79001-208">Users in the school.</span></span> <span data-ttu-id="79001-209">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="79001-209">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="79001-210">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="79001-210">JSON representation</span></span>

<span data-ttu-id="79001-211">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79001-211">The following is a JSON representation of the resource.</span></span>

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
