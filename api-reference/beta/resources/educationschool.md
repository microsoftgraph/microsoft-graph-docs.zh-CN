---
title: educationSchool 资源类型
description: '学校。 **EducationSchool**资源当前与 administrativeUnit 资源相对应并共享相同的 ID。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1b5e0807ae73110a921c70beef6a98589db41269
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972549"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="e922a-104">educationSchool 资源类型</span><span class="sxs-lookup"><span data-stu-id="e922a-104">educationSchool resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e922a-105">学校。</span><span class="sxs-lookup"><span data-stu-id="e922a-105">A school.</span></span> <span data-ttu-id="e922a-106">**EducationSchool**资源当前与[administrativeUnit](administrativeunit.md)资源相对应并共享相同的 ID。</span><span class="sxs-lookup"><span data-stu-id="e922a-106">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>

<span data-ttu-id="e922a-107">此资源是[educationOrganization](educationorganization.md)的子类型。</span><span class="sxs-lookup"><span data-stu-id="e922a-107">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e922a-108">方法</span><span class="sxs-lookup"><span data-stu-id="e922a-108">Methods</span></span>

| <span data-ttu-id="e922a-109">方法</span><span class="sxs-lookup"><span data-stu-id="e922a-109">Method</span></span>                                                                     | <span data-ttu-id="e922a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e922a-110">Return Type</span></span>                                      | <span data-ttu-id="e922a-111">说明</span><span class="sxs-lookup"><span data-stu-id="e922a-111">Description</span></span>                                                                                 |
| :------------------------------------------------------------------------- | :----------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="e922a-112">Get</span><span class="sxs-lookup"><span data-stu-id="e922a-112">Get</span></span>](../api/educationschool-get.md)                                       | [<span data-ttu-id="e922a-113">educationSchool</span><span class="sxs-lookup"><span data-stu-id="e922a-113">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="e922a-114">读取 **educationSchool** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e922a-114">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="e922a-115">Add class</span><span class="sxs-lookup"><span data-stu-id="e922a-115">Add class</span></span>](../api/educationschool-post-classes.md)                        | [<span data-ttu-id="e922a-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="e922a-116">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="e922a-117">通过发布到课程导航属性，为学校添加一个新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="e922a-117">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="e922a-118">List classes</span><span class="sxs-lookup"><span data-stu-id="e922a-118">List classes</span></span>](../api/educationschool-list-classes.md)                     | <span data-ttu-id="e922a-119">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e922a-119">[educationClass](educationclass.md) collection</span></span>   | <span data-ttu-id="e922a-120">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e922a-120">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="e922a-121">Remove class</span><span class="sxs-lookup"><span data-stu-id="e922a-121">Remove class</span></span>](../api/educationschool-delete-classes.md)                   | [<span data-ttu-id="e922a-122">educationClass</span><span class="sxs-lookup"><span data-stu-id="e922a-122">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="e922a-123">通过课程导航属性从学校删除 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="e922a-123">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="e922a-124">Add user</span><span class="sxs-lookup"><span data-stu-id="e922a-124">Add user</span></span>](../api/educationschool-post-users.md)                           | [<span data-ttu-id="e922a-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="e922a-125">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="e922a-126">通过发布到 **users** 导航属性，为学校添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="e922a-126">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="e922a-127">List users</span><span class="sxs-lookup"><span data-stu-id="e922a-127">List users</span></span>](../api/educationschool-list-users.md)                         | <span data-ttu-id="e922a-128">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e922a-128">[educationUser](educationuser.md) collection</span></span>     | <span data-ttu-id="e922a-129">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e922a-129">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="e922a-130">Remove user</span><span class="sxs-lookup"><span data-stu-id="e922a-130">Remove user</span></span>](../api/educationschool-delete-users.md)                      | [<span data-ttu-id="e922a-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="e922a-131">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="e922a-132">通过 **users** 导航属性从学校删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="e922a-132">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="e922a-133">获取 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="e922a-133">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) | [<span data-ttu-id="e922a-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="e922a-134">administrativeUnit</span></span>](administrativeunit.md)      | <span data-ttu-id="e922a-135">获取与此**educationSchool**相对应的**administrativeUnit** 。</span><span class="sxs-lookup"><span data-stu-id="e922a-135">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>                |
| [<span data-ttu-id="e922a-136">Update</span><span class="sxs-lookup"><span data-stu-id="e922a-136">Update</span></span>](../api/educationschool-update.md)                                 | [<span data-ttu-id="e922a-137">educationSchool</span><span class="sxs-lookup"><span data-stu-id="e922a-137">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="e922a-138">更新 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="e922a-138">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="e922a-139">删除</span><span class="sxs-lookup"><span data-stu-id="e922a-139">Delete</span></span>](../api/educationschool-delete.md)                                 | <span data-ttu-id="e922a-140">无</span><span class="sxs-lookup"><span data-stu-id="e922a-140">None</span></span>                                             | <span data-ttu-id="e922a-141">删除 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="e922a-141">Delete an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="e922a-142">Delta</span><span class="sxs-lookup"><span data-stu-id="e922a-142">Delta</span></span>](../api/educationschool-delta.md)                                   | <span data-ttu-id="e922a-143">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e922a-143">[educationSchool](educationschool.md) collection</span></span> | <span data-ttu-id="e922a-144">获取**educationSchools**的增量更改</span><span class="sxs-lookup"><span data-stu-id="e922a-144">Get incremental changes for **educationSchools**</span></span>                                            |

