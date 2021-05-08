---
title: educationClass 资源类型
description: '表示学校的课程。 **educationClass** 资源对应于 Microsoft 365 组并共享同一 ID。 学生是课程的正式成员，教师为所有者，且具有相应权限。 若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。  '
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 528ea878ad5ed507c83a750d617209b4cde3d589
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231516"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="7795d-106">educationClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="7795d-106">educationClass resource type</span></span>

<span data-ttu-id="7795d-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7795d-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7795d-108">表示学校的课程。</span><span class="sxs-lookup"><span data-stu-id="7795d-108">Represents a class within a school.</span></span> <span data-ttu-id="7795d-109">**educationClass** 资源对应于 Microsoft 365 组并共享同一 ID。</span><span class="sxs-lookup"><span data-stu-id="7795d-109">The **educationClass** resource corresponds to the Microsoft 365 group and shares the same ID.</span></span> <span data-ttu-id="7795d-110">学生是课程的正式成员，教师为所有者，且具有相应权限。</span><span class="sxs-lookup"><span data-stu-id="7795d-110">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="7795d-111">若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。</span><span class="sxs-lookup"><span data-stu-id="7795d-111">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>

<span data-ttu-id="7795d-112">继承自 [实体](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="7795d-112">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="7795d-113">方法</span><span class="sxs-lookup"><span data-stu-id="7795d-113">Methods</span></span>

| <span data-ttu-id="7795d-114">方法</span><span class="sxs-lookup"><span data-stu-id="7795d-114">Method</span></span>                                                   | <span data-ttu-id="7795d-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="7795d-115">Return type</span></span>                                                 | <span data-ttu-id="7795d-116">说明</span><span class="sxs-lookup"><span data-stu-id="7795d-116">Description</span></span>                                                                                          |
| :------------------------------------------------------- | :---------------------------------------------------------- | :--------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="7795d-117">列出 educationClasses</span><span class="sxs-lookup"><span data-stu-id="7795d-117">List educationClasses</span></span>](../api/educationclass-list.md)   | <span data-ttu-id="7795d-118">[educationClass](../resources/educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7795d-118">[educationClass](../resources/educationclass.md) collection</span></span> | <span data-ttu-id="7795d-119">获取 [educationClass 对象](../resources/educationclass.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="7795d-119">Get a list of the [educationClass](../resources/educationclass.md) objects and their properties.</span></span>     |
| [<span data-ttu-id="7795d-120">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="7795d-120">Create educationClass</span></span>](../api/educationclass-post.md) | [<span data-ttu-id="7795d-121">educationClass</span><span class="sxs-lookup"><span data-stu-id="7795d-121">educationClass</span></span>](../resources/educationclass.md)            | <span data-ttu-id="7795d-122">创建新的 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7795d-122">Create a new [educationClass](../resources/educationclass.md) object.</span></span>                                |
| [<span data-ttu-id="7795d-123">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="7795d-123">Get educationClass</span></span>](../api/educationclass-get.md)       | [<span data-ttu-id="7795d-124">educationClass</span><span class="sxs-lookup"><span data-stu-id="7795d-124">educationClass</span></span>](../resources/educationclass.md)            | <span data-ttu-id="7795d-125">读取 [educationClass](../resources/educationclass.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7795d-125">Read the properties and relationships of an [educationClass](../resources/educationclass.md) object.</span></span> |
| [<span data-ttu-id="7795d-126">更新 educationClass</span><span class="sxs-lookup"><span data-stu-id="7795d-126">Update educationClass</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="7795d-127">educationClass</span><span class="sxs-lookup"><span data-stu-id="7795d-127">educationClass</span></span>](../resources/educationclass.md)            | <span data-ttu-id="7795d-128">更新 [educationClass 对象](../resources/educationclass.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="7795d-128">Update the properties of an [educationClass](../resources/educationclass.md) object.</span></span>                 |
| [<span data-ttu-id="7795d-129">删除 educationClass</span><span class="sxs-lookup"><span data-stu-id="7795d-129">Delete educationClass</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="7795d-130">无</span><span class="sxs-lookup"><span data-stu-id="7795d-130">None</span></span>                                                        | <span data-ttu-id="7795d-131">删除 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7795d-131">Delete an [educationClass](../resources/educationclass.md) object.</span></span>                                  |
| [<span data-ttu-id="7795d-132">增量</span><span class="sxs-lookup"><span data-stu-id="7795d-132">delta</span></span>](../api/educationclass-delta.md)                  | <span data-ttu-id="7795d-133">[educationClass](../resources/educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7795d-133">[educationClass](../resources/educationclass.md) collection</span></span> | <span data-ttu-id="7795d-134">获取资源集合的增量更改。</span><span class="sxs-lookup"><span data-stu-id="7795d-134">Get incremental changes to the resource collection.</span></span>                                                  |

## <a name="properties"></a><span data-ttu-id="7795d-135">属性</span><span class="sxs-lookup"><span data-stu-id="7795d-135">Properties</span></span>

| <span data-ttu-id="7795d-136">属性</span><span class="sxs-lookup"><span data-stu-id="7795d-136">Property</span></span>             | <span data-ttu-id="7795d-137">类型</span><span class="sxs-lookup"><span data-stu-id="7795d-137">Type</span></span>                                           | <span data-ttu-id="7795d-138">说明</span><span class="sxs-lookup"><span data-stu-id="7795d-138">Description</span></span>                                                        |
| :------------------- | :--------------------------------------------- | :----------------------------------------------------------------- |
| <span data-ttu-id="7795d-139">id</span><span class="sxs-lookup"><span data-stu-id="7795d-139">id</span></span>                   | <span data-ttu-id="7795d-140">String</span><span class="sxs-lookup"><span data-stu-id="7795d-140">String</span></span>                                         | <span data-ttu-id="7795d-141">对象标识符。</span><span class="sxs-lookup"><span data-stu-id="7795d-141">Object identifier.</span></span> <span data-ttu-id="7795d-142">继承自 [实体](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="7795d-142">Inherited from [entity](../resources/entity.md).</span></span> |
| <span data-ttu-id="7795d-143">displayName</span><span class="sxs-lookup"><span data-stu-id="7795d-143">displayName</span></span>          | <span data-ttu-id="7795d-144">String</span><span class="sxs-lookup"><span data-stu-id="7795d-144">String</span></span>                                         | <span data-ttu-id="7795d-145">课程名称。</span><span class="sxs-lookup"><span data-stu-id="7795d-145">Name of the class.</span></span>                                                 |
| <span data-ttu-id="7795d-146">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7795d-146">mailNickname</span></span>         | <span data-ttu-id="7795d-147">String</span><span class="sxs-lookup"><span data-stu-id="7795d-147">String</span></span>                                         | <span data-ttu-id="7795d-148">向所有成员发送电子邮件的邮件名称（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="7795d-148">Mail name for sending email to all members, if this is enabled.</span></span>    |
| <span data-ttu-id="7795d-149">说明</span><span class="sxs-lookup"><span data-stu-id="7795d-149">description</span></span>          | <span data-ttu-id="7795d-150">String</span><span class="sxs-lookup"><span data-stu-id="7795d-150">String</span></span>                                         | <span data-ttu-id="7795d-151">课程说明。</span><span class="sxs-lookup"><span data-stu-id="7795d-151">Description of the class.</span></span>                                          |
| <span data-ttu-id="7795d-152">createdBy</span><span class="sxs-lookup"><span data-stu-id="7795d-152">createdBy</span></span>            | [<span data-ttu-id="7795d-153">identitySet</span><span class="sxs-lookup"><span data-stu-id="7795d-153">identitySet</span></span>](../resources/identityset.md)     | <span data-ttu-id="7795d-154">创建了课程的实体</span><span class="sxs-lookup"><span data-stu-id="7795d-154">Entity who created the class</span></span>                                       |
| <span data-ttu-id="7795d-155">classCode</span><span class="sxs-lookup"><span data-stu-id="7795d-155">classCode</span></span>            | <span data-ttu-id="7795d-156">String</span><span class="sxs-lookup"><span data-stu-id="7795d-156">String</span></span>                                         | <span data-ttu-id="7795d-157">学校用于标识课程的课程代码。</span><span class="sxs-lookup"><span data-stu-id="7795d-157">Class code used by the school to identify the class.</span></span>               |
| <span data-ttu-id="7795d-158">externalName</span><span class="sxs-lookup"><span data-stu-id="7795d-158">externalName</span></span>         | <span data-ttu-id="7795d-159">String</span><span class="sxs-lookup"><span data-stu-id="7795d-159">String</span></span>                                         | <span data-ttu-id="7795d-160">同步系统中的课程名称。</span><span class="sxs-lookup"><span data-stu-id="7795d-160">Name of the class in the syncing system.</span></span>                           |
| <span data-ttu-id="7795d-161">externalId</span><span class="sxs-lookup"><span data-stu-id="7795d-161">externalId</span></span>           | <span data-ttu-id="7795d-162">String</span><span class="sxs-lookup"><span data-stu-id="7795d-162">String</span></span>                                         | <span data-ttu-id="7795d-163">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="7795d-163">ID of the class from the syncing system.</span></span>                           |
| <span data-ttu-id="7795d-164">externalSource</span><span class="sxs-lookup"><span data-stu-id="7795d-164">externalSource</span></span>       | <span data-ttu-id="7795d-165">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="7795d-165">educationExternalSource</span></span>                        | <span data-ttu-id="7795d-166">此课程的创建方式。</span><span class="sxs-lookup"><span data-stu-id="7795d-166">How this class was created.</span></span> <span data-ttu-id="7795d-167">可取值为：`sis`、`manual`。</span><span class="sxs-lookup"><span data-stu-id="7795d-167">Possible values are: `sis`, `manual`.</span></span>  |
| <span data-ttu-id="7795d-168">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="7795d-168">externalSourceDetail</span></span> | <span data-ttu-id="7795d-169">String</span><span class="sxs-lookup"><span data-stu-id="7795d-169">String</span></span>                                         | <span data-ttu-id="7795d-170">生成此资源的外部源的名称。</span><span class="sxs-lookup"><span data-stu-id="7795d-170">The name of the external source this resources was generated from.</span></span> |
| <span data-ttu-id="7795d-171">grade</span><span class="sxs-lookup"><span data-stu-id="7795d-171">grade</span></span>                | <span data-ttu-id="7795d-172">String</span><span class="sxs-lookup"><span data-stu-id="7795d-172">String</span></span>                                         | <span data-ttu-id="7795d-173">课程的年级。</span><span class="sxs-lookup"><span data-stu-id="7795d-173">Grade level of the class.</span></span>                                          |
| <span data-ttu-id="7795d-174">term</span><span class="sxs-lookup"><span data-stu-id="7795d-174">term</span></span>                 | [<span data-ttu-id="7795d-175">educationTerm</span><span class="sxs-lookup"><span data-stu-id="7795d-175">educationTerm</span></span>](../resources/educationterm.md) | <span data-ttu-id="7795d-176">此课程的学期。</span><span class="sxs-lookup"><span data-stu-id="7795d-176">Term for this class.</span></span>                                               |

## <a name="relationships"></a><span data-ttu-id="7795d-177">关系</span><span class="sxs-lookup"><span data-stu-id="7795d-177">Relationships</span></span>

| <span data-ttu-id="7795d-178">关系</span><span class="sxs-lookup"><span data-stu-id="7795d-178">Relationship</span></span> | <span data-ttu-id="7795d-179">类型</span><span class="sxs-lookup"><span data-stu-id="7795d-179">Type</span></span>                                                          | <span data-ttu-id="7795d-180">说明</span><span class="sxs-lookup"><span data-stu-id="7795d-180">Description</span></span>                                               |
| :----------- | :------------------------------------------------------------ | :-------------------------------------------------------- |
| <span data-ttu-id="7795d-181">group</span><span class="sxs-lookup"><span data-stu-id="7795d-181">group</span></span>        | [<span data-ttu-id="7795d-182">组</span><span class="sxs-lookup"><span data-stu-id="7795d-182">group</span></span>](../resources/group.md)                                | <span data-ttu-id="7795d-183">组Microsoft 365对象。</span><span class="sxs-lookup"><span data-stu-id="7795d-183">The underlying Microsoft 365 group object.</span></span>                |
| <span data-ttu-id="7795d-184">members</span><span class="sxs-lookup"><span data-stu-id="7795d-184">members</span></span>      | <span data-ttu-id="7795d-185">[educationUser](../resources/educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7795d-185">[educationUser](../resources/educationuser.md) collection</span></span>     | <span data-ttu-id="7795d-186">课程中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="7795d-186">All users in the class.</span></span> <span data-ttu-id="7795d-187">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="7795d-187">Nullable.</span></span>                         |
| <span data-ttu-id="7795d-188">schools</span><span class="sxs-lookup"><span data-stu-id="7795d-188">schools</span></span>      | <span data-ttu-id="7795d-189">[educationSchool](../resources/educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7795d-189">[educationSchool](../resources/educationschool.md) collection</span></span> | <span data-ttu-id="7795d-190">与此课程相关的所有学校。</span><span class="sxs-lookup"><span data-stu-id="7795d-190">All schools that this class is associated with.</span></span> <span data-ttu-id="7795d-191">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="7795d-191">Nullable.</span></span> |
| <span data-ttu-id="7795d-192">teachers</span><span class="sxs-lookup"><span data-stu-id="7795d-192">teachers</span></span>     | <span data-ttu-id="7795d-193">[educationUser](../resources/educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7795d-193">[educationUser](../resources/educationuser.md) collection</span></span>     | <span data-ttu-id="7795d-194">课程中的所有教师。</span><span class="sxs-lookup"><span data-stu-id="7795d-194">All teachers in the class.</span></span> <span data-ttu-id="7795d-195">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="7795d-195">Nullable.</span></span>                      |

## <a name="json-representation"></a><span data-ttu-id="7795d-196">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7795d-196">JSON representation</span></span>

<span data-ttu-id="7795d-197">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7795d-197">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationClass",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationClass",
  "id": "String (identifier)",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```
