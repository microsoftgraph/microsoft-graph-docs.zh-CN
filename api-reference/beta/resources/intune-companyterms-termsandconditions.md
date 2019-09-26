---
title: termsAndConditions 资源类型
description: TermsAndConditions 实体表示给定条款和条件 (T&C) 策略的元数据和内容。 当用户第一次尝试注册到 Intune 时向用户显示 T&C 策略的内容，之后会在进行了管理员要求重新接受的编辑时显示。 这允许管理员与用户必须同意的预配进行通信，以便将设备注册到 Intune 中。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 788c128540d20effeaafcb254019e6b1a76c709a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37198983"
---
# <a name="termsandconditions-resource-type"></a><span data-ttu-id="e8052-105">termsAndConditions 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8052-105">termsAndConditions resource type</span></span>

> <span data-ttu-id="e8052-106">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e8052-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8052-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e8052-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8052-108">TermsAndConditions 实体表示给定条款和条件 (T&C) 策略的元数据和内容。</span><span class="sxs-lookup"><span data-stu-id="e8052-108">A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy.</span></span> <span data-ttu-id="e8052-109">当用户第一次尝试注册到 Intune 时向用户显示 T&C 策略的内容，之后会在进行了管理员要求重新接受的编辑时显示。</span><span class="sxs-lookup"><span data-stu-id="e8052-109">T&C policies’ contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance.</span></span> <span data-ttu-id="e8052-110">这允许管理员与用户必须同意的预配进行通信，以便将设备注册到 Intune 中。</span><span class="sxs-lookup"><span data-stu-id="e8052-110">They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="e8052-111">方法</span><span class="sxs-lookup"><span data-stu-id="e8052-111">Methods</span></span>
|<span data-ttu-id="e8052-112">方法</span><span class="sxs-lookup"><span data-stu-id="e8052-112">Method</span></span>|<span data-ttu-id="e8052-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="e8052-113">Return Type</span></span>|<span data-ttu-id="e8052-114">说明</span><span class="sxs-lookup"><span data-stu-id="e8052-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e8052-115">List termsAndConditionses</span><span class="sxs-lookup"><span data-stu-id="e8052-115">List termsAndConditionses</span></span>](../api/intune-companyterms-termsandconditions-list.md)|<span data-ttu-id="e8052-116">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e8052-116">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) collection</span></span>|<span data-ttu-id="e8052-117">列出 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e8052-117">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>|
|[<span data-ttu-id="e8052-118">Get termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="e8052-118">Get termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-get.md)|[<span data-ttu-id="e8052-119">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="e8052-119">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="e8052-120">读取 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e8052-120">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="e8052-121">Create termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="e8052-121">Create termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-create.md)|[<span data-ttu-id="e8052-122">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="e8052-122">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="e8052-123">创建新的 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e8052-123">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="e8052-124">Delete termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="e8052-124">Delete termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-delete.md)|<span data-ttu-id="e8052-125">无</span><span class="sxs-lookup"><span data-stu-id="e8052-125">None</span></span>|<span data-ttu-id="e8052-126">删除 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)。</span><span class="sxs-lookup"><span data-stu-id="e8052-126">Deletes a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>|
|[<span data-ttu-id="e8052-127">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="e8052-127">Update termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-update.md)|[<span data-ttu-id="e8052-128">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="e8052-128">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="e8052-129">更新 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e8052-129">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e8052-130">属性</span><span class="sxs-lookup"><span data-stu-id="e8052-130">Properties</span></span>
|<span data-ttu-id="e8052-131">属性</span><span class="sxs-lookup"><span data-stu-id="e8052-131">Property</span></span>|<span data-ttu-id="e8052-132">类型</span><span class="sxs-lookup"><span data-stu-id="e8052-132">Type</span></span>|<span data-ttu-id="e8052-133">说明</span><span class="sxs-lookup"><span data-stu-id="e8052-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8052-134">id</span><span class="sxs-lookup"><span data-stu-id="e8052-134">id</span></span>|<span data-ttu-id="e8052-135">字符串</span><span class="sxs-lookup"><span data-stu-id="e8052-135">String</span></span>|<span data-ttu-id="e8052-136">T&C 策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e8052-136">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="e8052-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8052-137">createdDateTime</span></span>|<span data-ttu-id="e8052-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8052-138">DateTimeOffset</span></span>|<span data-ttu-id="e8052-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e8052-139">DateTime the object was created.</span></span>|
|<span data-ttu-id="e8052-140">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8052-140">modifiedDateTime</span></span>|<span data-ttu-id="e8052-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8052-141">DateTimeOffset</span></span>|<span data-ttu-id="e8052-142">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e8052-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="e8052-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8052-143">lastModifiedDateTime</span></span>|<span data-ttu-id="e8052-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8052-144">DateTimeOffset</span></span>|<span data-ttu-id="e8052-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e8052-145">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="e8052-146">displayName</span><span class="sxs-lookup"><span data-stu-id="e8052-146">displayName</span></span>|<span data-ttu-id="e8052-147">String</span><span class="sxs-lookup"><span data-stu-id="e8052-147">String</span></span>|<span data-ttu-id="e8052-148">管理员提供的 T&C 策略名称。</span><span class="sxs-lookup"><span data-stu-id="e8052-148">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="e8052-149">说明</span><span class="sxs-lookup"><span data-stu-id="e8052-149">description</span></span>|<span data-ttu-id="e8052-150">字符串</span><span class="sxs-lookup"><span data-stu-id="e8052-150">String</span></span>|<span data-ttu-id="e8052-151">管理员提供的 T&C 策略描述。</span><span class="sxs-lookup"><span data-stu-id="e8052-151">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="e8052-152">title</span><span class="sxs-lookup"><span data-stu-id="e8052-152">title</span></span>|<span data-ttu-id="e8052-153">String</span><span class="sxs-lookup"><span data-stu-id="e8052-153">String</span></span>|<span data-ttu-id="e8052-154">管理员提供的条款和条件标题。</span><span class="sxs-lookup"><span data-stu-id="e8052-154">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="e8052-155">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="e8052-155">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="e8052-156">bodyText</span><span class="sxs-lookup"><span data-stu-id="e8052-156">bodyText</span></span>|<span data-ttu-id="e8052-157">String</span><span class="sxs-lookup"><span data-stu-id="e8052-157">String</span></span>|<span data-ttu-id="e8052-158">管理员提供的条款和条件正文文本，通常为条款本身。</span><span class="sxs-lookup"><span data-stu-id="e8052-158">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="e8052-159">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="e8052-159">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="e8052-160">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="e8052-160">acceptanceStatement</span></span>|<span data-ttu-id="e8052-161">String</span><span class="sxs-lookup"><span data-stu-id="e8052-161">String</span></span>|<span data-ttu-id="e8052-162">管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。</span><span class="sxs-lookup"><span data-stu-id="e8052-162">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="e8052-163">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="e8052-163">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="e8052-164">version</span><span class="sxs-lookup"><span data-stu-id="e8052-164">version</span></span>|<span data-ttu-id="e8052-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e8052-165">Int32</span></span>|<span data-ttu-id="e8052-166">指示当前条款版本的整数。</span><span class="sxs-lookup"><span data-stu-id="e8052-166">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="e8052-167">当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。</span><span class="sxs-lookup"><span data-stu-id="e8052-167">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|
|<span data-ttu-id="e8052-168">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e8052-168">roleScopeTagIds</span></span>|<span data-ttu-id="e8052-169">String collection</span><span class="sxs-lookup"><span data-stu-id="e8052-169">String collection</span></span>|<span data-ttu-id="e8052-170">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e8052-170">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8052-171">关系</span><span class="sxs-lookup"><span data-stu-id="e8052-171">Relationships</span></span>
|<span data-ttu-id="e8052-172">关系</span><span class="sxs-lookup"><span data-stu-id="e8052-172">Relationship</span></span>|<span data-ttu-id="e8052-173">类型</span><span class="sxs-lookup"><span data-stu-id="e8052-173">Type</span></span>|<span data-ttu-id="e8052-174">说明</span><span class="sxs-lookup"><span data-stu-id="e8052-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8052-175">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="e8052-175">groupAssignments</span></span>|<span data-ttu-id="e8052-176">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="e8052-176">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="e8052-177">此 T&C 策略的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="e8052-177">The list of group assignments for this T&C policy.</span></span>|
|<span data-ttu-id="e8052-178">assignments</span><span class="sxs-lookup"><span data-stu-id="e8052-178">assignments</span></span>|<span data-ttu-id="e8052-179">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e8052-179">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="e8052-180">此 T&C 策略的分配列表。</span><span class="sxs-lookup"><span data-stu-id="e8052-180">The list of assignments for this T&C policy.</span></span>|
|<span data-ttu-id="e8052-181">acceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="e8052-181">acceptanceStatuses</span></span>|<span data-ttu-id="e8052-182">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e8052-182">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="e8052-183">此 T&C 策略的接受状态列表。</span><span class="sxs-lookup"><span data-stu-id="e8052-183">The list of acceptance statuses for this T&C policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8052-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8052-184">JSON Representation</span></span>
<span data-ttu-id="e8052-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8052-185">Here is a JSON representation of the resource.</span></span>
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