## <a name="properties"></a><span data-ttu-id="e922a-145">属性</span><span class="sxs-lookup"><span data-stu-id="e922a-145">Properties</span></span>

| <span data-ttu-id="e922a-146">属性</span><span class="sxs-lookup"><span data-stu-id="e922a-146">Property</span></span>            | <span data-ttu-id="e922a-147">类型</span><span class="sxs-lookup"><span data-stu-id="e922a-147">Type</span></span>                                  | <span data-ttu-id="e922a-148">说明</span><span class="sxs-lookup"><span data-stu-id="e922a-148">Description</span></span>                                        |
| :------------------ | :------------------------------------ | :------------------------------------------------- |
| <span data-ttu-id="e922a-149">id</span><span class="sxs-lookup"><span data-stu-id="e922a-149">id</span></span>                  | <span data-ttu-id="e922a-150">字符串</span><span class="sxs-lookup"><span data-stu-id="e922a-150">String</span></span>                                | <span data-ttu-id="e922a-151">该学校的 GUID。</span><span class="sxs-lookup"><span data-stu-id="e922a-151">GUID of this school.</span></span>                               |
| <span data-ttu-id="e922a-152">address</span><span class="sxs-lookup"><span data-stu-id="e922a-152">address</span></span>             | [<span data-ttu-id="e922a-153">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="e922a-153">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="e922a-154">学校地址。</span><span class="sxs-lookup"><span data-stu-id="e922a-154">Address of the school.</span></span>                             |
| <span data-ttu-id="e922a-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="e922a-155">createdBy</span></span>           | [<span data-ttu-id="e922a-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="e922a-156">identitySet</span></span>](identityset.md)         | <span data-ttu-id="e922a-157">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="e922a-157">Entity who created the school.</span></span>                     |
| <span data-ttu-id="e922a-158">说明</span><span class="sxs-lookup"><span data-stu-id="e922a-158">description</span></span>         | <span data-ttu-id="e922a-159">String</span><span class="sxs-lookup"><span data-stu-id="e922a-159">String</span></span>                                | <span data-ttu-id="e922a-160">学校描述。</span><span class="sxs-lookup"><span data-stu-id="e922a-160">Description of the school.</span></span>                         |
| <span data-ttu-id="e922a-161">displayName</span><span class="sxs-lookup"><span data-stu-id="e922a-161">displayName</span></span>         | <span data-ttu-id="e922a-162">字符串</span><span class="sxs-lookup"><span data-stu-id="e922a-162">String</span></span>                                | <span data-ttu-id="e922a-163">学校的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e922a-163">Display name of the school.</span></span>                        |
| <span data-ttu-id="e922a-164">externalId</span><span class="sxs-lookup"><span data-stu-id="e922a-164">externalId</span></span>          | <span data-ttu-id="e922a-165">String</span><span class="sxs-lookup"><span data-stu-id="e922a-165">String</span></span>                                | <span data-ttu-id="e922a-166">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="e922a-166">ID of school in syncing system.</span></span>                    |
| <span data-ttu-id="e922a-167">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="e922a-167">externalPrincipalId</span></span> | <span data-ttu-id="e922a-168">String</span><span class="sxs-lookup"><span data-stu-id="e922a-168">String</span></span>                                | <span data-ttu-id="e922a-169">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="e922a-169">ID of principal in syncing system.</span></span>                 |
| <span data-ttu-id="e922a-170">externalSource</span><span class="sxs-lookup"><span data-stu-id="e922a-170">externalSource</span></span>      | <span data-ttu-id="e922a-171">string</span><span class="sxs-lookup"><span data-stu-id="e922a-171">string</span></span>                                | <span data-ttu-id="e922a-172">只读。</span><span class="sxs-lookup"><span data-stu-id="e922a-172">Read-Only.</span></span> <span data-ttu-id="e922a-173">可能的值是：`sis` 或 `manual`。</span><span class="sxs-lookup"><span data-stu-id="e922a-173">Possible values are: `sis` or `manual`.</span></span> |
| <span data-ttu-id="e922a-174">fax</span><span class="sxs-lookup"><span data-stu-id="e922a-174">fax</span></span>                 | <span data-ttu-id="e922a-175">String</span><span class="sxs-lookup"><span data-stu-id="e922a-175">String</span></span>                                | <span data-ttu-id="e922a-176">学校传真号码。</span><span class="sxs-lookup"><span data-stu-id="e922a-176">Fax number of school.</span></span>                              |
| <span data-ttu-id="e922a-177">highestGrade</span><span class="sxs-lookup"><span data-stu-id="e922a-177">highestGrade</span></span>        | <span data-ttu-id="e922a-178">String</span><span class="sxs-lookup"><span data-stu-id="e922a-178">String</span></span>                                | <span data-ttu-id="e922a-179">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="e922a-179">Highest grade taught.</span></span>                              |
| <span data-ttu-id="e922a-180">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="e922a-180">lowestGrade</span></span>         | <span data-ttu-id="e922a-181">String</span><span class="sxs-lookup"><span data-stu-id="e922a-181">String</span></span>                                | <span data-ttu-id="e922a-182">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="e922a-182">Lowest grade taught.</span></span>                               |
| <span data-ttu-id="e922a-183">phone</span><span class="sxs-lookup"><span data-stu-id="e922a-183">phone</span></span>               | <span data-ttu-id="e922a-184">String</span><span class="sxs-lookup"><span data-stu-id="e922a-184">String</span></span>                                | <span data-ttu-id="e922a-185">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="e922a-185">Phone number of school.</span></span>                            |
| <span data-ttu-id="e922a-186">principalEmail</span><span class="sxs-lookup"><span data-stu-id="e922a-186">principalEmail</span></span>      | <span data-ttu-id="e922a-187">String</span><span class="sxs-lookup"><span data-stu-id="e922a-187">String</span></span>                                | <span data-ttu-id="e922a-188">主体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="e922a-188">Email address of the principal.</span></span>                    |
| <span data-ttu-id="e922a-189">principalName</span><span class="sxs-lookup"><span data-stu-id="e922a-189">principalName</span></span>       | <span data-ttu-id="e922a-190">String</span><span class="sxs-lookup"><span data-stu-id="e922a-190">String</span></span>                                | <span data-ttu-id="e922a-191">主体名称。</span><span class="sxs-lookup"><span data-stu-id="e922a-191">Name of the principal.</span></span>                             |
| <span data-ttu-id="e922a-192">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="e922a-192">schoolNumber</span></span>        | <span data-ttu-id="e922a-193">String</span><span class="sxs-lookup"><span data-stu-id="e922a-193">String</span></span>                                | <span data-ttu-id="e922a-194">学校编号。</span><span class="sxs-lookup"><span data-stu-id="e922a-194">School Number.</span></span>                                     |

