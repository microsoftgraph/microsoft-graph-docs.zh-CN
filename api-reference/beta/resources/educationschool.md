---
title: educationSchool 资源类型
description: '学校。 **EducationSchool**资源当前与 administrativeUnit 资源相对应并共享相同的 ID。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9cded9db9ab9d7310a10ab690e05f49dca8711c8
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750141"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="9bbc9-104">educationSchool 资源类型</span><span class="sxs-lookup"><span data-stu-id="9bbc9-104">educationSchool resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bbc9-105">学校。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-105">A school.</span></span> <span data-ttu-id="9bbc9-106">**EducationSchool**资源当前与[administrativeUnit](administrativeunit.md)资源相对应并共享相同的 ID。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-106">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>

<span data-ttu-id="9bbc9-107">此资源是[educationOrganization](educationorganization.md)的子类型。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-107">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9bbc9-108">方法</span><span class="sxs-lookup"><span data-stu-id="9bbc9-108">Methods</span></span>

| <span data-ttu-id="9bbc9-109">方法</span><span class="sxs-lookup"><span data-stu-id="9bbc9-109">Method</span></span>                                                                     | <span data-ttu-id="9bbc9-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9bbc9-110">Return Type</span></span>                                      | <span data-ttu-id="9bbc9-111">说明</span><span class="sxs-lookup"><span data-stu-id="9bbc9-111">Description</span></span>                                                                                 |
| :------------------------------------------------------------------------- | :----------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="9bbc9-112">Get</span><span class="sxs-lookup"><span data-stu-id="9bbc9-112">Get</span></span>](../api/educationschool-get.md)                                       | [<span data-ttu-id="9bbc9-113">educationSchool</span><span class="sxs-lookup"><span data-stu-id="9bbc9-113">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="9bbc9-114">读取 **educationSchool** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-114">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="9bbc9-115">Add class</span><span class="sxs-lookup"><span data-stu-id="9bbc9-115">Add class</span></span>](../api/educationschool-post-classes.md)                        | [<span data-ttu-id="9bbc9-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="9bbc9-116">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="9bbc9-117">通过发布到课程导航属性，为学校添加一个新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-117">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="9bbc9-118">List classes</span><span class="sxs-lookup"><span data-stu-id="9bbc9-118">List classes</span></span>](../api/educationschool-list-classes.md)                     | <span data-ttu-id="9bbc9-119">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9bbc9-119">[educationClass](educationclass.md) collection</span></span>   | <span data-ttu-id="9bbc9-120">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-120">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="9bbc9-121">Remove class</span><span class="sxs-lookup"><span data-stu-id="9bbc9-121">Remove class</span></span>](../api/educationschool-delete-classes.md)                   | [<span data-ttu-id="9bbc9-122">educationClass</span><span class="sxs-lookup"><span data-stu-id="9bbc9-122">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="9bbc9-123">通过课程导航属性从学校删除 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-123">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="9bbc9-124">Add user</span><span class="sxs-lookup"><span data-stu-id="9bbc9-124">Add user</span></span>](../api/educationschool-post-users.md)                           | [<span data-ttu-id="9bbc9-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="9bbc9-125">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="9bbc9-126">通过发布到 **users** 导航属性，为学校添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-126">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="9bbc9-127">List users</span><span class="sxs-lookup"><span data-stu-id="9bbc9-127">List users</span></span>](../api/educationschool-list-users.md)                         | <span data-ttu-id="9bbc9-128">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9bbc9-128">[educationUser](educationuser.md) collection</span></span>     | <span data-ttu-id="9bbc9-129">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-129">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="9bbc9-130">Remove user</span><span class="sxs-lookup"><span data-stu-id="9bbc9-130">Remove user</span></span>](../api/educationschool-delete-users.md)                      | [<span data-ttu-id="9bbc9-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="9bbc9-131">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="9bbc9-132">通过 **users** 导航属性从学校删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-132">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="9bbc9-133">获取 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="9bbc9-133">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) | [<span data-ttu-id="9bbc9-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="9bbc9-134">administrativeUnit</span></span>](administrativeunit.md)      | <span data-ttu-id="9bbc9-135">获取与此**educationSchool**相对应的**administrativeUnit** 。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-135">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>                |
| [<span data-ttu-id="9bbc9-136">Update</span><span class="sxs-lookup"><span data-stu-id="9bbc9-136">Update</span></span>](../api/educationschool-update.md)                                 | [<span data-ttu-id="9bbc9-137">educationSchool</span><span class="sxs-lookup"><span data-stu-id="9bbc9-137">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="9bbc9-138">更新 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-138">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="9bbc9-139">删除</span><span class="sxs-lookup"><span data-stu-id="9bbc9-139">Delete</span></span>](../api/educationschool-delete.md)                                 | <span data-ttu-id="9bbc9-140">无</span><span class="sxs-lookup"><span data-stu-id="9bbc9-140">None</span></span>                                             | <span data-ttu-id="9bbc9-141">删除 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-141">Delete an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="9bbc9-142">Delta</span><span class="sxs-lookup"><span data-stu-id="9bbc9-142">Delta</span></span>](../api/educationschool-delta.md)                                   | <span data-ttu-id="9bbc9-143">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9bbc9-143">[educationSchool](educationschool.md) collection</span></span> | <span data-ttu-id="9bbc9-144">获取**educationSchools**的增量更改</span><span class="sxs-lookup"><span data-stu-id="9bbc9-144">Get incremental changes for **educationSchools**</span></span>                                            |

## <a name="properties"></a><span data-ttu-id="9bbc9-145">属性</span><span class="sxs-lookup"><span data-stu-id="9bbc9-145">Properties</span></span>

| <span data-ttu-id="9bbc9-146">属性</span><span class="sxs-lookup"><span data-stu-id="9bbc9-146">Property</span></span>            | <span data-ttu-id="9bbc9-147">类型</span><span class="sxs-lookup"><span data-stu-id="9bbc9-147">Type</span></span>                                  | <span data-ttu-id="9bbc9-148">说明</span><span class="sxs-lookup"><span data-stu-id="9bbc9-148">Description</span></span>                                        |
| :------------------ | :------------------------------------ | :------------------------------------------------- |
| <span data-ttu-id="9bbc9-149">id</span><span class="sxs-lookup"><span data-stu-id="9bbc9-149">id</span></span>                  | <span data-ttu-id="9bbc9-150">字符串</span><span class="sxs-lookup"><span data-stu-id="9bbc9-150">String</span></span>                                | <span data-ttu-id="9bbc9-151">该学校的 GUID。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-151">GUID of this school.</span></span>                               |
| <span data-ttu-id="9bbc9-152">address</span><span class="sxs-lookup"><span data-stu-id="9bbc9-152">address</span></span>             | [<span data-ttu-id="9bbc9-153">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="9bbc9-153">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="9bbc9-154">学校地址。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-154">Address of the school.</span></span>                             |
| <span data-ttu-id="9bbc9-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="9bbc9-155">createdBy</span></span>           | [<span data-ttu-id="9bbc9-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="9bbc9-156">identitySet</span></span>](identityset.md)         | <span data-ttu-id="9bbc9-157">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-157">Entity who created the school.</span></span>                     |
| <span data-ttu-id="9bbc9-158">说明</span><span class="sxs-lookup"><span data-stu-id="9bbc9-158">description</span></span>         | <span data-ttu-id="9bbc9-159">String</span><span class="sxs-lookup"><span data-stu-id="9bbc9-159">String</span></span>                                | <span data-ttu-id="9bbc9-160">学校描述。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-160">Description of the school.</span></span>                         |
| <span data-ttu-id="9bbc9-161">displayName</span><span class="sxs-lookup"><span data-stu-id="9bbc9-161">displayName</span></span>         | <span data-ttu-id="9bbc9-162">字符串</span><span class="sxs-lookup"><span data-stu-id="9bbc9-162">String</span></span>                                | <span data-ttu-id="9bbc9-163">学校的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-163">Display name of the school.</span></span>                        |
| <span data-ttu-id="9bbc9-164">externalId</span><span class="sxs-lookup"><span data-stu-id="9bbc9-164">externalId</span></span>          | <span data-ttu-id="9bbc9-165">String</span><span class="sxs-lookup"><span data-stu-id="9bbc9-165">String</span></span>                                | <span data-ttu-id="9bbc9-166">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-166">ID of school in syncing system.</span></span>                    |
| <span data-ttu-id="9bbc9-167">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="9bbc9-167">externalPrincipalId</span></span> | <span data-ttu-id="9bbc9-168">String</span><span class="sxs-lookup"><span data-stu-id="9bbc9-168">String</span></span>                                | <span data-ttu-id="9bbc9-169">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-169">ID of principal in syncing system.</span></span>                 |
| <span data-ttu-id="9bbc9-170">externalSource</span><span class="sxs-lookup"><span data-stu-id="9bbc9-170">externalSource</span></span>      | <span data-ttu-id="9bbc9-171">string</span><span class="sxs-lookup"><span data-stu-id="9bbc9-171">string</span></span>                                | <span data-ttu-id="9bbc9-172">只读。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-172">Read-Only.</span></span> <span data-ttu-id="9bbc9-173">可能的值是：`sis` 或 `manual`。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-173">Possible values are: `sis` or `manual`.</span></span> |
| <span data-ttu-id="9bbc9-174">fax</span><span class="sxs-lookup"><span data-stu-id="9bbc9-174">fax</span></span>                 | <span data-ttu-id="9bbc9-175">String</span><span class="sxs-lookup"><span data-stu-id="9bbc9-175">String</span></span>                                | <span data-ttu-id="9bbc9-176">学校传真号码。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-176">Fax number of school.</span></span>                              |
| <span data-ttu-id="9bbc9-177">highestGrade</span><span class="sxs-lookup"><span data-stu-id="9bbc9-177">highestGrade</span></span>        | <span data-ttu-id="9bbc9-178">String</span><span class="sxs-lookup"><span data-stu-id="9bbc9-178">String</span></span>                                | <span data-ttu-id="9bbc9-179">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-179">Highest grade taught.</span></span>                              |
| <span data-ttu-id="9bbc9-180">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="9bbc9-180">lowestGrade</span></span>         | <span data-ttu-id="9bbc9-181">String</span><span class="sxs-lookup"><span data-stu-id="9bbc9-181">String</span></span>                                | <span data-ttu-id="9bbc9-182">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-182">Lowest grade taught.</span></span>                               |
| <span data-ttu-id="9bbc9-183">phone</span><span class="sxs-lookup"><span data-stu-id="9bbc9-183">phone</span></span>               | <span data-ttu-id="9bbc9-184">String</span><span class="sxs-lookup"><span data-stu-id="9bbc9-184">String</span></span>                                | <span data-ttu-id="9bbc9-185">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-185">Phone number of school.</span></span>                            |
| <span data-ttu-id="9bbc9-186">principalEmail</span><span class="sxs-lookup"><span data-stu-id="9bbc9-186">principalEmail</span></span>      | <span data-ttu-id="9bbc9-187">String</span><span class="sxs-lookup"><span data-stu-id="9bbc9-187">String</span></span>                                | <span data-ttu-id="9bbc9-188">主体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-188">Email address of the principal.</span></span>                    |
| <span data-ttu-id="9bbc9-189">principalName</span><span class="sxs-lookup"><span data-stu-id="9bbc9-189">principalName</span></span>       | <span data-ttu-id="9bbc9-190">String</span><span class="sxs-lookup"><span data-stu-id="9bbc9-190">String</span></span>                                | <span data-ttu-id="9bbc9-191">主体名称。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-191">Name of the principal.</span></span>                             |
| <span data-ttu-id="9bbc9-192">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="9bbc9-192">schoolNumber</span></span>        | <span data-ttu-id="9bbc9-193">String</span><span class="sxs-lookup"><span data-stu-id="9bbc9-193">String</span></span>                                | <span data-ttu-id="9bbc9-194">学校编号。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-194">School Number.</span></span>                                     |

## <a name="relationships"></a><span data-ttu-id="9bbc9-195">关系</span><span class="sxs-lookup"><span data-stu-id="9bbc9-195">Relationships</span></span>

| <span data-ttu-id="9bbc9-196">关系</span><span class="sxs-lookup"><span data-stu-id="9bbc9-196">Relationship</span></span> | <span data-ttu-id="9bbc9-197">类型</span><span class="sxs-lookup"><span data-stu-id="9bbc9-197">Type</span></span>                                           | <span data-ttu-id="9bbc9-198">说明</span><span class="sxs-lookup"><span data-stu-id="9bbc9-198">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="9bbc9-199">classes</span><span class="sxs-lookup"><span data-stu-id="9bbc9-199">classes</span></span>      | <span data-ttu-id="9bbc9-200">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9bbc9-200">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="9bbc9-201">在学校教授的课程。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-201">Classes taught at the school.</span></span> <span data-ttu-id="9bbc9-202">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-202">Nullable.</span></span> |
| <span data-ttu-id="9bbc9-203">users</span><span class="sxs-lookup"><span data-stu-id="9bbc9-203">users</span></span>        | <span data-ttu-id="9bbc9-204">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9bbc9-204">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="9bbc9-205">学校中的用户。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-205">Users in the school.</span></span> <span data-ttu-id="9bbc9-206">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-206">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="9bbc9-207">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9bbc9-207">JSON representation</span></span>

<span data-ttu-id="9bbc9-208">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9bbc9-208">The following is a JSON representation of the resource.</span></span>

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
