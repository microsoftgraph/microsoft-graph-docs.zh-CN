---
title: educationSchool 资源类型
description: '学校。 **educationSchool**资源当前与 administrativeUnit 资源相对应并共享相同的 ID。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 893f01fffcc606c85cec30789ec94dd658b2a4b2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334191"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="7571a-104">educationSchool 资源类型</span><span class="sxs-lookup"><span data-stu-id="7571a-104">educationSchool resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7571a-105">学校。</span><span class="sxs-lookup"><span data-stu-id="7571a-105">A school.</span></span> <span data-ttu-id="7571a-106">**educationSchool**资源当前与[administrativeUnit](administrativeunit.md)资源相对应并共享相同的 ID。</span><span class="sxs-lookup"><span data-stu-id="7571a-106">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>  

<span data-ttu-id="7571a-107">此资源是[educationOrganization](educationorganization.md)的子类型。</span><span class="sxs-lookup"><span data-stu-id="7571a-107">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>




## <a name="methods"></a><span data-ttu-id="7571a-108">方法</span><span class="sxs-lookup"><span data-stu-id="7571a-108">Methods</span></span>

| <span data-ttu-id="7571a-109">方法</span><span class="sxs-lookup"><span data-stu-id="7571a-109">Method</span></span>           | <span data-ttu-id="7571a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="7571a-110">Return Type</span></span>    |<span data-ttu-id="7571a-111">说明</span><span class="sxs-lookup"><span data-stu-id="7571a-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7571a-112">Get</span><span class="sxs-lookup"><span data-stu-id="7571a-112">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="7571a-113">educationSchool</span><span class="sxs-lookup"><span data-stu-id="7571a-113">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="7571a-114">读取 **educationSchool** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7571a-114">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="7571a-115">Add class</span><span class="sxs-lookup"><span data-stu-id="7571a-115">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="7571a-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="7571a-116">educationClass</span></span>](educationclass.md)| <span data-ttu-id="7571a-117">通过发布到课程导航属性，为学校添加一个新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="7571a-117">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="7571a-118">List classes</span><span class="sxs-lookup"><span data-stu-id="7571a-118">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="7571a-119">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7571a-119">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="7571a-120">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7571a-120">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="7571a-121">Remove class</span><span class="sxs-lookup"><span data-stu-id="7571a-121">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="7571a-122">educationClass</span><span class="sxs-lookup"><span data-stu-id="7571a-122">educationClass</span></span>](educationclass.md)| <span data-ttu-id="7571a-123">通过课程导航属性从学校删除 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="7571a-123">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="7571a-124">Add user</span><span class="sxs-lookup"><span data-stu-id="7571a-124">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="7571a-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="7571a-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="7571a-126">通过发布到 **users** 导航属性，为学校添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="7571a-126">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="7571a-127">List users</span><span class="sxs-lookup"><span data-stu-id="7571a-127">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="7571a-128">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7571a-128">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="7571a-129">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7571a-129">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="7571a-130">Remove user</span><span class="sxs-lookup"><span data-stu-id="7571a-130">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="7571a-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="7571a-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="7571a-132">通过 **users** 导航属性从学校删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="7571a-132">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="7571a-133">获取 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="7571a-133">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) |[<span data-ttu-id="7571a-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="7571a-134">administrativeUnit</span></span>](administrativeunit.md)| <span data-ttu-id="7571a-135">获取与此**educationSchool**相对应的**administrativeUnit** 。</span><span class="sxs-lookup"><span data-stu-id="7571a-135">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="7571a-136">Update</span><span class="sxs-lookup"><span data-stu-id="7571a-136">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="7571a-137">educationSchool</span><span class="sxs-lookup"><span data-stu-id="7571a-137">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="7571a-138">更新 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="7571a-138">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="7571a-139">删除</span><span class="sxs-lookup"><span data-stu-id="7571a-139">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="7571a-140">无</span><span class="sxs-lookup"><span data-stu-id="7571a-140">None</span></span> |<span data-ttu-id="7571a-141">删除 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="7571a-141">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7571a-142">属性</span><span class="sxs-lookup"><span data-stu-id="7571a-142">Properties</span></span>
| <span data-ttu-id="7571a-143">属性</span><span class="sxs-lookup"><span data-stu-id="7571a-143">Property</span></span>     | <span data-ttu-id="7571a-144">类型</span><span class="sxs-lookup"><span data-stu-id="7571a-144">Type</span></span>   |<span data-ttu-id="7571a-145">说明</span><span class="sxs-lookup"><span data-stu-id="7571a-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7571a-146">id</span><span class="sxs-lookup"><span data-stu-id="7571a-146">id</span></span>|<span data-ttu-id="7571a-147">String</span><span class="sxs-lookup"><span data-stu-id="7571a-147">String</span></span>|<span data-ttu-id="7571a-148">该学校的 GUID。</span><span class="sxs-lookup"><span data-stu-id="7571a-148">GUID of this school.</span></span>|
|<span data-ttu-id="7571a-149">displayName</span><span class="sxs-lookup"><span data-stu-id="7571a-149">displayName</span></span>| <span data-ttu-id="7571a-150">String</span><span class="sxs-lookup"><span data-stu-id="7571a-150">String</span></span>| <span data-ttu-id="7571a-151">学校的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7571a-151">Display name of the school.</span></span>| 
|<span data-ttu-id="7571a-152">说明</span><span class="sxs-lookup"><span data-stu-id="7571a-152">description</span></span>| <span data-ttu-id="7571a-153">字符串</span><span class="sxs-lookup"><span data-stu-id="7571a-153">String</span></span> | <span data-ttu-id="7571a-154">学校描述。</span><span class="sxs-lookup"><span data-stu-id="7571a-154">Description of the school.</span></span>| 
|<span data-ttu-id="7571a-155">状态</span><span class="sxs-lookup"><span data-stu-id="7571a-155">status</span></span>| <span data-ttu-id="7571a-156">string</span><span class="sxs-lookup"><span data-stu-id="7571a-156">string</span></span>| <span data-ttu-id="7571a-157">只读。</span><span class="sxs-lookup"><span data-stu-id="7571a-157">Read-Only.</span></span> <span data-ttu-id="7571a-158">可取值为：`inactive`、`active`、`expired`、`deleteable`。</span><span class="sxs-lookup"><span data-stu-id="7571a-158">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="7571a-159">externalSource</span><span class="sxs-lookup"><span data-stu-id="7571a-159">externalSource</span></span>| <span data-ttu-id="7571a-160">string</span><span class="sxs-lookup"><span data-stu-id="7571a-160">string</span></span>| <span data-ttu-id="7571a-161">只读。</span><span class="sxs-lookup"><span data-stu-id="7571a-161">Read-Only.</span></span>  <span data-ttu-id="7571a-162">可取值为：`sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="7571a-162">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7571a-163">principalEmail</span><span class="sxs-lookup"><span data-stu-id="7571a-163">principalEmail</span></span>| <span data-ttu-id="7571a-164">String</span><span class="sxs-lookup"><span data-stu-id="7571a-164">String</span></span>| <span data-ttu-id="7571a-165">主体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="7571a-165">Email address of the principal.</span></span>|
|<span data-ttu-id="7571a-166">principalName</span><span class="sxs-lookup"><span data-stu-id="7571a-166">principalName</span></span>| <span data-ttu-id="7571a-167">String</span><span class="sxs-lookup"><span data-stu-id="7571a-167">String</span></span> | <span data-ttu-id="7571a-168">主体名称。</span><span class="sxs-lookup"><span data-stu-id="7571a-168">Name of the principal.</span></span>|
|<span data-ttu-id="7571a-169">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="7571a-169">externalPrincipalId</span></span>| <span data-ttu-id="7571a-170">String</span><span class="sxs-lookup"><span data-stu-id="7571a-170">String</span></span> | <span data-ttu-id="7571a-171">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="7571a-171">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="7571a-172">highestGrade</span><span class="sxs-lookup"><span data-stu-id="7571a-172">highestGrade</span></span>|<span data-ttu-id="7571a-173">String</span><span class="sxs-lookup"><span data-stu-id="7571a-173">String</span></span>| <span data-ttu-id="7571a-174">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="7571a-174">Highest grade taught.</span></span> |
|<span data-ttu-id="7571a-175">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="7571a-175">lowestGrade</span></span>|<span data-ttu-id="7571a-176">String</span><span class="sxs-lookup"><span data-stu-id="7571a-176">String</span></span>| <span data-ttu-id="7571a-177">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="7571a-177">Lowest grade taught.</span></span> |
|<span data-ttu-id="7571a-178">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="7571a-178">schoolNumber</span></span>|<span data-ttu-id="7571a-179">String</span><span class="sxs-lookup"><span data-stu-id="7571a-179">String</span></span>| <span data-ttu-id="7571a-180">学校编号。</span><span class="sxs-lookup"><span data-stu-id="7571a-180">School Number.</span></span>|
|<span data-ttu-id="7571a-181">externalId</span><span class="sxs-lookup"><span data-stu-id="7571a-181">externalId</span></span>|<span data-ttu-id="7571a-182">String</span><span class="sxs-lookup"><span data-stu-id="7571a-182">String</span></span>| <span data-ttu-id="7571a-183">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="7571a-183">ID of school in syncing system.</span></span> |
|<span data-ttu-id="7571a-184">phone</span><span class="sxs-lookup"><span data-stu-id="7571a-184">phone</span></span>|<span data-ttu-id="7571a-185">String</span><span class="sxs-lookup"><span data-stu-id="7571a-185">String</span></span>| <span data-ttu-id="7571a-186">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="7571a-186">Phone number of school.</span></span> |
|<span data-ttu-id="7571a-187">fax</span><span class="sxs-lookup"><span data-stu-id="7571a-187">fax</span></span>|<span data-ttu-id="7571a-188">String</span><span class="sxs-lookup"><span data-stu-id="7571a-188">String</span></span>| <span data-ttu-id="7571a-189">学校传真号码。</span><span class="sxs-lookup"><span data-stu-id="7571a-189">Fax number of school.</span></span> |
|<span data-ttu-id="7571a-190">address</span><span class="sxs-lookup"><span data-stu-id="7571a-190">address</span></span>|[<span data-ttu-id="7571a-191">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="7571a-191">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="7571a-192">学校地址。</span><span class="sxs-lookup"><span data-stu-id="7571a-192">Address of the school.</span></span>|
|<span data-ttu-id="7571a-193">createdBy</span><span class="sxs-lookup"><span data-stu-id="7571a-193">createdBy</span></span>|[<span data-ttu-id="7571a-194">identitySet</span><span class="sxs-lookup"><span data-stu-id="7571a-194">identitySet</span></span>](identityset.md)|<span data-ttu-id="7571a-195">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="7571a-195">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="7571a-196">关系</span><span class="sxs-lookup"><span data-stu-id="7571a-196">Relationships</span></span>
| <span data-ttu-id="7571a-197">关系</span><span class="sxs-lookup"><span data-stu-id="7571a-197">Relationship</span></span> | <span data-ttu-id="7571a-198">类型</span><span class="sxs-lookup"><span data-stu-id="7571a-198">Type</span></span>   |<span data-ttu-id="7571a-199">说明</span><span class="sxs-lookup"><span data-stu-id="7571a-199">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7571a-200">classes</span><span class="sxs-lookup"><span data-stu-id="7571a-200">classes</span></span>|<span data-ttu-id="7571a-201">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7571a-201">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="7571a-202">在学校教授的课程。</span><span class="sxs-lookup"><span data-stu-id="7571a-202">Classes taught at the school.</span></span> <span data-ttu-id="7571a-203">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="7571a-203">Nullable.</span></span>|
|<span data-ttu-id="7571a-204">users</span><span class="sxs-lookup"><span data-stu-id="7571a-204">users</span></span>|<span data-ttu-id="7571a-205">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7571a-205">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="7571a-206">学校中的用户。</span><span class="sxs-lookup"><span data-stu-id="7571a-206">Users in the school.</span></span> <span data-ttu-id="7571a-207">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="7571a-207">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7571a-208">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7571a-208">JSON representation</span></span>

<span data-ttu-id="7571a-209">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7571a-209">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
<!--
{
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
