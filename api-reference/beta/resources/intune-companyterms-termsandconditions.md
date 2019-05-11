---
title: termsAndConditions 资源类型
description: TermsAndConditions 实体表示给定条款和条件 (T&C) 策略的元数据和内容。 当用户第一次尝试注册到 Intune 时向用户显示 T&C 策略的内容，之后会在进行了管理员要求重新接受的编辑时显示。 这允许管理员与用户必须同意的预配进行通信，以便将设备注册到 Intune 中。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8dc02275b32cdc3b5c0ca789890245c9b8593dec
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949155"
---
# <a name="termsandconditions-resource-type"></a><span data-ttu-id="de839-105">termsAndConditions 资源类型</span><span class="sxs-lookup"><span data-stu-id="de839-105">termsAndConditions resource type</span></span>

> <span data-ttu-id="de839-106">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="de839-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de839-107">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="de839-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de839-108">TermsAndConditions 实体表示给定条款和条件 (T&C) 策略的元数据和内容。</span><span class="sxs-lookup"><span data-stu-id="de839-108">A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy.</span></span> <span data-ttu-id="de839-109">当用户第一次尝试注册到 Intune 时向用户显示 T&C 策略的内容，之后会在进行了管理员要求重新接受的编辑时显示。</span><span class="sxs-lookup"><span data-stu-id="de839-109">T&C policies’ contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance.</span></span> <span data-ttu-id="de839-110">这允许管理员与用户必须同意的预配进行通信，以便将设备注册到 Intune 中。</span><span class="sxs-lookup"><span data-stu-id="de839-110">They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="de839-111">方法</span><span class="sxs-lookup"><span data-stu-id="de839-111">Methods</span></span>
|<span data-ttu-id="de839-112">方法</span><span class="sxs-lookup"><span data-stu-id="de839-112">Method</span></span>|<span data-ttu-id="de839-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="de839-113">Return Type</span></span>|<span data-ttu-id="de839-114">说明</span><span class="sxs-lookup"><span data-stu-id="de839-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="de839-115">List termsAndConditionses</span><span class="sxs-lookup"><span data-stu-id="de839-115">List termsAndConditionses</span></span>](../api/intune-companyterms-termsandconditions-list.md)|<span data-ttu-id="de839-116">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de839-116">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) collection</span></span>|<span data-ttu-id="de839-117">列出 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="de839-117">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>|
|[<span data-ttu-id="de839-118">Get termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="de839-118">Get termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-get.md)|[<span data-ttu-id="de839-119">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="de839-119">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="de839-120">读取 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="de839-120">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="de839-121">Create termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="de839-121">Create termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-create.md)|[<span data-ttu-id="de839-122">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="de839-122">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="de839-123">创建新的 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="de839-123">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="de839-124">Delete termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="de839-124">Delete termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-delete.md)|<span data-ttu-id="de839-125">无</span><span class="sxs-lookup"><span data-stu-id="de839-125">None</span></span>|<span data-ttu-id="de839-126">删除 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)。</span><span class="sxs-lookup"><span data-stu-id="de839-126">Deletes a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>|
|[<span data-ttu-id="de839-127">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="de839-127">Update termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-update.md)|[<span data-ttu-id="de839-128">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="de839-128">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="de839-129">更新 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="de839-129">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="de839-130">属性</span><span class="sxs-lookup"><span data-stu-id="de839-130">Properties</span></span>
|<span data-ttu-id="de839-131">属性</span><span class="sxs-lookup"><span data-stu-id="de839-131">Property</span></span>|<span data-ttu-id="de839-132">类型</span><span class="sxs-lookup"><span data-stu-id="de839-132">Type</span></span>|<span data-ttu-id="de839-133">说明</span><span class="sxs-lookup"><span data-stu-id="de839-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de839-134">id</span><span class="sxs-lookup"><span data-stu-id="de839-134">id</span></span>|<span data-ttu-id="de839-135">字符串</span><span class="sxs-lookup"><span data-stu-id="de839-135">String</span></span>|<span data-ttu-id="de839-136">T&C 策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="de839-136">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="de839-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de839-137">createdDateTime</span></span>|<span data-ttu-id="de839-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de839-138">DateTimeOffset</span></span>|<span data-ttu-id="de839-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="de839-139">DateTime the object was created.</span></span>|
|<span data-ttu-id="de839-140">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de839-140">modifiedDateTime</span></span>|<span data-ttu-id="de839-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de839-141">DateTimeOffset</span></span>|<span data-ttu-id="de839-142">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="de839-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="de839-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de839-143">lastModifiedDateTime</span></span>|<span data-ttu-id="de839-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de839-144">DateTimeOffset</span></span>|<span data-ttu-id="de839-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="de839-145">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="de839-146">displayName</span><span class="sxs-lookup"><span data-stu-id="de839-146">displayName</span></span>|<span data-ttu-id="de839-147">String</span><span class="sxs-lookup"><span data-stu-id="de839-147">String</span></span>|<span data-ttu-id="de839-148">管理员提供的 T&C 策略名称。</span><span class="sxs-lookup"><span data-stu-id="de839-148">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="de839-149">说明</span><span class="sxs-lookup"><span data-stu-id="de839-149">description</span></span>|<span data-ttu-id="de839-150">字符串</span><span class="sxs-lookup"><span data-stu-id="de839-150">String</span></span>|<span data-ttu-id="de839-151">管理员提供的 T&C 策略描述。</span><span class="sxs-lookup"><span data-stu-id="de839-151">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="de839-152">title</span><span class="sxs-lookup"><span data-stu-id="de839-152">title</span></span>|<span data-ttu-id="de839-153">String</span><span class="sxs-lookup"><span data-stu-id="de839-153">String</span></span>|<span data-ttu-id="de839-154">管理员提供的条款和条件标题。</span><span class="sxs-lookup"><span data-stu-id="de839-154">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="de839-155">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="de839-155">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="de839-156">bodyText</span><span class="sxs-lookup"><span data-stu-id="de839-156">bodyText</span></span>|<span data-ttu-id="de839-157">String</span><span class="sxs-lookup"><span data-stu-id="de839-157">String</span></span>|<span data-ttu-id="de839-158">管理员提供的条款和条件正文文本，通常为条款本身。</span><span class="sxs-lookup"><span data-stu-id="de839-158">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="de839-159">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="de839-159">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="de839-160">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="de839-160">acceptanceStatement</span></span>|<span data-ttu-id="de839-161">String</span><span class="sxs-lookup"><span data-stu-id="de839-161">String</span></span>|<span data-ttu-id="de839-162">管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。</span><span class="sxs-lookup"><span data-stu-id="de839-162">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="de839-163">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="de839-163">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="de839-164">version</span><span class="sxs-lookup"><span data-stu-id="de839-164">version</span></span>|<span data-ttu-id="de839-165">Int32</span><span class="sxs-lookup"><span data-stu-id="de839-165">Int32</span></span>|<span data-ttu-id="de839-166">指示当前条款版本的整数。</span><span class="sxs-lookup"><span data-stu-id="de839-166">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="de839-167">当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。</span><span class="sxs-lookup"><span data-stu-id="de839-167">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de839-168">关系</span><span class="sxs-lookup"><span data-stu-id="de839-168">Relationships</span></span>
|<span data-ttu-id="de839-169">关系</span><span class="sxs-lookup"><span data-stu-id="de839-169">Relationship</span></span>|<span data-ttu-id="de839-170">类型</span><span class="sxs-lookup"><span data-stu-id="de839-170">Type</span></span>|<span data-ttu-id="de839-171">说明</span><span class="sxs-lookup"><span data-stu-id="de839-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de839-172">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="de839-172">groupAssignments</span></span>|<span data-ttu-id="de839-173">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="de839-173">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="de839-174">此 T&C 策略的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="de839-174">The list of group assignments for this T&C policy.</span></span>|
|<span data-ttu-id="de839-175">assignments</span><span class="sxs-lookup"><span data-stu-id="de839-175">assignments</span></span>|<span data-ttu-id="de839-176">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de839-176">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="de839-177">此 T&C 策略的分配列表。</span><span class="sxs-lookup"><span data-stu-id="de839-177">The list of assignments for this T&C policy.</span></span>|
|<span data-ttu-id="de839-178">acceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="de839-178">acceptanceStatuses</span></span>|<span data-ttu-id="de839-179">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de839-179">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="de839-180">此 T&C 策略的接受状态列表。</span><span class="sxs-lookup"><span data-stu-id="de839-180">The list of acceptance statuses for this T&C policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de839-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de839-181">JSON Representation</span></span>
<span data-ttu-id="de839-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de839-182">Here is a JSON representation of the resource.</span></span>
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
  "version": 1024
}
```




