---
title: educationSchool 资源类型
description: '一种表示学校的资源，用于管理所表示学校的课程、教师和学生。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d7cc20b01b35f678b20e18e21dcb099a89982ab9
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37553906"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="460ed-103">educationSchool 资源类型</span><span class="sxs-lookup"><span data-stu-id="460ed-103">educationSchool resource type</span></span>

<span data-ttu-id="460ed-104">一种表示学校的资源，用于管理所表示学校的课程、教师和学生。</span><span class="sxs-lookup"><span data-stu-id="460ed-104">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  

## <a name="methods"></a><span data-ttu-id="460ed-105">方法</span><span class="sxs-lookup"><span data-stu-id="460ed-105">Methods</span></span>

| <span data-ttu-id="460ed-106">方法</span><span class="sxs-lookup"><span data-stu-id="460ed-106">Method</span></span>                                                   | <span data-ttu-id="460ed-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="460ed-107">Return Type</span></span>                                    | <span data-ttu-id="460ed-108">说明</span><span class="sxs-lookup"><span data-stu-id="460ed-108">Description</span></span>                                                                                 |
| :------------------------------------------------------- | :--------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="460ed-109">Get</span><span class="sxs-lookup"><span data-stu-id="460ed-109">Get</span></span>](../api/educationschool-get.md)                     | [<span data-ttu-id="460ed-110">educationSchool</span><span class="sxs-lookup"><span data-stu-id="460ed-110">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="460ed-111">读取 **educationSchool** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="460ed-111">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="460ed-112">Add class</span><span class="sxs-lookup"><span data-stu-id="460ed-112">Add class</span></span>](../api/educationschool-post-classes.md)      | [<span data-ttu-id="460ed-113">educationClass</span><span class="sxs-lookup"><span data-stu-id="460ed-113">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="460ed-114">通过发布到课程导航属性，为学校添加一个新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="460ed-114">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="460ed-115">List classes</span><span class="sxs-lookup"><span data-stu-id="460ed-115">List classes</span></span>](../api/educationschool-list-classes.md)   | <span data-ttu-id="460ed-116">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="460ed-116">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="460ed-117">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="460ed-117">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="460ed-118">Remove class</span><span class="sxs-lookup"><span data-stu-id="460ed-118">Remove class</span></span>](../api/educationschool-delete-classes.md) | [<span data-ttu-id="460ed-119">educationClass</span><span class="sxs-lookup"><span data-stu-id="460ed-119">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="460ed-120">通过课程导航属性从学校删除 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="460ed-120">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="460ed-121">Add user</span><span class="sxs-lookup"><span data-stu-id="460ed-121">Add user</span></span>](../api/educationschool-post-users.md)         | [<span data-ttu-id="460ed-122">educationUser</span><span class="sxs-lookup"><span data-stu-id="460ed-122">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="460ed-123">通过发布到 **users** 导航属性，为学校添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="460ed-123">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="460ed-124">List users</span><span class="sxs-lookup"><span data-stu-id="460ed-124">List users</span></span>](../api/educationschool-list-users.md)       | <span data-ttu-id="460ed-125">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="460ed-125">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="460ed-126">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="460ed-126">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="460ed-127">Remove user</span><span class="sxs-lookup"><span data-stu-id="460ed-127">Remove user</span></span>](../api/educationschool-delete-users.md)    | [<span data-ttu-id="460ed-128">educationUser</span><span class="sxs-lookup"><span data-stu-id="460ed-128">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="460ed-129">通过 **users** 导航属性从学校删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="460ed-129">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="460ed-130">Update</span><span class="sxs-lookup"><span data-stu-id="460ed-130">Update</span></span>](../api/educationschool-update.md)               | [<span data-ttu-id="460ed-131">educationSchool</span><span class="sxs-lookup"><span data-stu-id="460ed-131">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="460ed-132">更新 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="460ed-132">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="460ed-133">删除</span><span class="sxs-lookup"><span data-stu-id="460ed-133">Delete</span></span>](../api/educationschool-delete.md)               | <span data-ttu-id="460ed-134">无</span><span class="sxs-lookup"><span data-stu-id="460ed-134">None</span></span>                                           | <span data-ttu-id="460ed-135">删除 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="460ed-135">Delete an **educationSchool** object.</span></span>                                                       |

