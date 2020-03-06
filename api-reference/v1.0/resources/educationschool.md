---
title: educationSchool 资源类型
description: '一种表示学校的资源，用于管理所表示学校的课程、教师和学生。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 407f29c7d8f9468c5e9b1da1badad294cb655121
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531512"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="ccec6-103">educationSchool 资源类型</span><span class="sxs-lookup"><span data-stu-id="ccec6-103">educationSchool resource type</span></span>

<span data-ttu-id="ccec6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccec6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ccec6-105">一种表示学校的资源，用于管理所表示学校的课程、教师和学生。</span><span class="sxs-lookup"><span data-stu-id="ccec6-105">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  

## <a name="methods"></a><span data-ttu-id="ccec6-106">Methods</span><span class="sxs-lookup"><span data-stu-id="ccec6-106">Methods</span></span>

| <span data-ttu-id="ccec6-107">方法</span><span class="sxs-lookup"><span data-stu-id="ccec6-107">Method</span></span>                                                   | <span data-ttu-id="ccec6-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ccec6-108">Return Type</span></span>                                    | <span data-ttu-id="ccec6-109">说明</span><span class="sxs-lookup"><span data-stu-id="ccec6-109">Description</span></span>                                                                                 |
| :------------------------------------------------------- | :--------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="ccec6-110">Get</span><span class="sxs-lookup"><span data-stu-id="ccec6-110">Get</span></span>](../api/educationschool-get.md)                     | [<span data-ttu-id="ccec6-111">educationSchool</span><span class="sxs-lookup"><span data-stu-id="ccec6-111">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="ccec6-112">读取 **educationSchool** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ccec6-112">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="ccec6-113">Add class</span><span class="sxs-lookup"><span data-stu-id="ccec6-113">Add class</span></span>](../api/educationschool-post-classes.md)      | [<span data-ttu-id="ccec6-114">educationClass</span><span class="sxs-lookup"><span data-stu-id="ccec6-114">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="ccec6-115">通过发布到课程导航属性，为学校添加一个新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="ccec6-115">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="ccec6-116">List classes</span><span class="sxs-lookup"><span data-stu-id="ccec6-116">List classes</span></span>](../api/educationschool-list-classes.md)   | <span data-ttu-id="ccec6-117">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ccec6-117">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="ccec6-118">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ccec6-118">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="ccec6-119">Remove class</span><span class="sxs-lookup"><span data-stu-id="ccec6-119">Remove class</span></span>](../api/educationschool-delete-classes.md) | [<span data-ttu-id="ccec6-120">educationClass</span><span class="sxs-lookup"><span data-stu-id="ccec6-120">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="ccec6-121">通过课程导航属性从学校删除 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="ccec6-121">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="ccec6-122">Add user</span><span class="sxs-lookup"><span data-stu-id="ccec6-122">Add user</span></span>](../api/educationschool-post-users.md)         | [<span data-ttu-id="ccec6-123">educationUser</span><span class="sxs-lookup"><span data-stu-id="ccec6-123">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="ccec6-124">通过发布到 **users** 导航属性，为学校添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="ccec6-124">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="ccec6-125">List users</span><span class="sxs-lookup"><span data-stu-id="ccec6-125">List users</span></span>](../api/educationschool-list-users.md)       | <span data-ttu-id="ccec6-126">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ccec6-126">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="ccec6-127">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ccec6-127">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="ccec6-128">Remove user</span><span class="sxs-lookup"><span data-stu-id="ccec6-128">Remove user</span></span>](../api/educationschool-delete-users.md)    | [<span data-ttu-id="ccec6-129">educationUser</span><span class="sxs-lookup"><span data-stu-id="ccec6-129">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="ccec6-130">通过 **users** 导航属性从学校删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="ccec6-130">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="ccec6-131">Update</span><span class="sxs-lookup"><span data-stu-id="ccec6-131">Update</span></span>](../api/educationschool-update.md)               | [<span data-ttu-id="ccec6-132">educationSchool</span><span class="sxs-lookup"><span data-stu-id="ccec6-132">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="ccec6-133">更新 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="ccec6-133">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="ccec6-134">删除</span><span class="sxs-lookup"><span data-stu-id="ccec6-134">Delete</span></span>](../api/educationschool-delete.md)               | <span data-ttu-id="ccec6-135">无</span><span class="sxs-lookup"><span data-stu-id="ccec6-135">None</span></span>                                           | <span data-ttu-id="ccec6-136">删除 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="ccec6-136">Delete an **educationSchool** object.</span></span>                                                       |

## <a name="properties"></a><span data-ttu-id="ccec6-137">属性</span><span class="sxs-lookup"><span data-stu-id="ccec6-137">Properties</span></span>

| <span data-ttu-id="ccec6-138">属性</span><span class="sxs-lookup"><span data-stu-id="ccec6-138">Property</span></span>            | <span data-ttu-id="ccec6-139">类型</span><span class="sxs-lookup"><span data-stu-id="ccec6-139">Type</span></span>                                  | <span data-ttu-id="ccec6-140">说明</span><span class="sxs-lookup"><span data-stu-id="ccec6-140">Description</span></span>                                                                        |
| :------------------ | :------------------------------------ | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="ccec6-141">id</span><span class="sxs-lookup"><span data-stu-id="ccec6-141">id</span></span>                  | <span data-ttu-id="ccec6-142">String</span><span class="sxs-lookup"><span data-stu-id="ccec6-142">String</span></span>                                | <span data-ttu-id="ccec6-143">该学校的 GUID。</span><span class="sxs-lookup"><span data-stu-id="ccec6-143">GUID of this school.</span></span>                                                               |
| <span data-ttu-id="ccec6-144">displayName</span><span class="sxs-lookup"><span data-stu-id="ccec6-144">displayName</span></span>         | <span data-ttu-id="ccec6-145">字符串</span><span class="sxs-lookup"><span data-stu-id="ccec6-145">String</span></span>                                | <span data-ttu-id="ccec6-146">学校的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ccec6-146">Display name of the school.</span></span>                                                        |
| <span data-ttu-id="ccec6-147">说明</span><span class="sxs-lookup"><span data-stu-id="ccec6-147">description</span></span>         | <span data-ttu-id="ccec6-148">字符串</span><span class="sxs-lookup"><span data-stu-id="ccec6-148">String</span></span>                                | <span data-ttu-id="ccec6-149">学校描述。</span><span class="sxs-lookup"><span data-stu-id="ccec6-149">Description of the school.</span></span>                                                         |
| <span data-ttu-id="ccec6-150">状态</span><span class="sxs-lookup"><span data-stu-id="ccec6-150">status</span></span>              | <span data-ttu-id="ccec6-151">string</span><span class="sxs-lookup"><span data-stu-id="ccec6-151">string</span></span>                                | <span data-ttu-id="ccec6-152">只读。</span><span class="sxs-lookup"><span data-stu-id="ccec6-152">Read-Only.</span></span> <span data-ttu-id="ccec6-153">可能的值包括 `inactive`、`active`、`expired`、`deleteable`。</span><span class="sxs-lookup"><span data-stu-id="ccec6-153">The possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span> |
| <span data-ttu-id="ccec6-154">externalSource</span><span class="sxs-lookup"><span data-stu-id="ccec6-154">externalSource</span></span>      | <span data-ttu-id="ccec6-155">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="ccec6-155">educationExternalSource</span></span>               | <span data-ttu-id="ccec6-156">只读。</span><span class="sxs-lookup"><span data-stu-id="ccec6-156">Read-Only.</span></span>  <span data-ttu-id="ccec6-157">可能的值包括 `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="ccec6-157">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>        |
| <span data-ttu-id="ccec6-158">principalEmail</span><span class="sxs-lookup"><span data-stu-id="ccec6-158">principalEmail</span></span>      | <span data-ttu-id="ccec6-159">字符串</span><span class="sxs-lookup"><span data-stu-id="ccec6-159">String</span></span>                                | <span data-ttu-id="ccec6-160">主体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="ccec6-160">Email address of the principal.</span></span>                                                    |
| <span data-ttu-id="ccec6-161">principalName</span><span class="sxs-lookup"><span data-stu-id="ccec6-161">principalName</span></span>       | <span data-ttu-id="ccec6-162">字符串</span><span class="sxs-lookup"><span data-stu-id="ccec6-162">String</span></span>                                | <span data-ttu-id="ccec6-163">主体名称。</span><span class="sxs-lookup"><span data-stu-id="ccec6-163">Name of the principal.</span></span>                                                             |
| <span data-ttu-id="ccec6-164">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="ccec6-164">externalPrincipalId</span></span> | <span data-ttu-id="ccec6-165">字符串</span><span class="sxs-lookup"><span data-stu-id="ccec6-165">String</span></span>                                | <span data-ttu-id="ccec6-166">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="ccec6-166">ID of principal in syncing system.</span></span>                                                 |
| <span data-ttu-id="ccec6-167">highestGrade</span><span class="sxs-lookup"><span data-stu-id="ccec6-167">highestGrade</span></span>        | <span data-ttu-id="ccec6-168">字符串</span><span class="sxs-lookup"><span data-stu-id="ccec6-168">String</span></span>                                | <span data-ttu-id="ccec6-169">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="ccec6-169">Highest grade taught.</span></span>                                                              |
| <span data-ttu-id="ccec6-170">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="ccec6-170">lowestGrade</span></span>         | <span data-ttu-id="ccec6-171">字符串</span><span class="sxs-lookup"><span data-stu-id="ccec6-171">String</span></span>                                | <span data-ttu-id="ccec6-172">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="ccec6-172">Lowest grade taught.</span></span>                                                               |
| <span data-ttu-id="ccec6-173">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="ccec6-173">schoolNumber</span></span>        | <span data-ttu-id="ccec6-174">字符串</span><span class="sxs-lookup"><span data-stu-id="ccec6-174">String</span></span>                                | <span data-ttu-id="ccec6-175">学校编号。</span><span class="sxs-lookup"><span data-stu-id="ccec6-175">School Number.</span></span>                                                                     |
| <span data-ttu-id="ccec6-176">externalId</span><span class="sxs-lookup"><span data-stu-id="ccec6-176">externalId</span></span>          | <span data-ttu-id="ccec6-177">String</span><span class="sxs-lookup"><span data-stu-id="ccec6-177">String</span></span>                                | <span data-ttu-id="ccec6-178">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="ccec6-178">ID of school in syncing system.</span></span>                                                    |
| <span data-ttu-id="ccec6-179">phone</span><span class="sxs-lookup"><span data-stu-id="ccec6-179">phone</span></span>               | <span data-ttu-id="ccec6-180">String</span><span class="sxs-lookup"><span data-stu-id="ccec6-180">String</span></span>                                | <span data-ttu-id="ccec6-181">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="ccec6-181">Phone number of school.</span></span>                                                            |
| <span data-ttu-id="ccec6-182">address</span><span class="sxs-lookup"><span data-stu-id="ccec6-182">address</span></span>             | [<span data-ttu-id="ccec6-183">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="ccec6-183">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="ccec6-184">学校地址。</span><span class="sxs-lookup"><span data-stu-id="ccec6-184">Address of the school.</span></span>                                                             |
| <span data-ttu-id="ccec6-185">createdBy</span><span class="sxs-lookup"><span data-stu-id="ccec6-185">createdBy</span></span>           | [<span data-ttu-id="ccec6-186">identitySet</span><span class="sxs-lookup"><span data-stu-id="ccec6-186">identitySet</span></span>](identityset.md)         | <span data-ttu-id="ccec6-187">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="ccec6-187">Entity who created the school.</span></span>                                                     |

## <a name="relationships"></a><span data-ttu-id="ccec6-188">关系</span><span class="sxs-lookup"><span data-stu-id="ccec6-188">Relationships</span></span>

| <span data-ttu-id="ccec6-189">关系</span><span class="sxs-lookup"><span data-stu-id="ccec6-189">Relationship</span></span> | <span data-ttu-id="ccec6-190">类型</span><span class="sxs-lookup"><span data-stu-id="ccec6-190">Type</span></span>                                           | <span data-ttu-id="ccec6-191">说明</span><span class="sxs-lookup"><span data-stu-id="ccec6-191">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="ccec6-192">classes</span><span class="sxs-lookup"><span data-stu-id="ccec6-192">classes</span></span>      | <span data-ttu-id="ccec6-193">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ccec6-193">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="ccec6-194">在学校教授的课程。</span><span class="sxs-lookup"><span data-stu-id="ccec6-194">Classes taught at the school.</span></span> <span data-ttu-id="ccec6-195">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="ccec6-195">Nullable.</span></span> |
| <span data-ttu-id="ccec6-196">users</span><span class="sxs-lookup"><span data-stu-id="ccec6-196">users</span></span>        | <span data-ttu-id="ccec6-197">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ccec6-197">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="ccec6-198">学校中的用户。</span><span class="sxs-lookup"><span data-stu-id="ccec6-198">Users in the school.</span></span> <span data-ttu-id="ccec6-199">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="ccec6-199">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="ccec6-200">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ccec6-200">JSON representation</span></span>

<span data-ttu-id="ccec6-201">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ccec6-201">The following is a JSON representation of the resource.</span></span>

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
