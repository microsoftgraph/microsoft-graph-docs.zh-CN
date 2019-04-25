---
title: educationSchool 资源类型
description: '学校。 **educationSchool**资源当前与 administrativeUnit 资源相对应并共享相同的 ID。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 917395324e6ae519af468a4bb4b31056796e1498
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542920"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="2d8da-104">educationSchool 资源类型</span><span class="sxs-lookup"><span data-stu-id="2d8da-104">educationSchool resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d8da-105">学校。</span><span class="sxs-lookup"><span data-stu-id="2d8da-105">A school.</span></span> <span data-ttu-id="2d8da-106">**educationSchool**资源当前与[administrativeUnit](administrativeunit.md)资源相对应并共享相同的 ID。</span><span class="sxs-lookup"><span data-stu-id="2d8da-106">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>  

<span data-ttu-id="2d8da-107">此资源是[educationOrganization](educationorganization.md)的子类型。</span><span class="sxs-lookup"><span data-stu-id="2d8da-107">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>




## <a name="methods"></a><span data-ttu-id="2d8da-108">方法</span><span class="sxs-lookup"><span data-stu-id="2d8da-108">Methods</span></span>

| <span data-ttu-id="2d8da-109">方法</span><span class="sxs-lookup"><span data-stu-id="2d8da-109">Method</span></span>           | <span data-ttu-id="2d8da-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="2d8da-110">Return Type</span></span>    |<span data-ttu-id="2d8da-111">说明</span><span class="sxs-lookup"><span data-stu-id="2d8da-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2d8da-112">Get</span><span class="sxs-lookup"><span data-stu-id="2d8da-112">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="2d8da-113">educationSchool</span><span class="sxs-lookup"><span data-stu-id="2d8da-113">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="2d8da-114">读取 **educationSchool** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2d8da-114">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="2d8da-115">Add class</span><span class="sxs-lookup"><span data-stu-id="2d8da-115">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="2d8da-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="2d8da-116">educationClass</span></span>](educationclass.md)| <span data-ttu-id="2d8da-117">通过发布到课程导航属性，为学校添加一个新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="2d8da-117">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="2d8da-118">List classes</span><span class="sxs-lookup"><span data-stu-id="2d8da-118">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="2d8da-119">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2d8da-119">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="2d8da-120">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2d8da-120">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="2d8da-121">Remove class</span><span class="sxs-lookup"><span data-stu-id="2d8da-121">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="2d8da-122">educationClass</span><span class="sxs-lookup"><span data-stu-id="2d8da-122">educationClass</span></span>](educationclass.md)| <span data-ttu-id="2d8da-123">通过课程导航属性从学校删除 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="2d8da-123">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="2d8da-124">Add user</span><span class="sxs-lookup"><span data-stu-id="2d8da-124">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="2d8da-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="2d8da-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="2d8da-126">通过发布到 **users** 导航属性，为学校添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="2d8da-126">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="2d8da-127">List users</span><span class="sxs-lookup"><span data-stu-id="2d8da-127">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="2d8da-128">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2d8da-128">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="2d8da-129">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2d8da-129">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="2d8da-130">Remove user</span><span class="sxs-lookup"><span data-stu-id="2d8da-130">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="2d8da-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="2d8da-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="2d8da-132">通过 **users** 导航属性从学校删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="2d8da-132">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="2d8da-133">获取 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="2d8da-133">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) |[<span data-ttu-id="2d8da-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="2d8da-134">administrativeUnit</span></span>](administrativeunit.md)| <span data-ttu-id="2d8da-135">获取与此**educationSchool**相对应的**administrativeUnit** 。</span><span class="sxs-lookup"><span data-stu-id="2d8da-135">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="2d8da-136">Update</span><span class="sxs-lookup"><span data-stu-id="2d8da-136">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="2d8da-137">educationSchool</span><span class="sxs-lookup"><span data-stu-id="2d8da-137">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="2d8da-138">更新 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="2d8da-138">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="2d8da-139">删除</span><span class="sxs-lookup"><span data-stu-id="2d8da-139">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="2d8da-140">无</span><span class="sxs-lookup"><span data-stu-id="2d8da-140">None</span></span> |<span data-ttu-id="2d8da-141">删除 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="2d8da-141">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2d8da-142">属性</span><span class="sxs-lookup"><span data-stu-id="2d8da-142">Properties</span></span>
| <span data-ttu-id="2d8da-143">属性</span><span class="sxs-lookup"><span data-stu-id="2d8da-143">Property</span></span>     | <span data-ttu-id="2d8da-144">类型</span><span class="sxs-lookup"><span data-stu-id="2d8da-144">Type</span></span>   |<span data-ttu-id="2d8da-145">说明</span><span class="sxs-lookup"><span data-stu-id="2d8da-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d8da-146">id</span><span class="sxs-lookup"><span data-stu-id="2d8da-146">id</span></span>|<span data-ttu-id="2d8da-147">String</span><span class="sxs-lookup"><span data-stu-id="2d8da-147">String</span></span>|<span data-ttu-id="2d8da-148">该学校的 GUID。</span><span class="sxs-lookup"><span data-stu-id="2d8da-148">GUID of this school.</span></span>|
|<span data-ttu-id="2d8da-149">displayName</span><span class="sxs-lookup"><span data-stu-id="2d8da-149">displayName</span></span>| <span data-ttu-id="2d8da-150">String</span><span class="sxs-lookup"><span data-stu-id="2d8da-150">String</span></span>| <span data-ttu-id="2d8da-151">学校的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2d8da-151">Display name of the school.</span></span>| 
|<span data-ttu-id="2d8da-152">description</span><span class="sxs-lookup"><span data-stu-id="2d8da-152">description</span></span>| <span data-ttu-id="2d8da-153">String</span><span class="sxs-lookup"><span data-stu-id="2d8da-153">String</span></span> | <span data-ttu-id="2d8da-154">学校描述。</span><span class="sxs-lookup"><span data-stu-id="2d8da-154">Description of the school.</span></span>| 
|<span data-ttu-id="2d8da-155">status</span><span class="sxs-lookup"><span data-stu-id="2d8da-155">status</span></span>| <span data-ttu-id="2d8da-156">string</span><span class="sxs-lookup"><span data-stu-id="2d8da-156">string</span></span>| <span data-ttu-id="2d8da-157">只读。</span><span class="sxs-lookup"><span data-stu-id="2d8da-157">Read-Only.</span></span> <span data-ttu-id="2d8da-158">可取值为：`inactive`、`active`、`expired`、`deleteable`。</span><span class="sxs-lookup"><span data-stu-id="2d8da-158">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="2d8da-159">externalSource</span><span class="sxs-lookup"><span data-stu-id="2d8da-159">externalSource</span></span>| <span data-ttu-id="2d8da-160">string</span><span class="sxs-lookup"><span data-stu-id="2d8da-160">string</span></span>| <span data-ttu-id="2d8da-161">只读。</span><span class="sxs-lookup"><span data-stu-id="2d8da-161">Read-Only.</span></span>  <span data-ttu-id="2d8da-162">可取值为：`sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2d8da-162">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="2d8da-163">principalEmail</span><span class="sxs-lookup"><span data-stu-id="2d8da-163">principalEmail</span></span>| <span data-ttu-id="2d8da-164">String</span><span class="sxs-lookup"><span data-stu-id="2d8da-164">String</span></span>| <span data-ttu-id="2d8da-165">主体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="2d8da-165">Email address of the principal.</span></span>|
|<span data-ttu-id="2d8da-166">principalName</span><span class="sxs-lookup"><span data-stu-id="2d8da-166">principalName</span></span>| <span data-ttu-id="2d8da-167">String</span><span class="sxs-lookup"><span data-stu-id="2d8da-167">String</span></span> | <span data-ttu-id="2d8da-168">主体名称。</span><span class="sxs-lookup"><span data-stu-id="2d8da-168">Name of the principal.</span></span>|
|<span data-ttu-id="2d8da-169">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="2d8da-169">externalPrincipalId</span></span>| <span data-ttu-id="2d8da-170">String</span><span class="sxs-lookup"><span data-stu-id="2d8da-170">String</span></span> | <span data-ttu-id="2d8da-171">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="2d8da-171">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="2d8da-172">highestGrade</span><span class="sxs-lookup"><span data-stu-id="2d8da-172">highestGrade</span></span>|<span data-ttu-id="2d8da-173">String</span><span class="sxs-lookup"><span data-stu-id="2d8da-173">String</span></span>| <span data-ttu-id="2d8da-174">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="2d8da-174">Highest grade taught.</span></span> |
|<span data-ttu-id="2d8da-175">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="2d8da-175">lowestGrade</span></span>|<span data-ttu-id="2d8da-176">String</span><span class="sxs-lookup"><span data-stu-id="2d8da-176">String</span></span>| <span data-ttu-id="2d8da-177">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="2d8da-177">Lowest grade taught.</span></span> |
|<span data-ttu-id="2d8da-178">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="2d8da-178">schoolNumber</span></span>|<span data-ttu-id="2d8da-179">String</span><span class="sxs-lookup"><span data-stu-id="2d8da-179">String</span></span>| <span data-ttu-id="2d8da-180">学校编号。</span><span class="sxs-lookup"><span data-stu-id="2d8da-180">School Number.</span></span>|
|<span data-ttu-id="2d8da-181">externalId</span><span class="sxs-lookup"><span data-stu-id="2d8da-181">externalId</span></span>|<span data-ttu-id="2d8da-182">String</span><span class="sxs-lookup"><span data-stu-id="2d8da-182">String</span></span>| <span data-ttu-id="2d8da-183">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="2d8da-183">ID of school in syncing system.</span></span> |
|<span data-ttu-id="2d8da-184">phone</span><span class="sxs-lookup"><span data-stu-id="2d8da-184">phone</span></span>|<span data-ttu-id="2d8da-185">String</span><span class="sxs-lookup"><span data-stu-id="2d8da-185">String</span></span>| <span data-ttu-id="2d8da-186">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="2d8da-186">Phone number of school.</span></span> |
|<span data-ttu-id="2d8da-187">fax</span><span class="sxs-lookup"><span data-stu-id="2d8da-187">fax</span></span>|<span data-ttu-id="2d8da-188">String</span><span class="sxs-lookup"><span data-stu-id="2d8da-188">String</span></span>| <span data-ttu-id="2d8da-189">学校传真号码。</span><span class="sxs-lookup"><span data-stu-id="2d8da-189">Fax number of school.</span></span> |
|<span data-ttu-id="2d8da-190">address</span><span class="sxs-lookup"><span data-stu-id="2d8da-190">address</span></span>|[<span data-ttu-id="2d8da-191">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="2d8da-191">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="2d8da-192">学校地址。</span><span class="sxs-lookup"><span data-stu-id="2d8da-192">Address of the school.</span></span>|
|<span data-ttu-id="2d8da-193">createdBy</span><span class="sxs-lookup"><span data-stu-id="2d8da-193">createdBy</span></span>|[<span data-ttu-id="2d8da-194">identitySet</span><span class="sxs-lookup"><span data-stu-id="2d8da-194">identitySet</span></span>](identityset.md)|<span data-ttu-id="2d8da-195">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="2d8da-195">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="2d8da-196">关系</span><span class="sxs-lookup"><span data-stu-id="2d8da-196">Relationships</span></span>
| <span data-ttu-id="2d8da-197">关系</span><span class="sxs-lookup"><span data-stu-id="2d8da-197">Relationship</span></span> | <span data-ttu-id="2d8da-198">类型</span><span class="sxs-lookup"><span data-stu-id="2d8da-198">Type</span></span>   |<span data-ttu-id="2d8da-199">说明</span><span class="sxs-lookup"><span data-stu-id="2d8da-199">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d8da-200">classes</span><span class="sxs-lookup"><span data-stu-id="2d8da-200">classes</span></span>|<span data-ttu-id="2d8da-201">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2d8da-201">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="2d8da-202">在学校教授的课程。</span><span class="sxs-lookup"><span data-stu-id="2d8da-202">Classes taught at the school.</span></span> <span data-ttu-id="2d8da-203">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="2d8da-203">Nullable.</span></span>|
|<span data-ttu-id="2d8da-204">users</span><span class="sxs-lookup"><span data-stu-id="2d8da-204">users</span></span>|<span data-ttu-id="2d8da-205">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2d8da-205">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="2d8da-206">学校中的用户。</span><span class="sxs-lookup"><span data-stu-id="2d8da-206">Users in the school.</span></span> <span data-ttu-id="2d8da-207">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="2d8da-207">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d8da-208">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d8da-208">JSON representation</span></span>

<span data-ttu-id="2d8da-209">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d8da-209">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationschool.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