## <a name="properties"></a><span data-ttu-id="460ed-136">属性</span><span class="sxs-lookup"><span data-stu-id="460ed-136">Properties</span></span>

| <span data-ttu-id="460ed-137">属性</span><span class="sxs-lookup"><span data-stu-id="460ed-137">Property</span></span>            | <span data-ttu-id="460ed-138">类型</span><span class="sxs-lookup"><span data-stu-id="460ed-138">Type</span></span>                                  | <span data-ttu-id="460ed-139">说明</span><span class="sxs-lookup"><span data-stu-id="460ed-139">Description</span></span>                                                                        |
| :------------------ | :------------------------------------ | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="460ed-140">id</span><span class="sxs-lookup"><span data-stu-id="460ed-140">id</span></span>                  | <span data-ttu-id="460ed-141">String</span><span class="sxs-lookup"><span data-stu-id="460ed-141">String</span></span>                                | <span data-ttu-id="460ed-142">该学校的 GUID。</span><span class="sxs-lookup"><span data-stu-id="460ed-142">GUID of this school.</span></span>                                                               |
| <span data-ttu-id="460ed-143">displayName</span><span class="sxs-lookup"><span data-stu-id="460ed-143">displayName</span></span>         | <span data-ttu-id="460ed-144">String</span><span class="sxs-lookup"><span data-stu-id="460ed-144">String</span></span>                                | <span data-ttu-id="460ed-145">学校的显示名称。</span><span class="sxs-lookup"><span data-stu-id="460ed-145">Display name of the school.</span></span>                                                        |
| <span data-ttu-id="460ed-146">说明</span><span class="sxs-lookup"><span data-stu-id="460ed-146">description</span></span>         | <span data-ttu-id="460ed-147">字符串</span><span class="sxs-lookup"><span data-stu-id="460ed-147">String</span></span>                                | <span data-ttu-id="460ed-148">学校描述。</span><span class="sxs-lookup"><span data-stu-id="460ed-148">Description of the school.</span></span>                                                         |
| <span data-ttu-id="460ed-149">状态</span><span class="sxs-lookup"><span data-stu-id="460ed-149">status</span></span>              | <span data-ttu-id="460ed-150">string</span><span class="sxs-lookup"><span data-stu-id="460ed-150">string</span></span>                                | <span data-ttu-id="460ed-151">只读。</span><span class="sxs-lookup"><span data-stu-id="460ed-151">Read-Only.</span></span> <span data-ttu-id="460ed-152">可能的值包括 `inactive`、`active`、`expired`、`deleteable`。</span><span class="sxs-lookup"><span data-stu-id="460ed-152">The possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span> |
| <span data-ttu-id="460ed-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="460ed-153">externalSource</span></span>      | <span data-ttu-id="460ed-154">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="460ed-154">educationExternalSource</span></span>               | <span data-ttu-id="460ed-155">只读。</span><span class="sxs-lookup"><span data-stu-id="460ed-155">Read-Only.</span></span>  <span data-ttu-id="460ed-156">可能的值包括 `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="460ed-156">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>        |
| <span data-ttu-id="460ed-157">principalEmail</span><span class="sxs-lookup"><span data-stu-id="460ed-157">principalEmail</span></span>      | <span data-ttu-id="460ed-158">String</span><span class="sxs-lookup"><span data-stu-id="460ed-158">String</span></span>                                | <span data-ttu-id="460ed-159">主体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="460ed-159">Email address of the principal.</span></span>                                                    |
| <span data-ttu-id="460ed-160">principalName</span><span class="sxs-lookup"><span data-stu-id="460ed-160">principalName</span></span>       | <span data-ttu-id="460ed-161">String</span><span class="sxs-lookup"><span data-stu-id="460ed-161">String</span></span>                                | <span data-ttu-id="460ed-162">主体名称。</span><span class="sxs-lookup"><span data-stu-id="460ed-162">Name of the principal.</span></span>                                                             |
| <span data-ttu-id="460ed-163">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="460ed-163">externalPrincipalId</span></span> | <span data-ttu-id="460ed-164">String</span><span class="sxs-lookup"><span data-stu-id="460ed-164">String</span></span>                                | <span data-ttu-id="460ed-165">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="460ed-165">ID of principal in syncing system.</span></span>                                                 |
| <span data-ttu-id="460ed-166">highestGrade</span><span class="sxs-lookup"><span data-stu-id="460ed-166">highestGrade</span></span>        | <span data-ttu-id="460ed-167">String</span><span class="sxs-lookup"><span data-stu-id="460ed-167">String</span></span>                                | <span data-ttu-id="460ed-168">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="460ed-168">Highest grade taught.</span></span>                                                              |
| <span data-ttu-id="460ed-169">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="460ed-169">lowestGrade</span></span>         | <span data-ttu-id="460ed-170">String</span><span class="sxs-lookup"><span data-stu-id="460ed-170">String</span></span>                                | <span data-ttu-id="460ed-171">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="460ed-171">Lowest grade taught.</span></span>                                                               |
| <span data-ttu-id="460ed-172">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="460ed-172">schoolNumber</span></span>        | <span data-ttu-id="460ed-173">String</span><span class="sxs-lookup"><span data-stu-id="460ed-173">String</span></span>                                | <span data-ttu-id="460ed-174">学校编号。</span><span class="sxs-lookup"><span data-stu-id="460ed-174">School Number.</span></span>                                                                     |
| <span data-ttu-id="460ed-175">externalId</span><span class="sxs-lookup"><span data-stu-id="460ed-175">externalId</span></span>          | <span data-ttu-id="460ed-176">String</span><span class="sxs-lookup"><span data-stu-id="460ed-176">String</span></span>                                | <span data-ttu-id="460ed-177">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="460ed-177">ID of school in syncing system.</span></span>                                                    |
| <span data-ttu-id="460ed-178">phone</span><span class="sxs-lookup"><span data-stu-id="460ed-178">phone</span></span>               | <span data-ttu-id="460ed-179">String</span><span class="sxs-lookup"><span data-stu-id="460ed-179">String</span></span>                                | <span data-ttu-id="460ed-180">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="460ed-180">Phone number of school.</span></span>                                                            |
| <span data-ttu-id="460ed-181">address</span><span class="sxs-lookup"><span data-stu-id="460ed-181">address</span></span>             | [<span data-ttu-id="460ed-182">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="460ed-182">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="460ed-183">学校地址。</span><span class="sxs-lookup"><span data-stu-id="460ed-183">Address of the school.</span></span>                                                             |
| <span data-ttu-id="460ed-184">createdBy</span><span class="sxs-lookup"><span data-stu-id="460ed-184">createdBy</span></span>           | [<span data-ttu-id="460ed-185">identitySet</span><span class="sxs-lookup"><span data-stu-id="460ed-185">identitySet</span></span>](identityset.md)         | <span data-ttu-id="460ed-186">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="460ed-186">Entity who created the school.</span></span>                                                     |

## <a name="relationships"></a><span data-ttu-id="460ed-187">关系</span><span class="sxs-lookup"><span data-stu-id="460ed-187">Relationships</span></span>

| <span data-ttu-id="460ed-188">关系</span><span class="sxs-lookup"><span data-stu-id="460ed-188">Relationship</span></span> | <span data-ttu-id="460ed-189">类型</span><span class="sxs-lookup"><span data-stu-id="460ed-189">Type</span></span>                                           | <span data-ttu-id="460ed-190">说明</span><span class="sxs-lookup"><span data-stu-id="460ed-190">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="460ed-191">classes</span><span class="sxs-lookup"><span data-stu-id="460ed-191">classes</span></span>      | <span data-ttu-id="460ed-192">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="460ed-192">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="460ed-193">在学校教授的课程。</span><span class="sxs-lookup"><span data-stu-id="460ed-193">Classes taught at the school.</span></span> <span data-ttu-id="460ed-194">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="460ed-194">Nullable.</span></span> |
| <span data-ttu-id="460ed-195">users</span><span class="sxs-lookup"><span data-stu-id="460ed-195">users</span></span>        | <span data-ttu-id="460ed-196">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="460ed-196">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="460ed-197">学校中的用户。</span><span class="sxs-lookup"><span data-stu-id="460ed-197">Users in the school.</span></span> <span data-ttu-id="460ed-198">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="460ed-198">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="460ed-199">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="460ed-199">JSON representation</span></span>

<span data-ttu-id="460ed-200">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="460ed-200">The following is a JSON representation of the resource.</span></span>

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
