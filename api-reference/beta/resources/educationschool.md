---
title: educationSchool 资源类型
description: '学校。 **EducationSchool**资源当前与 administrativeUnit 资源相对应并共享相同的 ID。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 67baa3f5a57e968b53ae3f51a6c49b3743be25a6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500938"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="1a6e9-104">educationSchool 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a6e9-104">educationSchool resource type</span></span>

<span data-ttu-id="1a6e9-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1a6e9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a6e9-106">学校。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-106">A school.</span></span> <span data-ttu-id="1a6e9-107">**EducationSchool**资源当前与[administrativeUnit](administrativeunit.md)资源相对应并共享相同的 ID。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-107">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>

<span data-ttu-id="1a6e9-108">此资源是[educationOrganization](educationorganization.md)的子类型。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-108">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1a6e9-109">方法</span><span class="sxs-lookup"><span data-stu-id="1a6e9-109">Methods</span></span>

| <span data-ttu-id="1a6e9-110">方法</span><span class="sxs-lookup"><span data-stu-id="1a6e9-110">Method</span></span>                                                                     | <span data-ttu-id="1a6e9-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="1a6e9-111">Return Type</span></span>                                      | <span data-ttu-id="1a6e9-112">说明</span><span class="sxs-lookup"><span data-stu-id="1a6e9-112">Description</span></span>                                                                                 |
| :------------------------------------------------------------------------- | :----------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="1a6e9-113">获取</span><span class="sxs-lookup"><span data-stu-id="1a6e9-113">Get</span></span>](../api/educationschool-get.md)                                       | [<span data-ttu-id="1a6e9-114">educationSchool</span><span class="sxs-lookup"><span data-stu-id="1a6e9-114">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="1a6e9-115">读取 **educationSchool** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-115">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="1a6e9-116">Add class</span><span class="sxs-lookup"><span data-stu-id="1a6e9-116">Add class</span></span>](../api/educationschool-post-classes.md)                        | [<span data-ttu-id="1a6e9-117">educationClass</span><span class="sxs-lookup"><span data-stu-id="1a6e9-117">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="1a6e9-118">通过发布到课程导航属性，为学校添加一个新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-118">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="1a6e9-119">List classes</span><span class="sxs-lookup"><span data-stu-id="1a6e9-119">List classes</span></span>](../api/educationschool-list-classes.md)                     | <span data-ttu-id="1a6e9-120">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a6e9-120">[educationClass](educationclass.md) collection</span></span>   | <span data-ttu-id="1a6e9-121">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-121">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="1a6e9-122">Remove class</span><span class="sxs-lookup"><span data-stu-id="1a6e9-122">Remove class</span></span>](../api/educationschool-delete-classes.md)                   | [<span data-ttu-id="1a6e9-123">educationClass</span><span class="sxs-lookup"><span data-stu-id="1a6e9-123">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="1a6e9-124">通过课程导航属性从学校删除 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-124">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="1a6e9-125">Add user</span><span class="sxs-lookup"><span data-stu-id="1a6e9-125">Add user</span></span>](../api/educationschool-post-users.md)                           | [<span data-ttu-id="1a6e9-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="1a6e9-126">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="1a6e9-127">通过发布到 **users** 导航属性，为学校添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-127">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="1a6e9-128">List users</span><span class="sxs-lookup"><span data-stu-id="1a6e9-128">List users</span></span>](../api/educationschool-list-users.md)                         | <span data-ttu-id="1a6e9-129">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a6e9-129">[educationUser](educationuser.md) collection</span></span>     | <span data-ttu-id="1a6e9-130">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-130">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="1a6e9-131">Remove user</span><span class="sxs-lookup"><span data-stu-id="1a6e9-131">Remove user</span></span>](../api/educationschool-delete-users.md)                      | [<span data-ttu-id="1a6e9-132">educationUser</span><span class="sxs-lookup"><span data-stu-id="1a6e9-132">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="1a6e9-133">通过 **users** 导航属性从学校删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-133">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="1a6e9-134">获取 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="1a6e9-134">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) | [<span data-ttu-id="1a6e9-135">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="1a6e9-135">administrativeUnit</span></span>](administrativeunit.md)      | <span data-ttu-id="1a6e9-136">获取与此**educationSchool**相对应的**administrativeUnit** 。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-136">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>                |
| [<span data-ttu-id="1a6e9-137">Update</span><span class="sxs-lookup"><span data-stu-id="1a6e9-137">Update</span></span>](../api/educationschool-update.md)                                 | [<span data-ttu-id="1a6e9-138">educationSchool</span><span class="sxs-lookup"><span data-stu-id="1a6e9-138">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="1a6e9-139">更新 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-139">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="1a6e9-140">删除</span><span class="sxs-lookup"><span data-stu-id="1a6e9-140">Delete</span></span>](../api/educationschool-delete.md)                                 | <span data-ttu-id="1a6e9-141">无</span><span class="sxs-lookup"><span data-stu-id="1a6e9-141">None</span></span>                                             | <span data-ttu-id="1a6e9-142">删除 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-142">Delete an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="1a6e9-143">Delta</span><span class="sxs-lookup"><span data-stu-id="1a6e9-143">Delta</span></span>](../api/educationschool-delta.md)                                   | <span data-ttu-id="1a6e9-144">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a6e9-144">[educationSchool](educationschool.md) collection</span></span> | <span data-ttu-id="1a6e9-145">获取**educationSchools**的增量更改</span><span class="sxs-lookup"><span data-stu-id="1a6e9-145">Get incremental changes for **educationSchools**</span></span>                                            |

