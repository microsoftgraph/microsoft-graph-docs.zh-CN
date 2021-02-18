---
title: educationSchool 资源类型
description: '学校。 **educationSchool** 资源当前对应于 administrativeUnit 资源并共享相同的 ID。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f8481ad876cd5c4c9a2f1bc8ca67297c647475ba
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292635"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="75bea-104">educationSchool 资源类型</span><span class="sxs-lookup"><span data-stu-id="75bea-104">educationSchool resource type</span></span>

<span data-ttu-id="75bea-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75bea-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75bea-106">学校。</span><span class="sxs-lookup"><span data-stu-id="75bea-106">A school.</span></span> <span data-ttu-id="75bea-107">**educationSchool** 资源当前对应于 [administrativeUnit](administrativeunit.md)资源并共享相同的 ID。</span><span class="sxs-lookup"><span data-stu-id="75bea-107">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>

<span data-ttu-id="75bea-108">此资源是 [educationOrganization](educationorganization.md)的子类型。</span><span class="sxs-lookup"><span data-stu-id="75bea-108">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>

## <a name="methods"></a><span data-ttu-id="75bea-109">方法</span><span class="sxs-lookup"><span data-stu-id="75bea-109">Methods</span></span>

| <span data-ttu-id="75bea-110">方法</span><span class="sxs-lookup"><span data-stu-id="75bea-110">Method</span></span>                                                                     | <span data-ttu-id="75bea-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="75bea-111">Return Type</span></span>                                      | <span data-ttu-id="75bea-112">说明</span><span class="sxs-lookup"><span data-stu-id="75bea-112">Description</span></span>                                                                                 |
| :------------------------------------------------------------------------- | :----------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="75bea-113">获取</span><span class="sxs-lookup"><span data-stu-id="75bea-113">Get</span></span>](../api/educationschool-get.md)                                       | [<span data-ttu-id="75bea-114">educationSchool</span><span class="sxs-lookup"><span data-stu-id="75bea-114">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="75bea-115">读取 **educationSchool** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="75bea-115">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="75bea-116">Add class</span><span class="sxs-lookup"><span data-stu-id="75bea-116">Add class</span></span>](../api/educationschool-post-classes.md)                        | [<span data-ttu-id="75bea-117">educationClass</span><span class="sxs-lookup"><span data-stu-id="75bea-117">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="75bea-118">通过发布到课程导航属性，为学校添加一个新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="75bea-118">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="75bea-119">List classes</span><span class="sxs-lookup"><span data-stu-id="75bea-119">List classes</span></span>](../api/educationschool-list-classes.md)                     | <span data-ttu-id="75bea-120">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75bea-120">[educationClass](educationclass.md) collection</span></span>   | <span data-ttu-id="75bea-121">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="75bea-121">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="75bea-122">Remove class</span><span class="sxs-lookup"><span data-stu-id="75bea-122">Remove class</span></span>](../api/educationschool-delete-classes.md)                   | [<span data-ttu-id="75bea-123">educationClass</span><span class="sxs-lookup"><span data-stu-id="75bea-123">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="75bea-124">通过课程导航属性从学校删除 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="75bea-124">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="75bea-125">Add user</span><span class="sxs-lookup"><span data-stu-id="75bea-125">Add user</span></span>](../api/educationschool-post-users.md)                           | [<span data-ttu-id="75bea-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="75bea-126">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="75bea-127">通过发布到 **users** 导航属性，为学校添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="75bea-127">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="75bea-128">List users</span><span class="sxs-lookup"><span data-stu-id="75bea-128">List users</span></span>](../api/educationschool-list-users.md)                         | <span data-ttu-id="75bea-129">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75bea-129">[educationUser](educationuser.md) collection</span></span>     | <span data-ttu-id="75bea-130">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="75bea-130">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="75bea-131">Remove user</span><span class="sxs-lookup"><span data-stu-id="75bea-131">Remove user</span></span>](../api/educationschool-delete-users.md)                      | [<span data-ttu-id="75bea-132">educationUser</span><span class="sxs-lookup"><span data-stu-id="75bea-132">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="75bea-133">通过 **users** 导航属性从学校删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="75bea-133">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="75bea-134">获取 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="75bea-134">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) | [<span data-ttu-id="75bea-135">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="75bea-135">administrativeUnit</span></span>](administrativeunit.md)      | <span data-ttu-id="75bea-136">获取 **对应于此** **educationSchool 的 administrativeUnit。**</span><span class="sxs-lookup"><span data-stu-id="75bea-136">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>                |
| [<span data-ttu-id="75bea-137">Update</span><span class="sxs-lookup"><span data-stu-id="75bea-137">Update</span></span>](../api/educationschool-update.md)                                 | [<span data-ttu-id="75bea-138">educationSchool</span><span class="sxs-lookup"><span data-stu-id="75bea-138">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="75bea-139">更新 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="75bea-139">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="75bea-140">删除</span><span class="sxs-lookup"><span data-stu-id="75bea-140">Delete</span></span>](../api/educationschool-delete.md)                                 | <span data-ttu-id="75bea-141">无</span><span class="sxs-lookup"><span data-stu-id="75bea-141">None</span></span>                                             | <span data-ttu-id="75bea-142">删除 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="75bea-142">Delete an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="75bea-143">Delta</span><span class="sxs-lookup"><span data-stu-id="75bea-143">Delta</span></span>](../api/educationschool-delta.md)                                   | <span data-ttu-id="75bea-144">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75bea-144">[educationSchool](educationschool.md) collection</span></span> | <span data-ttu-id="75bea-145">获取 **educationSchools 的增量更改**</span><span class="sxs-lookup"><span data-stu-id="75bea-145">Get incremental changes for **educationSchools**</span></span>                                            |

