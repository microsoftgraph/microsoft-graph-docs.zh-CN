---
title: educationSchool 资源类型
description: '学校。 **EducationSchool**资源当前与 administrativeUnit 资源相对应并共享相同的 ID。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 32ed190f39d84e4c756d265527f4f0a8bcaf73f5
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509810"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="81da4-104">educationSchool 资源类型</span><span class="sxs-lookup"><span data-stu-id="81da4-104">educationSchool resource type</span></span>

<span data-ttu-id="81da4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81da4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81da4-106">学校。</span><span class="sxs-lookup"><span data-stu-id="81da4-106">A school.</span></span> <span data-ttu-id="81da4-107">**EducationSchool**资源当前与[administrativeUnit](administrativeunit.md)资源相对应并共享相同的 ID。</span><span class="sxs-lookup"><span data-stu-id="81da4-107">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>

<span data-ttu-id="81da4-108">此资源是[educationOrganization](educationorganization.md)的子类型。</span><span class="sxs-lookup"><span data-stu-id="81da4-108">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>

## <a name="methods"></a><span data-ttu-id="81da4-109">方法</span><span class="sxs-lookup"><span data-stu-id="81da4-109">Methods</span></span>

| <span data-ttu-id="81da4-110">方法</span><span class="sxs-lookup"><span data-stu-id="81da4-110">Method</span></span>                                                                     | <span data-ttu-id="81da4-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="81da4-111">Return Type</span></span>                                      | <span data-ttu-id="81da4-112">说明</span><span class="sxs-lookup"><span data-stu-id="81da4-112">Description</span></span>                                                                                 |
| :------------------------------------------------------------------------- | :----------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="81da4-113">获取</span><span class="sxs-lookup"><span data-stu-id="81da4-113">Get</span></span>](../api/educationschool-get.md)                                       | [<span data-ttu-id="81da4-114">educationSchool</span><span class="sxs-lookup"><span data-stu-id="81da4-114">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="81da4-115">读取 **educationSchool** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="81da4-115">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="81da4-116">Add class</span><span class="sxs-lookup"><span data-stu-id="81da4-116">Add class</span></span>](../api/educationschool-post-classes.md)                        | [<span data-ttu-id="81da4-117">educationClass</span><span class="sxs-lookup"><span data-stu-id="81da4-117">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="81da4-118">通过发布到课程导航属性，为学校添加一个新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="81da4-118">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="81da4-119">List classes</span><span class="sxs-lookup"><span data-stu-id="81da4-119">List classes</span></span>](../api/educationschool-list-classes.md)                     | <span data-ttu-id="81da4-120">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81da4-120">[educationClass](educationclass.md) collection</span></span>   | <span data-ttu-id="81da4-121">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="81da4-121">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="81da4-122">Remove class</span><span class="sxs-lookup"><span data-stu-id="81da4-122">Remove class</span></span>](../api/educationschool-delete-classes.md)                   | [<span data-ttu-id="81da4-123">educationClass</span><span class="sxs-lookup"><span data-stu-id="81da4-123">educationClass</span></span>](educationclass.md)              | <span data-ttu-id="81da4-124">通过课程导航属性从学校删除 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="81da4-124">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="81da4-125">Add user</span><span class="sxs-lookup"><span data-stu-id="81da4-125">Add user</span></span>](../api/educationschool-post-users.md)                           | [<span data-ttu-id="81da4-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="81da4-126">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="81da4-127">通过发布到 **users** 导航属性，为学校添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="81da4-127">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="81da4-128">List users</span><span class="sxs-lookup"><span data-stu-id="81da4-128">List users</span></span>](../api/educationschool-list-users.md)                         | <span data-ttu-id="81da4-129">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81da4-129">[educationUser](educationuser.md) collection</span></span>     | <span data-ttu-id="81da4-130">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="81da4-130">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="81da4-131">Remove user</span><span class="sxs-lookup"><span data-stu-id="81da4-131">Remove user</span></span>](../api/educationschool-delete-users.md)                      | [<span data-ttu-id="81da4-132">educationUser</span><span class="sxs-lookup"><span data-stu-id="81da4-132">educationUser</span></span>](educationuser.md)                | <span data-ttu-id="81da4-133">通过 **users** 导航属性从学校删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="81da4-133">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="81da4-134">获取 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="81da4-134">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) | [<span data-ttu-id="81da4-135">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="81da4-135">administrativeUnit</span></span>](administrativeunit.md)      | <span data-ttu-id="81da4-136">获取与此**educationSchool**相对应的**administrativeUnit** 。</span><span class="sxs-lookup"><span data-stu-id="81da4-136">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>                |
| [<span data-ttu-id="81da4-137">Update</span><span class="sxs-lookup"><span data-stu-id="81da4-137">Update</span></span>](../api/educationschool-update.md)                                 | [<span data-ttu-id="81da4-138">educationSchool</span><span class="sxs-lookup"><span data-stu-id="81da4-138">educationSchool</span></span>](educationschool.md)            | <span data-ttu-id="81da4-139">更新 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="81da4-139">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="81da4-140">删除</span><span class="sxs-lookup"><span data-stu-id="81da4-140">Delete</span></span>](../api/educationschool-delete.md)                                 | <span data-ttu-id="81da4-141">无</span><span class="sxs-lookup"><span data-stu-id="81da4-141">None</span></span>                                             | <span data-ttu-id="81da4-142">删除 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="81da4-142">Delete an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="81da4-143">Delta</span><span class="sxs-lookup"><span data-stu-id="81da4-143">Delta</span></span>](../api/educationschool-delta.md)                                   | <span data-ttu-id="81da4-144">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81da4-144">[educationSchool](educationschool.md) collection</span></span> | <span data-ttu-id="81da4-145">获取**educationSchools**的增量更改</span><span class="sxs-lookup"><span data-stu-id="81da4-145">Get incremental changes for **educationSchools**</span></span>                                            |

