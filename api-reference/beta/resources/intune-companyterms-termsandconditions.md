---
title: termsAndConditions 资源类型
description: TermsAndConditions 实体表示给定条款和条件 (T&C) 策略的元数据和内容。 当用户第一次尝试注册到 Intune 时向用户显示 T&C 策略的内容，之后会在进行了管理员要求重新接受的编辑时显示。 这允许管理员与用户必须同意的预配进行通信，以便将设备注册到 Intune 中。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 470d584257a4c037677e63f7cbac84956fd65f8e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472070"
---
# <a name="termsandconditions-resource-type"></a><span data-ttu-id="8cca6-105">termsAndConditions 资源类型</span><span class="sxs-lookup"><span data-stu-id="8cca6-105">termsAndConditions resource type</span></span>

<span data-ttu-id="8cca6-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cca6-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8cca6-107">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8cca6-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cca6-108">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8cca6-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cca6-109">TermsAndConditions 实体表示给定条款和条件 (T&C) 策略的元数据和内容。</span><span class="sxs-lookup"><span data-stu-id="8cca6-109">A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy.</span></span> <span data-ttu-id="8cca6-110">当用户第一次尝试注册到 Intune 时向用户显示 T&C 策略的内容，之后会在进行了管理员要求重新接受的编辑时显示。</span><span class="sxs-lookup"><span data-stu-id="8cca6-110">T&C policies’ contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance.</span></span> <span data-ttu-id="8cca6-111">这允许管理员与用户必须同意的预配进行通信，以便将设备注册到 Intune 中。</span><span class="sxs-lookup"><span data-stu-id="8cca6-111">They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="8cca6-112">方法</span><span class="sxs-lookup"><span data-stu-id="8cca6-112">Methods</span></span>
|<span data-ttu-id="8cca6-113">方法</span><span class="sxs-lookup"><span data-stu-id="8cca6-113">Method</span></span>|<span data-ttu-id="8cca6-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="8cca6-114">Return Type</span></span>|<span data-ttu-id="8cca6-115">说明</span><span class="sxs-lookup"><span data-stu-id="8cca6-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8cca6-116">List termsAndConditionses</span><span class="sxs-lookup"><span data-stu-id="8cca6-116">List termsAndConditionses</span></span>](../api/intune-companyterms-termsandconditions-list.md)|<span data-ttu-id="8cca6-117">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8cca6-117">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) collection</span></span>|<span data-ttu-id="8cca6-118">列出 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8cca6-118">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>|
|[<span data-ttu-id="8cca6-119">Get termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="8cca6-119">Get termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-get.md)|[<span data-ttu-id="8cca6-120">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="8cca6-120">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="8cca6-121">读取 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8cca6-121">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="8cca6-122">Create termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="8cca6-122">Create termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-create.md)|[<span data-ttu-id="8cca6-123">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="8cca6-123">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="8cca6-124">创建新的 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8cca6-124">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="8cca6-125">Delete termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="8cca6-125">Delete termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-delete.md)|<span data-ttu-id="8cca6-126">无</span><span class="sxs-lookup"><span data-stu-id="8cca6-126">None</span></span>|<span data-ttu-id="8cca6-127">删除 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)。</span><span class="sxs-lookup"><span data-stu-id="8cca6-127">Deletes a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>|
|[<span data-ttu-id="8cca6-128">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="8cca6-128">Update termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-update.md)|[<span data-ttu-id="8cca6-129">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="8cca6-129">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="8cca6-130">更新 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8cca6-130">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8cca6-131">属性</span><span class="sxs-lookup"><span data-stu-id="8cca6-131">Properties</span></span>
|<span data-ttu-id="8cca6-132">属性</span><span class="sxs-lookup"><span data-stu-id="8cca6-132">Property</span></span>|<span data-ttu-id="8cca6-133">类型</span><span class="sxs-lookup"><span data-stu-id="8cca6-133">Type</span></span>|<span data-ttu-id="8cca6-134">说明</span><span class="sxs-lookup"><span data-stu-id="8cca6-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cca6-135">id</span><span class="sxs-lookup"><span data-stu-id="8cca6-135">id</span></span>|<span data-ttu-id="8cca6-136">字符串</span><span class="sxs-lookup"><span data-stu-id="8cca6-136">String</span></span>|<span data-ttu-id="8cca6-137">T&C 策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8cca6-137">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="8cca6-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8cca6-138">createdDateTime</span></span>|<span data-ttu-id="8cca6-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cca6-139">DateTimeOffset</span></span>|<span data-ttu-id="8cca6-140">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8cca6-140">DateTime the object was created.</span></span>|
|<span data-ttu-id="8cca6-141">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8cca6-141">modifiedDateTime</span></span>|<span data-ttu-id="8cca6-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cca6-142">DateTimeOffset</span></span>|<span data-ttu-id="8cca6-143">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8cca6-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="8cca6-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8cca6-144">lastModifiedDateTime</span></span>|<span data-ttu-id="8cca6-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cca6-145">DateTimeOffset</span></span>|<span data-ttu-id="8cca6-146">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8cca6-146">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="8cca6-147">displayName</span><span class="sxs-lookup"><span data-stu-id="8cca6-147">displayName</span></span>|<span data-ttu-id="8cca6-148">String</span><span class="sxs-lookup"><span data-stu-id="8cca6-148">String</span></span>|<span data-ttu-id="8cca6-149">管理员提供的 T&C 策略名称。</span><span class="sxs-lookup"><span data-stu-id="8cca6-149">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="8cca6-150">description</span><span class="sxs-lookup"><span data-stu-id="8cca6-150">description</span></span>|<span data-ttu-id="8cca6-151">字符串</span><span class="sxs-lookup"><span data-stu-id="8cca6-151">String</span></span>|<span data-ttu-id="8cca6-152">管理员提供的 T&C 策略描述。</span><span class="sxs-lookup"><span data-stu-id="8cca6-152">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="8cca6-153">title</span><span class="sxs-lookup"><span data-stu-id="8cca6-153">title</span></span>|<span data-ttu-id="8cca6-154">String</span><span class="sxs-lookup"><span data-stu-id="8cca6-154">String</span></span>|<span data-ttu-id="8cca6-155">管理员提供的条款和条件标题。</span><span class="sxs-lookup"><span data-stu-id="8cca6-155">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="8cca6-156">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="8cca6-156">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="8cca6-157">bodyText</span><span class="sxs-lookup"><span data-stu-id="8cca6-157">bodyText</span></span>|<span data-ttu-id="8cca6-158">String</span><span class="sxs-lookup"><span data-stu-id="8cca6-158">String</span></span>|<span data-ttu-id="8cca6-159">管理员提供的条款和条件正文文本，通常为条款本身。</span><span class="sxs-lookup"><span data-stu-id="8cca6-159">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="8cca6-160">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="8cca6-160">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="8cca6-161">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="8cca6-161">acceptanceStatement</span></span>|<span data-ttu-id="8cca6-162">String</span><span class="sxs-lookup"><span data-stu-id="8cca6-162">String</span></span>|<span data-ttu-id="8cca6-163">管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。</span><span class="sxs-lookup"><span data-stu-id="8cca6-163">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="8cca6-164">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="8cca6-164">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="8cca6-165">version</span><span class="sxs-lookup"><span data-stu-id="8cca6-165">version</span></span>|<span data-ttu-id="8cca6-166">Int32</span><span class="sxs-lookup"><span data-stu-id="8cca6-166">Int32</span></span>|<span data-ttu-id="8cca6-167">指示当前条款版本的整数。</span><span class="sxs-lookup"><span data-stu-id="8cca6-167">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="8cca6-168">当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。</span><span class="sxs-lookup"><span data-stu-id="8cca6-168">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|
|<span data-ttu-id="8cca6-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8cca6-169">roleScopeTagIds</span></span>|<span data-ttu-id="8cca6-170">String collection</span><span class="sxs-lookup"><span data-stu-id="8cca6-170">String collection</span></span>|<span data-ttu-id="8cca6-171">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="8cca6-171">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cca6-172">关系</span><span class="sxs-lookup"><span data-stu-id="8cca6-172">Relationships</span></span>
|<span data-ttu-id="8cca6-173">关系</span><span class="sxs-lookup"><span data-stu-id="8cca6-173">Relationship</span></span>|<span data-ttu-id="8cca6-174">类型</span><span class="sxs-lookup"><span data-stu-id="8cca6-174">Type</span></span>|<span data-ttu-id="8cca6-175">说明</span><span class="sxs-lookup"><span data-stu-id="8cca6-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cca6-176">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="8cca6-176">groupAssignments</span></span>|<span data-ttu-id="8cca6-177">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="8cca6-177">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="8cca6-178">此 T&C 策略的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="8cca6-178">The list of group assignments for this T&C policy.</span></span>|
|<span data-ttu-id="8cca6-179">assignments</span><span class="sxs-lookup"><span data-stu-id="8cca6-179">assignments</span></span>|<span data-ttu-id="8cca6-180">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8cca6-180">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="8cca6-181">此 T&C 策略的分配列表。</span><span class="sxs-lookup"><span data-stu-id="8cca6-181">The list of assignments for this T&C policy.</span></span>|
|<span data-ttu-id="8cca6-182">acceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="8cca6-182">acceptanceStatuses</span></span>|<span data-ttu-id="8cca6-183">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8cca6-183">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="8cca6-184">此 T&C 策略的接受状态列表。</span><span class="sxs-lookup"><span data-stu-id="8cca6-184">The list of acceptance statuses for this T&C policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8cca6-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8cca6-185">JSON Representation</span></span>
<span data-ttu-id="8cca6-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8cca6-186">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "title": "String",
  "bodyText": "String",
  "acceptanceStatement": "String",
  "version": 1024,
  "roleScopeTagIds": [
    "String"
  ]
}
```