## <a name="properties"></a><span data-ttu-id="75bea-146">属性</span><span class="sxs-lookup"><span data-stu-id="75bea-146">Properties</span></span>

| <span data-ttu-id="75bea-147">属性</span><span class="sxs-lookup"><span data-stu-id="75bea-147">Property</span></span>             | <span data-ttu-id="75bea-148">类型</span><span class="sxs-lookup"><span data-stu-id="75bea-148">Type</span></span>                                  | <span data-ttu-id="75bea-149">说明</span><span class="sxs-lookup"><span data-stu-id="75bea-149">Description</span></span>                                                                                                                                                          |
| :------------------- | :------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="75bea-150">id</span><span class="sxs-lookup"><span data-stu-id="75bea-150">id</span></span>                   | <span data-ttu-id="75bea-151">String</span><span class="sxs-lookup"><span data-stu-id="75bea-151">String</span></span>                                | <span data-ttu-id="75bea-152">该学校的 GUID。</span><span class="sxs-lookup"><span data-stu-id="75bea-152">GUID of this school.</span></span>                                                                                                                                                 |
| <span data-ttu-id="75bea-153">address</span><span class="sxs-lookup"><span data-stu-id="75bea-153">address</span></span>              | [<span data-ttu-id="75bea-154">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="75bea-154">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="75bea-155">学校地址。</span><span class="sxs-lookup"><span data-stu-id="75bea-155">Address of the school.</span></span>                                                                                                                                               |
| <span data-ttu-id="75bea-156">createdBy</span><span class="sxs-lookup"><span data-stu-id="75bea-156">createdBy</span></span>            | [<span data-ttu-id="75bea-157">identitySet</span><span class="sxs-lookup"><span data-stu-id="75bea-157">identitySet</span></span>](identityset.md)         | <span data-ttu-id="75bea-158">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="75bea-158">Entity who created the school.</span></span>                                                                                                                                       |
| <span data-ttu-id="75bea-159">description</span><span class="sxs-lookup"><span data-stu-id="75bea-159">description</span></span>          | <span data-ttu-id="75bea-160">String</span><span class="sxs-lookup"><span data-stu-id="75bea-160">String</span></span>                                | <span data-ttu-id="75bea-161">学校描述。</span><span class="sxs-lookup"><span data-stu-id="75bea-161">Description of the school.</span></span>                                                                                                                                           |
| <span data-ttu-id="75bea-162">displayName</span><span class="sxs-lookup"><span data-stu-id="75bea-162">displayName</span></span>          | <span data-ttu-id="75bea-163">String</span><span class="sxs-lookup"><span data-stu-id="75bea-163">String</span></span>                                | <span data-ttu-id="75bea-164">学校的显示名称。</span><span class="sxs-lookup"><span data-stu-id="75bea-164">Display name of the school.</span></span>                                                                                                                                          |
| <span data-ttu-id="75bea-165">externalId</span><span class="sxs-lookup"><span data-stu-id="75bea-165">externalId</span></span>           | <span data-ttu-id="75bea-166">String</span><span class="sxs-lookup"><span data-stu-id="75bea-166">String</span></span>                                | <span data-ttu-id="75bea-167">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="75bea-167">ID of school in syncing system.</span></span>                                                                                                                                      |
| <span data-ttu-id="75bea-168">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="75bea-168">externalPrincipalId</span></span>  | <span data-ttu-id="75bea-169">String</span><span class="sxs-lookup"><span data-stu-id="75bea-169">String</span></span>                                | <span data-ttu-id="75bea-170">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="75bea-170">ID of principal in syncing system.</span></span>                                                                                                                                   |
| <span data-ttu-id="75bea-171">externalSource</span><span class="sxs-lookup"><span data-stu-id="75bea-171">externalSource</span></span>       | <span data-ttu-id="75bea-172">String</span><span class="sxs-lookup"><span data-stu-id="75bea-172">String</span></span>                                | <span data-ttu-id="75bea-173">此资源的外部源类型由 (自动确定 `externalSourceDetail`) 。</span><span class="sxs-lookup"><span data-stu-id="75bea-173">The type of external source this resource was generated from (automatically determined from `externalSourceDetail`).</span></span> <span data-ttu-id="75bea-174">可能的值为： `sis`、 `lms`或 `manual`。</span><span class="sxs-lookup"><span data-stu-id="75bea-174">Possible values are: `sis`, `lms`, or `manual`.</span></span> |
| <span data-ttu-id="75bea-175">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="75bea-175">externalSourceDetail</span></span> | <span data-ttu-id="75bea-176">String</span><span class="sxs-lookup"><span data-stu-id="75bea-176">String</span></span>                                | <span data-ttu-id="75bea-177">生成这些资源的外部源的名称。</span><span class="sxs-lookup"><span data-stu-id="75bea-177">The name of the external source this resources was generated from.</span></span>                                                                                                   |
| <span data-ttu-id="75bea-178">highestGrade</span><span class="sxs-lookup"><span data-stu-id="75bea-178">highestGrade</span></span>         | <span data-ttu-id="75bea-179">String</span><span class="sxs-lookup"><span data-stu-id="75bea-179">String</span></span>                                | <span data-ttu-id="75bea-180">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="75bea-180">Highest grade taught.</span></span>                                                                                                                                                |
| <span data-ttu-id="75bea-181">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="75bea-181">lowestGrade</span></span>          | <span data-ttu-id="75bea-182">String</span><span class="sxs-lookup"><span data-stu-id="75bea-182">String</span></span>                                | <span data-ttu-id="75bea-183">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="75bea-183">Lowest grade taught.</span></span>                                                                                                                                                 |
| <span data-ttu-id="75bea-184">phone</span><span class="sxs-lookup"><span data-stu-id="75bea-184">phone</span></span>                | <span data-ttu-id="75bea-185">String</span><span class="sxs-lookup"><span data-stu-id="75bea-185">String</span></span>                                | <span data-ttu-id="75bea-186">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="75bea-186">Phone number of school.</span></span>                                                                                                                                              |
| <span data-ttu-id="75bea-187">principalEmail</span><span class="sxs-lookup"><span data-stu-id="75bea-187">principalEmail</span></span>       | <span data-ttu-id="75bea-188">String</span><span class="sxs-lookup"><span data-stu-id="75bea-188">String</span></span>                                | <span data-ttu-id="75bea-189">主体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="75bea-189">Email address of the principal.</span></span>                                                                                                                                      |
| <span data-ttu-id="75bea-190">principalName</span><span class="sxs-lookup"><span data-stu-id="75bea-190">principalName</span></span>        | <span data-ttu-id="75bea-191">String</span><span class="sxs-lookup"><span data-stu-id="75bea-191">String</span></span>                                | <span data-ttu-id="75bea-192">主体名称。</span><span class="sxs-lookup"><span data-stu-id="75bea-192">Name of the principal.</span></span>                                                                                                                                               |
| <span data-ttu-id="75bea-193">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="75bea-193">schoolNumber</span></span>         | <span data-ttu-id="75bea-194">String</span><span class="sxs-lookup"><span data-stu-id="75bea-194">String</span></span>                                | <span data-ttu-id="75bea-195">学校编号。</span><span class="sxs-lookup"><span data-stu-id="75bea-195">School Number.</span></span>                                                                                                                                                       |

## <a name="relationships"></a><span data-ttu-id="75bea-196">关系</span><span class="sxs-lookup"><span data-stu-id="75bea-196">Relationships</span></span>

| <span data-ttu-id="75bea-197">关系</span><span class="sxs-lookup"><span data-stu-id="75bea-197">Relationship</span></span> | <span data-ttu-id="75bea-198">类型</span><span class="sxs-lookup"><span data-stu-id="75bea-198">Type</span></span>                                           | <span data-ttu-id="75bea-199">说明</span><span class="sxs-lookup"><span data-stu-id="75bea-199">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="75bea-200">classes</span><span class="sxs-lookup"><span data-stu-id="75bea-200">classes</span></span>      | <span data-ttu-id="75bea-201">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75bea-201">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="75bea-202">在学校教授的课程。</span><span class="sxs-lookup"><span data-stu-id="75bea-202">Classes taught at the school.</span></span> <span data-ttu-id="75bea-203">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="75bea-203">Nullable.</span></span> |
| <span data-ttu-id="75bea-204">users</span><span class="sxs-lookup"><span data-stu-id="75bea-204">users</span></span>        | <span data-ttu-id="75bea-205">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75bea-205">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="75bea-206">学校中的用户。</span><span class="sxs-lookup"><span data-stu-id="75bea-206">Users in the school.</span></span> <span data-ttu-id="75bea-207">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="75bea-207">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="75bea-208">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="75bea-208">JSON representation</span></span>

<span data-ttu-id="75bea-209">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75bea-209">The following is a JSON representation of the resource.</span></span>

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
  ]
}-->