## <a name="properties"></a><span data-ttu-id="81da4-146">属性</span><span class="sxs-lookup"><span data-stu-id="81da4-146">Properties</span></span>

| <span data-ttu-id="81da4-147">属性</span><span class="sxs-lookup"><span data-stu-id="81da4-147">Property</span></span>             | <span data-ttu-id="81da4-148">类型</span><span class="sxs-lookup"><span data-stu-id="81da4-148">Type</span></span>                                  | <span data-ttu-id="81da4-149">说明</span><span class="sxs-lookup"><span data-stu-id="81da4-149">Description</span></span>                                                                                                                                                          |
| :------------------- | :------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="81da4-150">id</span><span class="sxs-lookup"><span data-stu-id="81da4-150">id</span></span>                   | <span data-ttu-id="81da4-151">字符串</span><span class="sxs-lookup"><span data-stu-id="81da4-151">String</span></span>                                | <span data-ttu-id="81da4-152">该学校的 GUID。</span><span class="sxs-lookup"><span data-stu-id="81da4-152">GUID of this school.</span></span>                                                                                                                                                 |
| <span data-ttu-id="81da4-153">address</span><span class="sxs-lookup"><span data-stu-id="81da4-153">address</span></span>              | [<span data-ttu-id="81da4-154">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="81da4-154">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="81da4-155">学校地址。</span><span class="sxs-lookup"><span data-stu-id="81da4-155">Address of the school.</span></span>                                                                                                                                               |
| <span data-ttu-id="81da4-156">createdBy</span><span class="sxs-lookup"><span data-stu-id="81da4-156">createdBy</span></span>            | [<span data-ttu-id="81da4-157">identitySet</span><span class="sxs-lookup"><span data-stu-id="81da4-157">identitySet</span></span>](identityset.md)         | <span data-ttu-id="81da4-158">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="81da4-158">Entity who created the school.</span></span>                                                                                                                                       |
| <span data-ttu-id="81da4-159">说明</span><span class="sxs-lookup"><span data-stu-id="81da4-159">description</span></span>          | <span data-ttu-id="81da4-160">String</span><span class="sxs-lookup"><span data-stu-id="81da4-160">String</span></span>                                | <span data-ttu-id="81da4-161">学校描述。</span><span class="sxs-lookup"><span data-stu-id="81da4-161">Description of the school.</span></span>                                                                                                                                           |
| <span data-ttu-id="81da4-162">displayName</span><span class="sxs-lookup"><span data-stu-id="81da4-162">displayName</span></span>          | <span data-ttu-id="81da4-163">字符串</span><span class="sxs-lookup"><span data-stu-id="81da4-163">String</span></span>                                | <span data-ttu-id="81da4-164">学校的显示名称。</span><span class="sxs-lookup"><span data-stu-id="81da4-164">Display name of the school.</span></span>                                                                                                                                          |
| <span data-ttu-id="81da4-165">externalId</span><span class="sxs-lookup"><span data-stu-id="81da4-165">externalId</span></span>           | <span data-ttu-id="81da4-166">String</span><span class="sxs-lookup"><span data-stu-id="81da4-166">String</span></span>                                | <span data-ttu-id="81da4-167">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="81da4-167">ID of school in syncing system.</span></span>                                                                                                                                      |
| <span data-ttu-id="81da4-168">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="81da4-168">externalPrincipalId</span></span>  | <span data-ttu-id="81da4-169">字符串</span><span class="sxs-lookup"><span data-stu-id="81da4-169">String</span></span>                                | <span data-ttu-id="81da4-170">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="81da4-170">ID of principal in syncing system.</span></span>                                                                                                                                   |
| <span data-ttu-id="81da4-171">externalSource</span><span class="sxs-lookup"><span data-stu-id="81da4-171">externalSource</span></span>       | <span data-ttu-id="81da4-172">字符串</span><span class="sxs-lookup"><span data-stu-id="81da4-172">String</span></span>                                | <span data-ttu-id="81da4-173">从其生成此资源的外部源的类型（自动根据而确定 `externalSourceDetail` ）。</span><span class="sxs-lookup"><span data-stu-id="81da4-173">The type of external source this resource was generated from (automatically determined from `externalSourceDetail`).</span></span> <span data-ttu-id="81da4-174">可能的值包括： `sis` 、 `lms` 或 `manual` 。</span><span class="sxs-lookup"><span data-stu-id="81da4-174">Possible values are: `sis`, `lms`, or `manual`.</span></span> |
| <span data-ttu-id="81da4-175">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="81da4-175">externalSourceDetail</span></span> | <span data-ttu-id="81da4-176">字符串</span><span class="sxs-lookup"><span data-stu-id="81da4-176">String</span></span>                                | <span data-ttu-id="81da4-177">从中生成此资源的外部源的名称。</span><span class="sxs-lookup"><span data-stu-id="81da4-177">The name of the external source this resources was generated from.</span></span>                                                                                                   |
| <span data-ttu-id="81da4-178">highestGrade</span><span class="sxs-lookup"><span data-stu-id="81da4-178">highestGrade</span></span>         | <span data-ttu-id="81da4-179">字符串</span><span class="sxs-lookup"><span data-stu-id="81da4-179">String</span></span>                                | <span data-ttu-id="81da4-180">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="81da4-180">Highest grade taught.</span></span>                                                                                                                                                |
| <span data-ttu-id="81da4-181">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="81da4-181">lowestGrade</span></span>          | <span data-ttu-id="81da4-182">字符串</span><span class="sxs-lookup"><span data-stu-id="81da4-182">String</span></span>                                | <span data-ttu-id="81da4-183">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="81da4-183">Lowest grade taught.</span></span>                                                                                                                                                 |
| <span data-ttu-id="81da4-184">phone</span><span class="sxs-lookup"><span data-stu-id="81da4-184">phone</span></span>                | <span data-ttu-id="81da4-185">String</span><span class="sxs-lookup"><span data-stu-id="81da4-185">String</span></span>                                | <span data-ttu-id="81da4-186">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="81da4-186">Phone number of school.</span></span>                                                                                                                                              |
| <span data-ttu-id="81da4-187">principalEmail</span><span class="sxs-lookup"><span data-stu-id="81da4-187">principalEmail</span></span>       | <span data-ttu-id="81da4-188">字符串</span><span class="sxs-lookup"><span data-stu-id="81da4-188">String</span></span>                                | <span data-ttu-id="81da4-189">主体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="81da4-189">Email address of the principal.</span></span>                                                                                                                                      |
| <span data-ttu-id="81da4-190">principalName</span><span class="sxs-lookup"><span data-stu-id="81da4-190">principalName</span></span>        | <span data-ttu-id="81da4-191">字符串</span><span class="sxs-lookup"><span data-stu-id="81da4-191">String</span></span>                                | <span data-ttu-id="81da4-192">主体名称。</span><span class="sxs-lookup"><span data-stu-id="81da4-192">Name of the principal.</span></span>                                                                                                                                               |
| <span data-ttu-id="81da4-193">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="81da4-193">schoolNumber</span></span>         | <span data-ttu-id="81da4-194">字符串</span><span class="sxs-lookup"><span data-stu-id="81da4-194">String</span></span>                                | <span data-ttu-id="81da4-195">学校编号。</span><span class="sxs-lookup"><span data-stu-id="81da4-195">School Number.</span></span>                                                                                                                                                       |

## <a name="relationships"></a><span data-ttu-id="81da4-196">关系</span><span class="sxs-lookup"><span data-stu-id="81da4-196">Relationships</span></span>

| <span data-ttu-id="81da4-197">关系</span><span class="sxs-lookup"><span data-stu-id="81da4-197">Relationship</span></span> | <span data-ttu-id="81da4-198">类型</span><span class="sxs-lookup"><span data-stu-id="81da4-198">Type</span></span>                                           | <span data-ttu-id="81da4-199">说明</span><span class="sxs-lookup"><span data-stu-id="81da4-199">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="81da4-200">classes</span><span class="sxs-lookup"><span data-stu-id="81da4-200">classes</span></span>      | <span data-ttu-id="81da4-201">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81da4-201">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="81da4-202">在学校教授的课程。</span><span class="sxs-lookup"><span data-stu-id="81da4-202">Classes taught at the school.</span></span> <span data-ttu-id="81da4-203">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="81da4-203">Nullable.</span></span> |
| <span data-ttu-id="81da4-204">users</span><span class="sxs-lookup"><span data-stu-id="81da4-204">users</span></span>        | <span data-ttu-id="81da4-205">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81da4-205">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="81da4-206">学校中的用户。</span><span class="sxs-lookup"><span data-stu-id="81da4-206">Users in the school.</span></span> <span data-ttu-id="81da4-207">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="81da4-207">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="81da4-208">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81da4-208">JSON representation</span></span>

<span data-ttu-id="81da4-209">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81da4-209">The following is a JSON representation of the resource.</span></span>

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