## <a name="properties"></a><span data-ttu-id="1a6e9-146">属性</span><span class="sxs-lookup"><span data-stu-id="1a6e9-146">Properties</span></span>

| <span data-ttu-id="1a6e9-147">属性</span><span class="sxs-lookup"><span data-stu-id="1a6e9-147">Property</span></span>            | <span data-ttu-id="1a6e9-148">类型</span><span class="sxs-lookup"><span data-stu-id="1a6e9-148">Type</span></span>                                  | <span data-ttu-id="1a6e9-149">说明</span><span class="sxs-lookup"><span data-stu-id="1a6e9-149">Description</span></span>                                        |
| :------------------ | :------------------------------------ | :------------------------------------------------- |
| <span data-ttu-id="1a6e9-150">id</span><span class="sxs-lookup"><span data-stu-id="1a6e9-150">id</span></span>                  | <span data-ttu-id="1a6e9-151">字符串</span><span class="sxs-lookup"><span data-stu-id="1a6e9-151">String</span></span>                                | <span data-ttu-id="1a6e9-152">该学校的 GUID。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-152">GUID of this school.</span></span>                               |
| <span data-ttu-id="1a6e9-153">address</span><span class="sxs-lookup"><span data-stu-id="1a6e9-153">address</span></span>             | [<span data-ttu-id="1a6e9-154">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="1a6e9-154">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="1a6e9-155">学校地址。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-155">Address of the school.</span></span>                             |
| <span data-ttu-id="1a6e9-156">createdBy</span><span class="sxs-lookup"><span data-stu-id="1a6e9-156">createdBy</span></span>           | [<span data-ttu-id="1a6e9-157">identitySet</span><span class="sxs-lookup"><span data-stu-id="1a6e9-157">identitySet</span></span>](identityset.md)         | <span data-ttu-id="1a6e9-158">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-158">Entity who created the school.</span></span>                     |
| <span data-ttu-id="1a6e9-159">说明</span><span class="sxs-lookup"><span data-stu-id="1a6e9-159">description</span></span>         | <span data-ttu-id="1a6e9-160">String</span><span class="sxs-lookup"><span data-stu-id="1a6e9-160">String</span></span>                                | <span data-ttu-id="1a6e9-161">学校描述。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-161">Description of the school.</span></span>                         |
| <span data-ttu-id="1a6e9-162">displayName</span><span class="sxs-lookup"><span data-stu-id="1a6e9-162">displayName</span></span>         | <span data-ttu-id="1a6e9-163">字符串</span><span class="sxs-lookup"><span data-stu-id="1a6e9-163">String</span></span>                                | <span data-ttu-id="1a6e9-164">学校的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-164">Display name of the school.</span></span>                        |
| <span data-ttu-id="1a6e9-165">externalId</span><span class="sxs-lookup"><span data-stu-id="1a6e9-165">externalId</span></span>          | <span data-ttu-id="1a6e9-166">String</span><span class="sxs-lookup"><span data-stu-id="1a6e9-166">String</span></span>                                | <span data-ttu-id="1a6e9-167">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-167">ID of school in syncing system.</span></span>                    |
| <span data-ttu-id="1a6e9-168">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="1a6e9-168">externalPrincipalId</span></span> | <span data-ttu-id="1a6e9-169">String</span><span class="sxs-lookup"><span data-stu-id="1a6e9-169">String</span></span>                                | <span data-ttu-id="1a6e9-170">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-170">ID of principal in syncing system.</span></span>                 |
| <span data-ttu-id="1a6e9-171">externalSource</span><span class="sxs-lookup"><span data-stu-id="1a6e9-171">externalSource</span></span>      | <span data-ttu-id="1a6e9-172">string</span><span class="sxs-lookup"><span data-stu-id="1a6e9-172">string</span></span>                                | <span data-ttu-id="1a6e9-173">只读。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-173">Read-Only.</span></span> <span data-ttu-id="1a6e9-174">可能的值是：`sis` 或 `manual`。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-174">Possible values are: `sis` or `manual`.</span></span> |
| <span data-ttu-id="1a6e9-175">highestGrade</span><span class="sxs-lookup"><span data-stu-id="1a6e9-175">highestGrade</span></span>        | <span data-ttu-id="1a6e9-176">String</span><span class="sxs-lookup"><span data-stu-id="1a6e9-176">String</span></span>                                | <span data-ttu-id="1a6e9-177">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-177">Highest grade taught.</span></span>                              |
| <span data-ttu-id="1a6e9-178">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="1a6e9-178">lowestGrade</span></span>         | <span data-ttu-id="1a6e9-179">String</span><span class="sxs-lookup"><span data-stu-id="1a6e9-179">String</span></span>                                | <span data-ttu-id="1a6e9-180">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-180">Lowest grade taught.</span></span>                               |
| <span data-ttu-id="1a6e9-181">phone</span><span class="sxs-lookup"><span data-stu-id="1a6e9-181">phone</span></span>               | <span data-ttu-id="1a6e9-182">String</span><span class="sxs-lookup"><span data-stu-id="1a6e9-182">String</span></span>                                | <span data-ttu-id="1a6e9-183">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-183">Phone number of school.</span></span>                            |
| <span data-ttu-id="1a6e9-184">principalEmail</span><span class="sxs-lookup"><span data-stu-id="1a6e9-184">principalEmail</span></span>      | <span data-ttu-id="1a6e9-185">String</span><span class="sxs-lookup"><span data-stu-id="1a6e9-185">String</span></span>                                | <span data-ttu-id="1a6e9-186">主体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-186">Email address of the principal.</span></span>                    |
| <span data-ttu-id="1a6e9-187">principalName</span><span class="sxs-lookup"><span data-stu-id="1a6e9-187">principalName</span></span>       | <span data-ttu-id="1a6e9-188">String</span><span class="sxs-lookup"><span data-stu-id="1a6e9-188">String</span></span>                                | <span data-ttu-id="1a6e9-189">主体名称。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-189">Name of the principal.</span></span>                             |
| <span data-ttu-id="1a6e9-190">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="1a6e9-190">schoolNumber</span></span>        | <span data-ttu-id="1a6e9-191">String</span><span class="sxs-lookup"><span data-stu-id="1a6e9-191">String</span></span>                                | <span data-ttu-id="1a6e9-192">学校编号。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-192">School Number.</span></span>                                     |

## <a name="relationships"></a><span data-ttu-id="1a6e9-193">关系</span><span class="sxs-lookup"><span data-stu-id="1a6e9-193">Relationships</span></span>

| <span data-ttu-id="1a6e9-194">关系</span><span class="sxs-lookup"><span data-stu-id="1a6e9-194">Relationship</span></span> | <span data-ttu-id="1a6e9-195">类型</span><span class="sxs-lookup"><span data-stu-id="1a6e9-195">Type</span></span>                                           | <span data-ttu-id="1a6e9-196">说明</span><span class="sxs-lookup"><span data-stu-id="1a6e9-196">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="1a6e9-197">classes</span><span class="sxs-lookup"><span data-stu-id="1a6e9-197">classes</span></span>      | <span data-ttu-id="1a6e9-198">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a6e9-198">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="1a6e9-199">在学校教授的课程。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-199">Classes taught at the school.</span></span> <span data-ttu-id="1a6e9-200">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-200">Nullable.</span></span> |
| <span data-ttu-id="1a6e9-201">users</span><span class="sxs-lookup"><span data-stu-id="1a6e9-201">users</span></span>        | <span data-ttu-id="1a6e9-202">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a6e9-202">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="1a6e9-203">学校中的用户。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-203">Users in the school.</span></span> <span data-ttu-id="1a6e9-204">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-204">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="1a6e9-205">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a6e9-205">JSON representation</span></span>

<span data-ttu-id="1a6e9-206">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a6e9-206">The following is a JSON representation of the resource.</span></span>

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
