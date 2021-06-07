---
title: termsAndConditions 资源类型
description: TermsAndConditions 实体表示给定条款和条件 (T&C) 策略的元数据和内容。 当用户第一次尝试注册到 Intune 时向用户显示 T&C 策略的内容，之后会在进行了管理员要求重新接受的编辑时显示。 这允许管理员与用户必须同意的预配进行通信，以便将设备注册到 Intune 中。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b1dcb37dd703b2094d8104e9860aeb44e4807d1f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758937"
---
# <a name="termsandconditions-resource-type"></a><span data-ttu-id="38a13-105">termsAndConditions 资源类型</span><span class="sxs-lookup"><span data-stu-id="38a13-105">termsAndConditions resource type</span></span>

<span data-ttu-id="38a13-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38a13-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38a13-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="38a13-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38a13-108">TermsAndConditions 实体表示给定条款和条件 (T&C) 策略的元数据和内容。</span><span class="sxs-lookup"><span data-stu-id="38a13-108">A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy.</span></span> <span data-ttu-id="38a13-109">当用户第一次尝试注册到 Intune 时向用户显示 T&C 策略的内容，之后会在进行了管理员要求重新接受的编辑时显示。</span><span class="sxs-lookup"><span data-stu-id="38a13-109">T&C policies’ contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance.</span></span> <span data-ttu-id="38a13-110">这允许管理员与用户必须同意的预配进行通信，以便将设备注册到 Intune 中。</span><span class="sxs-lookup"><span data-stu-id="38a13-110">They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="38a13-111">方法</span><span class="sxs-lookup"><span data-stu-id="38a13-111">Methods</span></span>
|<span data-ttu-id="38a13-112">方法</span><span class="sxs-lookup"><span data-stu-id="38a13-112">Method</span></span>|<span data-ttu-id="38a13-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="38a13-113">Return Type</span></span>|<span data-ttu-id="38a13-114">说明</span><span class="sxs-lookup"><span data-stu-id="38a13-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="38a13-115">List termsAndConditionses</span><span class="sxs-lookup"><span data-stu-id="38a13-115">List termsAndConditionses</span></span>](../api/intune-companyterms-termsandconditions-list.md)|<span data-ttu-id="38a13-116">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 集合</span><span class="sxs-lookup"><span data-stu-id="38a13-116">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) collection</span></span>|<span data-ttu-id="38a13-117">列出 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="38a13-117">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>|
|[<span data-ttu-id="38a13-118">Get termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="38a13-118">Get termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-get.md)|[<span data-ttu-id="38a13-119">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="38a13-119">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="38a13-120">读取 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="38a13-120">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="38a13-121">Create termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="38a13-121">Create termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-create.md)|[<span data-ttu-id="38a13-122">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="38a13-122">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="38a13-123">创建新的 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="38a13-123">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="38a13-124">Delete termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="38a13-124">Delete termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-delete.md)|<span data-ttu-id="38a13-125">无</span><span class="sxs-lookup"><span data-stu-id="38a13-125">None</span></span>|<span data-ttu-id="38a13-126">删除 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)。</span><span class="sxs-lookup"><span data-stu-id="38a13-126">Deletes a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>|
|[<span data-ttu-id="38a13-127">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="38a13-127">Update termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-update.md)|[<span data-ttu-id="38a13-128">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="38a13-128">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="38a13-129">更新 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="38a13-129">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="38a13-130">属性</span><span class="sxs-lookup"><span data-stu-id="38a13-130">Properties</span></span>
|<span data-ttu-id="38a13-131">属性</span><span class="sxs-lookup"><span data-stu-id="38a13-131">Property</span></span>|<span data-ttu-id="38a13-132">类型</span><span class="sxs-lookup"><span data-stu-id="38a13-132">Type</span></span>|<span data-ttu-id="38a13-133">说明</span><span class="sxs-lookup"><span data-stu-id="38a13-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38a13-134">id</span><span class="sxs-lookup"><span data-stu-id="38a13-134">id</span></span>|<span data-ttu-id="38a13-135">String</span><span class="sxs-lookup"><span data-stu-id="38a13-135">String</span></span>|<span data-ttu-id="38a13-136">T&C 策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="38a13-136">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="38a13-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38a13-137">createdDateTime</span></span>|<span data-ttu-id="38a13-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38a13-138">DateTimeOffset</span></span>|<span data-ttu-id="38a13-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="38a13-139">DateTime the object was created.</span></span>|
|<span data-ttu-id="38a13-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38a13-140">lastModifiedDateTime</span></span>|<span data-ttu-id="38a13-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38a13-141">DateTimeOffset</span></span>|<span data-ttu-id="38a13-142">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="38a13-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="38a13-143">displayName</span><span class="sxs-lookup"><span data-stu-id="38a13-143">displayName</span></span>|<span data-ttu-id="38a13-144">String</span><span class="sxs-lookup"><span data-stu-id="38a13-144">String</span></span>|<span data-ttu-id="38a13-145">管理员提供的 T&C 策略名称。</span><span class="sxs-lookup"><span data-stu-id="38a13-145">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="38a13-146">description</span><span class="sxs-lookup"><span data-stu-id="38a13-146">description</span></span>|<span data-ttu-id="38a13-147">String</span><span class="sxs-lookup"><span data-stu-id="38a13-147">String</span></span>|<span data-ttu-id="38a13-148">管理员提供的 T&C 策略描述。</span><span class="sxs-lookup"><span data-stu-id="38a13-148">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="38a13-149">title</span><span class="sxs-lookup"><span data-stu-id="38a13-149">title</span></span>|<span data-ttu-id="38a13-150">String</span><span class="sxs-lookup"><span data-stu-id="38a13-150">String</span></span>|<span data-ttu-id="38a13-151">管理员提供的条款和条件标题。</span><span class="sxs-lookup"><span data-stu-id="38a13-151">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="38a13-152">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="38a13-152">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="38a13-153">bodyText</span><span class="sxs-lookup"><span data-stu-id="38a13-153">bodyText</span></span>|<span data-ttu-id="38a13-154">String</span><span class="sxs-lookup"><span data-stu-id="38a13-154">String</span></span>|<span data-ttu-id="38a13-155">管理员提供的条款和条件正文文本，通常为条款本身。</span><span class="sxs-lookup"><span data-stu-id="38a13-155">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="38a13-156">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="38a13-156">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="38a13-157">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="38a13-157">acceptanceStatement</span></span>|<span data-ttu-id="38a13-158">String</span><span class="sxs-lookup"><span data-stu-id="38a13-158">String</span></span>|<span data-ttu-id="38a13-159">管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。</span><span class="sxs-lookup"><span data-stu-id="38a13-159">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="38a13-160">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="38a13-160">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="38a13-161">version</span><span class="sxs-lookup"><span data-stu-id="38a13-161">version</span></span>|<span data-ttu-id="38a13-162">Int32</span><span class="sxs-lookup"><span data-stu-id="38a13-162">Int32</span></span>|<span data-ttu-id="38a13-163">指示当前条款版本的整数。</span><span class="sxs-lookup"><span data-stu-id="38a13-163">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="38a13-164">当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。</span><span class="sxs-lookup"><span data-stu-id="38a13-164">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38a13-165">关系</span><span class="sxs-lookup"><span data-stu-id="38a13-165">Relationships</span></span>
|<span data-ttu-id="38a13-166">关系</span><span class="sxs-lookup"><span data-stu-id="38a13-166">Relationship</span></span>|<span data-ttu-id="38a13-167">类型</span><span class="sxs-lookup"><span data-stu-id="38a13-167">Type</span></span>|<span data-ttu-id="38a13-168">说明</span><span class="sxs-lookup"><span data-stu-id="38a13-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38a13-169">assignments</span><span class="sxs-lookup"><span data-stu-id="38a13-169">assignments</span></span>|<span data-ttu-id="38a13-170">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="38a13-170">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="38a13-171">此 T&C 策略的分配列表。</span><span class="sxs-lookup"><span data-stu-id="38a13-171">The list of assignments for this T&C policy.</span></span>|
|<span data-ttu-id="38a13-172">acceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="38a13-172">acceptanceStatuses</span></span>|<span data-ttu-id="38a13-173">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="38a13-173">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="38a13-174">此 T&C 策略的接受状态列表。</span><span class="sxs-lookup"><span data-stu-id="38a13-174">The list of acceptance statuses for this T&C policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="38a13-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="38a13-175">JSON Representation</span></span>
<span data-ttu-id="38a13-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38a13-176">Here is a JSON representation of the resource.</span></span>
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
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "title": "String",
  "bodyText": "String",
  "acceptanceStatement": "String",
  "version": 1024
}
```




