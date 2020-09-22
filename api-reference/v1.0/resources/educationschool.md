---
title: educationSchool 资源类型
description: '一种表示学校的资源，用于管理所表示学校的课程、教师和学生。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2ed10fd9be0a49fbf25acac635cf29b1759c31eb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032654"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="4fa04-103">educationSchool 资源类型</span><span class="sxs-lookup"><span data-stu-id="4fa04-103">educationSchool resource type</span></span>

<span data-ttu-id="4fa04-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fa04-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4fa04-105">一种表示学校的资源，用于管理所表示学校的课程、教师和学生。</span><span class="sxs-lookup"><span data-stu-id="4fa04-105">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  

## <a name="methods"></a><span data-ttu-id="4fa04-106">方法</span><span class="sxs-lookup"><span data-stu-id="4fa04-106">Methods</span></span>

| <span data-ttu-id="4fa04-107">方法</span><span class="sxs-lookup"><span data-stu-id="4fa04-107">Method</span></span>                                                   | <span data-ttu-id="4fa04-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4fa04-108">Return Type</span></span>                                    | <span data-ttu-id="4fa04-109">说明</span><span class="sxs-lookup"><span data-stu-id="4fa04-109">Description</span></span>                                                                                 |
| :------------------------------------------------------- | :--------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="4fa04-110">获取</span><span class="sxs-lookup"><span data-stu-id="4fa04-110">Get</span></span>](../api/educationschool-get.md)                     | [<span data-ttu-id="4fa04-111">educationSchool</span><span class="sxs-lookup"><span data-stu-id="4fa04-111">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="4fa04-112">读取 **educationSchool** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4fa04-112">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="4fa04-113">Add class</span><span class="sxs-lookup"><span data-stu-id="4fa04-113">Add class</span></span>](../api/educationschool-post-classes.md)      | [<span data-ttu-id="4fa04-114">educationClass</span><span class="sxs-lookup"><span data-stu-id="4fa04-114">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="4fa04-115">通过发布到课程导航属性，为学校添加一个新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="4fa04-115">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="4fa04-116">List classes</span><span class="sxs-lookup"><span data-stu-id="4fa04-116">List classes</span></span>](../api/educationschool-list-classes.md)   | <span data-ttu-id="4fa04-117">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4fa04-117">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="4fa04-118">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4fa04-118">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="4fa04-119">Remove class</span><span class="sxs-lookup"><span data-stu-id="4fa04-119">Remove class</span></span>](../api/educationschool-delete-classes.md) | [<span data-ttu-id="4fa04-120">educationClass</span><span class="sxs-lookup"><span data-stu-id="4fa04-120">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="4fa04-121">通过课程导航属性从学校删除 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="4fa04-121">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="4fa04-122">Add user</span><span class="sxs-lookup"><span data-stu-id="4fa04-122">Add user</span></span>](../api/educationschool-post-users.md)         | [<span data-ttu-id="4fa04-123">educationUser</span><span class="sxs-lookup"><span data-stu-id="4fa04-123">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="4fa04-124">通过发布到 **users** 导航属性，为学校添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="4fa04-124">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="4fa04-125">List users</span><span class="sxs-lookup"><span data-stu-id="4fa04-125">List users</span></span>](../api/educationschool-list-users.md)       | <span data-ttu-id="4fa04-126">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4fa04-126">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="4fa04-127">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4fa04-127">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="4fa04-128">Remove user</span><span class="sxs-lookup"><span data-stu-id="4fa04-128">Remove user</span></span>](../api/educationschool-delete-users.md)    | [<span data-ttu-id="4fa04-129">educationUser</span><span class="sxs-lookup"><span data-stu-id="4fa04-129">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="4fa04-130">通过 **users** 导航属性从学校删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="4fa04-130">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="4fa04-131">Update</span><span class="sxs-lookup"><span data-stu-id="4fa04-131">Update</span></span>](../api/educationschool-update.md)               | [<span data-ttu-id="4fa04-132">educationSchool</span><span class="sxs-lookup"><span data-stu-id="4fa04-132">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="4fa04-133">更新 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="4fa04-133">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="4fa04-134">删除</span><span class="sxs-lookup"><span data-stu-id="4fa04-134">Delete</span></span>](../api/educationschool-delete.md)               | <span data-ttu-id="4fa04-135">无</span><span class="sxs-lookup"><span data-stu-id="4fa04-135">None</span></span>                                           | <span data-ttu-id="4fa04-136">删除 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="4fa04-136">Delete an **educationSchool** object.</span></span>                                                       |

## <a name="properties"></a><span data-ttu-id="4fa04-137">属性</span><span class="sxs-lookup"><span data-stu-id="4fa04-137">Properties</span></span>

| <span data-ttu-id="4fa04-138">属性</span><span class="sxs-lookup"><span data-stu-id="4fa04-138">Property</span></span>            | <span data-ttu-id="4fa04-139">类型</span><span class="sxs-lookup"><span data-stu-id="4fa04-139">Type</span></span>                                  | <span data-ttu-id="4fa04-140">说明</span><span class="sxs-lookup"><span data-stu-id="4fa04-140">Description</span></span>                                                                        |
| :------------------ | :------------------------------------ | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="4fa04-141">id</span><span class="sxs-lookup"><span data-stu-id="4fa04-141">id</span></span>                  | <span data-ttu-id="4fa04-142">String</span><span class="sxs-lookup"><span data-stu-id="4fa04-142">String</span></span>                                | <span data-ttu-id="4fa04-143">该学校的 GUID。</span><span class="sxs-lookup"><span data-stu-id="4fa04-143">GUID of this school.</span></span>                                                               |
| <span data-ttu-id="4fa04-144">displayName</span><span class="sxs-lookup"><span data-stu-id="4fa04-144">displayName</span></span>         | <span data-ttu-id="4fa04-145">String</span><span class="sxs-lookup"><span data-stu-id="4fa04-145">String</span></span>                                | <span data-ttu-id="4fa04-146">学校的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4fa04-146">Display name of the school.</span></span>                                                        |
| <span data-ttu-id="4fa04-147">description</span><span class="sxs-lookup"><span data-stu-id="4fa04-147">description</span></span>         | <span data-ttu-id="4fa04-148">String</span><span class="sxs-lookup"><span data-stu-id="4fa04-148">String</span></span>                                | <span data-ttu-id="4fa04-149">学校描述。</span><span class="sxs-lookup"><span data-stu-id="4fa04-149">Description of the school.</span></span>                                                         |
| <span data-ttu-id="4fa04-150">状态</span><span class="sxs-lookup"><span data-stu-id="4fa04-150">status</span></span>              | <span data-ttu-id="4fa04-151">string</span><span class="sxs-lookup"><span data-stu-id="4fa04-151">string</span></span>                                | <span data-ttu-id="4fa04-152">只读。</span><span class="sxs-lookup"><span data-stu-id="4fa04-152">Read-Only.</span></span> <span data-ttu-id="4fa04-153">可能的值包括 `inactive`、`active`、`expired`、`deleteable`。</span><span class="sxs-lookup"><span data-stu-id="4fa04-153">The possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span> |
| <span data-ttu-id="4fa04-154">externalSource</span><span class="sxs-lookup"><span data-stu-id="4fa04-154">externalSource</span></span>      | <span data-ttu-id="4fa04-155">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="4fa04-155">educationExternalSource</span></span>               | <span data-ttu-id="4fa04-156">只读。</span><span class="sxs-lookup"><span data-stu-id="4fa04-156">Read-Only.</span></span>  <span data-ttu-id="4fa04-157">可能的值包括 `sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="4fa04-157">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>        |
| <span data-ttu-id="4fa04-158">principalEmail</span><span class="sxs-lookup"><span data-stu-id="4fa04-158">principalEmail</span></span>      | <span data-ttu-id="4fa04-159">String</span><span class="sxs-lookup"><span data-stu-id="4fa04-159">String</span></span>                                | <span data-ttu-id="4fa04-160">主体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="4fa04-160">Email address of the principal.</span></span>                                                    |
| <span data-ttu-id="4fa04-161">principalName</span><span class="sxs-lookup"><span data-stu-id="4fa04-161">principalName</span></span>       | <span data-ttu-id="4fa04-162">String</span><span class="sxs-lookup"><span data-stu-id="4fa04-162">String</span></span>                                | <span data-ttu-id="4fa04-163">主体名称。</span><span class="sxs-lookup"><span data-stu-id="4fa04-163">Name of the principal.</span></span>                                                             |
| <span data-ttu-id="4fa04-164">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="4fa04-164">externalPrincipalId</span></span> | <span data-ttu-id="4fa04-165">String</span><span class="sxs-lookup"><span data-stu-id="4fa04-165">String</span></span>                                | <span data-ttu-id="4fa04-166">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="4fa04-166">ID of principal in syncing system.</span></span>                                                 |
| <span data-ttu-id="4fa04-167">highestGrade</span><span class="sxs-lookup"><span data-stu-id="4fa04-167">highestGrade</span></span>        | <span data-ttu-id="4fa04-168">String</span><span class="sxs-lookup"><span data-stu-id="4fa04-168">String</span></span>                                | <span data-ttu-id="4fa04-169">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="4fa04-169">Highest grade taught.</span></span>                                                              |
| <span data-ttu-id="4fa04-170">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="4fa04-170">lowestGrade</span></span>         | <span data-ttu-id="4fa04-171">String</span><span class="sxs-lookup"><span data-stu-id="4fa04-171">String</span></span>                                | <span data-ttu-id="4fa04-172">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="4fa04-172">Lowest grade taught.</span></span>                                                               |
| <span data-ttu-id="4fa04-173">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="4fa04-173">schoolNumber</span></span>        | <span data-ttu-id="4fa04-174">String</span><span class="sxs-lookup"><span data-stu-id="4fa04-174">String</span></span>                                | <span data-ttu-id="4fa04-175">学校编号。</span><span class="sxs-lookup"><span data-stu-id="4fa04-175">School Number.</span></span>                                                                     |
| <span data-ttu-id="4fa04-176">externalId</span><span class="sxs-lookup"><span data-stu-id="4fa04-176">externalId</span></span>          | <span data-ttu-id="4fa04-177">String</span><span class="sxs-lookup"><span data-stu-id="4fa04-177">String</span></span>                                | <span data-ttu-id="4fa04-178">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="4fa04-178">ID of school in syncing system.</span></span>                                                    |
| <span data-ttu-id="4fa04-179">phone</span><span class="sxs-lookup"><span data-stu-id="4fa04-179">phone</span></span>               | <span data-ttu-id="4fa04-180">String</span><span class="sxs-lookup"><span data-stu-id="4fa04-180">String</span></span>                                | <span data-ttu-id="4fa04-181">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="4fa04-181">Phone number of school.</span></span>                                                            |
| <span data-ttu-id="4fa04-182">address</span><span class="sxs-lookup"><span data-stu-id="4fa04-182">address</span></span>             | [<span data-ttu-id="4fa04-183">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="4fa04-183">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="4fa04-184">学校地址。</span><span class="sxs-lookup"><span data-stu-id="4fa04-184">Address of the school.</span></span>                                                             |
| <span data-ttu-id="4fa04-185">createdBy</span><span class="sxs-lookup"><span data-stu-id="4fa04-185">createdBy</span></span>           | [<span data-ttu-id="4fa04-186">identitySet</span><span class="sxs-lookup"><span data-stu-id="4fa04-186">identitySet</span></span>](identityset.md)         | <span data-ttu-id="4fa04-187">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="4fa04-187">Entity who created the school.</span></span>                                                     |

## <a name="relationships"></a><span data-ttu-id="4fa04-188">关系</span><span class="sxs-lookup"><span data-stu-id="4fa04-188">Relationships</span></span>

| <span data-ttu-id="4fa04-189">关系</span><span class="sxs-lookup"><span data-stu-id="4fa04-189">Relationship</span></span> | <span data-ttu-id="4fa04-190">类型</span><span class="sxs-lookup"><span data-stu-id="4fa04-190">Type</span></span>                                           | <span data-ttu-id="4fa04-191">说明</span><span class="sxs-lookup"><span data-stu-id="4fa04-191">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="4fa04-192">classes</span><span class="sxs-lookup"><span data-stu-id="4fa04-192">classes</span></span>      | <span data-ttu-id="4fa04-193">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4fa04-193">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="4fa04-194">在学校教授的课程。</span><span class="sxs-lookup"><span data-stu-id="4fa04-194">Classes taught at the school.</span></span> <span data-ttu-id="4fa04-195">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="4fa04-195">Nullable.</span></span> |
| <span data-ttu-id="4fa04-196">users</span><span class="sxs-lookup"><span data-stu-id="4fa04-196">users</span></span>        | <span data-ttu-id="4fa04-197">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4fa04-197">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="4fa04-198">学校中的用户。</span><span class="sxs-lookup"><span data-stu-id="4fa04-198">Users in the school.</span></span> <span data-ttu-id="4fa04-199">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="4fa04-199">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="4fa04-200">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4fa04-200">JSON representation</span></span>

<span data-ttu-id="4fa04-201">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4fa04-201">The following is a JSON representation of the resource.</span></span>

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