## <a name="relationships"></a><span data-ttu-id="e922a-195">关系</span><span class="sxs-lookup"><span data-stu-id="e922a-195">Relationships</span></span>

| <span data-ttu-id="e922a-196">关系</span><span class="sxs-lookup"><span data-stu-id="e922a-196">Relationship</span></span> | <span data-ttu-id="e922a-197">类型</span><span class="sxs-lookup"><span data-stu-id="e922a-197">Type</span></span>                                           | <span data-ttu-id="e922a-198">说明</span><span class="sxs-lookup"><span data-stu-id="e922a-198">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="e922a-199">classes</span><span class="sxs-lookup"><span data-stu-id="e922a-199">classes</span></span>      | <span data-ttu-id="e922a-200">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e922a-200">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="e922a-201">在学校教授的课程。</span><span class="sxs-lookup"><span data-stu-id="e922a-201">Classes taught at the school.</span></span> <span data-ttu-id="e922a-202">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e922a-202">Nullable.</span></span> |
| <span data-ttu-id="e922a-203">users</span><span class="sxs-lookup"><span data-stu-id="e922a-203">users</span></span>        | <span data-ttu-id="e922a-204">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e922a-204">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="e922a-205">学校中的用户。</span><span class="sxs-lookup"><span data-stu-id="e922a-205">Users in the school.</span></span> <span data-ttu-id="e922a-206">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e922a-206">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="e922a-207">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e922a-207">JSON representation</span></span>

<span data-ttu-id="e922a-208">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e922a-208">The following is a JSON representation of the resource.</span></span>

<!-- {
"blockType": "resource",
"keyProperty": "id",
"optionalProperties": [

],
"@odata.type": "microsoft.graph.educationSchool"
}-->


```json
{
  "address": { "@odata.type": "microsoft.graph.physicalAddress" },
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "externalPrincipalId": "String",
  "externalSource": "string",
  "fax": "String",
  "highestGrade": "String",
  "id": "String (identifier)",
  "lowestGrade": "String",
  "phone": "String",
  "principalEmail": "String",
  "principalName": "String",
  "schoolNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [ 
    "Error: Resource educationSchool has documented navigation properties, but we thought it was a complex type!" 
  ]  
}-->
