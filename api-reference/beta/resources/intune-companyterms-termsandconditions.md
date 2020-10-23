---
title: termsAndConditions 资源类型
description: TermsAndConditions 实体表示给定条款和条件 (T&C) 策略的元数据和内容。 当用户第一次尝试注册到 Intune 时向用户显示 T&C 策略的内容，之后会在进行了管理员要求重新接受的编辑时显示。 这允许管理员与用户必须同意的预配进行通信，以便将设备注册到 Intune 中。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8b38d4cb630bc7c16f49028dee0721b13dbe1cd1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723949"
---
# <a name="termsandconditions-resource-type"></a><span data-ttu-id="bc59e-105">termsAndConditions 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc59e-105">termsAndConditions resource type</span></span>

<span data-ttu-id="bc59e-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc59e-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc59e-107">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bc59e-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc59e-108">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc59e-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc59e-109">TermsAndConditions 实体表示给定条款和条件 (T&C) 策略的元数据和内容。</span><span class="sxs-lookup"><span data-stu-id="bc59e-109">A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy.</span></span> <span data-ttu-id="bc59e-110">当用户第一次尝试注册到 Intune 时向用户显示 T&C 策略的内容，之后会在进行了管理员要求重新接受的编辑时显示。</span><span class="sxs-lookup"><span data-stu-id="bc59e-110">T&C policies’ contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance.</span></span> <span data-ttu-id="bc59e-111">这允许管理员与用户必须同意的预配进行通信，以便将设备注册到 Intune 中。</span><span class="sxs-lookup"><span data-stu-id="bc59e-111">They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="bc59e-112">Methods</span><span class="sxs-lookup"><span data-stu-id="bc59e-112">Methods</span></span>
|<span data-ttu-id="bc59e-113">方法</span><span class="sxs-lookup"><span data-stu-id="bc59e-113">Method</span></span>|<span data-ttu-id="bc59e-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="bc59e-114">Return Type</span></span>|<span data-ttu-id="bc59e-115">说明</span><span class="sxs-lookup"><span data-stu-id="bc59e-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bc59e-116">List termsAndConditionses</span><span class="sxs-lookup"><span data-stu-id="bc59e-116">List termsAndConditionses</span></span>](../api/intune-companyterms-termsandconditions-list.md)|<span data-ttu-id="bc59e-117">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bc59e-117">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) collection</span></span>|<span data-ttu-id="bc59e-118">列出 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bc59e-118">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>|
|[<span data-ttu-id="bc59e-119">Get termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="bc59e-119">Get termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-get.md)|[<span data-ttu-id="bc59e-120">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="bc59e-120">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="bc59e-121">读取 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bc59e-121">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="bc59e-122">Create termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="bc59e-122">Create termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-create.md)|[<span data-ttu-id="bc59e-123">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="bc59e-123">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="bc59e-124">创建新的 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bc59e-124">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="bc59e-125">Delete termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="bc59e-125">Delete termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-delete.md)|<span data-ttu-id="bc59e-126">无</span><span class="sxs-lookup"><span data-stu-id="bc59e-126">None</span></span>|<span data-ttu-id="bc59e-127">删除 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)。</span><span class="sxs-lookup"><span data-stu-id="bc59e-127">Deletes a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>|
|[<span data-ttu-id="bc59e-128">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="bc59e-128">Update termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-update.md)|[<span data-ttu-id="bc59e-129">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="bc59e-129">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="bc59e-130">更新 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bc59e-130">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc59e-131">属性</span><span class="sxs-lookup"><span data-stu-id="bc59e-131">Properties</span></span>
|<span data-ttu-id="bc59e-132">属性</span><span class="sxs-lookup"><span data-stu-id="bc59e-132">Property</span></span>|<span data-ttu-id="bc59e-133">类型</span><span class="sxs-lookup"><span data-stu-id="bc59e-133">Type</span></span>|<span data-ttu-id="bc59e-134">说明</span><span class="sxs-lookup"><span data-stu-id="bc59e-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc59e-135">id</span><span class="sxs-lookup"><span data-stu-id="bc59e-135">id</span></span>|<span data-ttu-id="bc59e-136">String</span><span class="sxs-lookup"><span data-stu-id="bc59e-136">String</span></span>|<span data-ttu-id="bc59e-137">T&C 策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bc59e-137">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="bc59e-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc59e-138">createdDateTime</span></span>|<span data-ttu-id="bc59e-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc59e-139">DateTimeOffset</span></span>|<span data-ttu-id="bc59e-140">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bc59e-140">DateTime the object was created.</span></span>|
|<span data-ttu-id="bc59e-141">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc59e-141">modifiedDateTime</span></span>|<span data-ttu-id="bc59e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc59e-142">DateTimeOffset</span></span>|<span data-ttu-id="bc59e-143">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bc59e-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="bc59e-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc59e-144">lastModifiedDateTime</span></span>|<span data-ttu-id="bc59e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc59e-145">DateTimeOffset</span></span>|<span data-ttu-id="bc59e-146">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bc59e-146">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="bc59e-147">displayName</span><span class="sxs-lookup"><span data-stu-id="bc59e-147">displayName</span></span>|<span data-ttu-id="bc59e-148">String</span><span class="sxs-lookup"><span data-stu-id="bc59e-148">String</span></span>|<span data-ttu-id="bc59e-149">管理员提供的 T&C 策略名称。</span><span class="sxs-lookup"><span data-stu-id="bc59e-149">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="bc59e-150">说明</span><span class="sxs-lookup"><span data-stu-id="bc59e-150">description</span></span>|<span data-ttu-id="bc59e-151">String</span><span class="sxs-lookup"><span data-stu-id="bc59e-151">String</span></span>|<span data-ttu-id="bc59e-152">管理员提供的 T&C 策略描述。</span><span class="sxs-lookup"><span data-stu-id="bc59e-152">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="bc59e-153">title</span><span class="sxs-lookup"><span data-stu-id="bc59e-153">title</span></span>|<span data-ttu-id="bc59e-154">String</span><span class="sxs-lookup"><span data-stu-id="bc59e-154">String</span></span>|<span data-ttu-id="bc59e-155">管理员提供的条款和条件标题。</span><span class="sxs-lookup"><span data-stu-id="bc59e-155">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="bc59e-156">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="bc59e-156">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="bc59e-157">bodyText</span><span class="sxs-lookup"><span data-stu-id="bc59e-157">bodyText</span></span>|<span data-ttu-id="bc59e-158">String</span><span class="sxs-lookup"><span data-stu-id="bc59e-158">String</span></span>|<span data-ttu-id="bc59e-159">管理员提供的条款和条件正文文本，通常为条款本身。</span><span class="sxs-lookup"><span data-stu-id="bc59e-159">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="bc59e-160">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="bc59e-160">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="bc59e-161">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="bc59e-161">acceptanceStatement</span></span>|<span data-ttu-id="bc59e-162">String</span><span class="sxs-lookup"><span data-stu-id="bc59e-162">String</span></span>|<span data-ttu-id="bc59e-163">管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。</span><span class="sxs-lookup"><span data-stu-id="bc59e-163">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="bc59e-164">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="bc59e-164">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="bc59e-165">version</span><span class="sxs-lookup"><span data-stu-id="bc59e-165">version</span></span>|<span data-ttu-id="bc59e-166">Int32</span><span class="sxs-lookup"><span data-stu-id="bc59e-166">Int32</span></span>|<span data-ttu-id="bc59e-167">指示当前条款版本的整数。</span><span class="sxs-lookup"><span data-stu-id="bc59e-167">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="bc59e-168">当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。</span><span class="sxs-lookup"><span data-stu-id="bc59e-168">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|
|<span data-ttu-id="bc59e-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bc59e-169">roleScopeTagIds</span></span>|<span data-ttu-id="bc59e-170">String collection</span><span class="sxs-lookup"><span data-stu-id="bc59e-170">String collection</span></span>|<span data-ttu-id="bc59e-171">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="bc59e-171">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc59e-172">关系</span><span class="sxs-lookup"><span data-stu-id="bc59e-172">Relationships</span></span>
|<span data-ttu-id="bc59e-173">关系</span><span class="sxs-lookup"><span data-stu-id="bc59e-173">Relationship</span></span>|<span data-ttu-id="bc59e-174">类型</span><span class="sxs-lookup"><span data-stu-id="bc59e-174">Type</span></span>|<span data-ttu-id="bc59e-175">说明</span><span class="sxs-lookup"><span data-stu-id="bc59e-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc59e-176">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="bc59e-176">groupAssignments</span></span>|<span data-ttu-id="bc59e-177">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bc59e-177">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="bc59e-178">此 T&C 策略的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="bc59e-178">The list of group assignments for this T&C policy.</span></span>|
|<span data-ttu-id="bc59e-179">assignments</span><span class="sxs-lookup"><span data-stu-id="bc59e-179">assignments</span></span>|<span data-ttu-id="bc59e-180">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bc59e-180">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="bc59e-181">此 T&C 策略的分配列表。</span><span class="sxs-lookup"><span data-stu-id="bc59e-181">The list of assignments for this T&C policy.</span></span>|
|<span data-ttu-id="bc59e-182">acceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="bc59e-182">acceptanceStatuses</span></span>|<span data-ttu-id="bc59e-183">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bc59e-183">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="bc59e-184">此 T&C 策略的接受状态列表。</span><span class="sxs-lookup"><span data-stu-id="bc59e-184">The list of acceptance statuses for this T&C policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc59e-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc59e-185">JSON Representation</span></span>
<span data-ttu-id="bc59e-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc59e-186">Here is a JSON representation of the resource.</span></span>
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





