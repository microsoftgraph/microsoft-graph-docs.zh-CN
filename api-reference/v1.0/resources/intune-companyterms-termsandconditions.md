---
title: termsAndConditions 资源类型
description: TermsAndConditions 实体表示给定条款和条件 (T&C) 策略的元数据和内容。 当用户第一次尝试注册到 Intune 时向用户显示 T&C 策略的内容，之后会在进行了管理员要求重新接受的编辑时显示。 这允许管理员与用户必须同意的预配进行通信，以便将设备注册到 Intune 中。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: be4cf9b5145a6e5ee320e82f33ec2f67a70829a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031988"
---
# <a name="termsandconditions-resource-type"></a><span data-ttu-id="ed980-105">termsAndConditions 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed980-105">termsAndConditions resource type</span></span>

> <span data-ttu-id="ed980-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ed980-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed980-107">TermsAndConditions 实体表示给定条款和条件 (T&C) 策略的元数据和内容。</span><span class="sxs-lookup"><span data-stu-id="ed980-107">A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy.</span></span> <span data-ttu-id="ed980-108">当用户第一次尝试注册到 Intune 时向用户显示 T&C 策略的内容，之后会在进行了管理员要求重新接受的编辑时显示。</span><span class="sxs-lookup"><span data-stu-id="ed980-108">T&C policies’ contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance.</span></span> <span data-ttu-id="ed980-109">这允许管理员与用户必须同意的预配进行通信，以便将设备注册到 Intune 中。</span><span class="sxs-lookup"><span data-stu-id="ed980-109">They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="ed980-110">方法</span><span class="sxs-lookup"><span data-stu-id="ed980-110">Methods</span></span>
|<span data-ttu-id="ed980-111">方法</span><span class="sxs-lookup"><span data-stu-id="ed980-111">Method</span></span>|<span data-ttu-id="ed980-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="ed980-112">Return Type</span></span>|<span data-ttu-id="ed980-113">说明</span><span class="sxs-lookup"><span data-stu-id="ed980-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ed980-114">List termsAndConditionses</span><span class="sxs-lookup"><span data-stu-id="ed980-114">List termsAndConditionses</span></span>](../api/intune-companyterms-termsandconditions-list.md)|<span data-ttu-id="ed980-115">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed980-115">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) collection</span></span>|<span data-ttu-id="ed980-116">列出 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ed980-116">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>|
|[<span data-ttu-id="ed980-117">Get termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="ed980-117">Get termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-get.md)|[<span data-ttu-id="ed980-118">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="ed980-118">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="ed980-119">读取 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ed980-119">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="ed980-120">Create termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="ed980-120">Create termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-create.md)|[<span data-ttu-id="ed980-121">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="ed980-121">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="ed980-122">创建新的 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ed980-122">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="ed980-123">Delete termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="ed980-123">Delete termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-delete.md)|<span data-ttu-id="ed980-124">无</span><span class="sxs-lookup"><span data-stu-id="ed980-124">None</span></span>|<span data-ttu-id="ed980-125">删除 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)。</span><span class="sxs-lookup"><span data-stu-id="ed980-125">Deletes a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>|
|[<span data-ttu-id="ed980-126">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="ed980-126">Update termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-update.md)|[<span data-ttu-id="ed980-127">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="ed980-127">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="ed980-128">更新 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ed980-128">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ed980-129">属性</span><span class="sxs-lookup"><span data-stu-id="ed980-129">Properties</span></span>
|<span data-ttu-id="ed980-130">属性</span><span class="sxs-lookup"><span data-stu-id="ed980-130">Property</span></span>|<span data-ttu-id="ed980-131">类型</span><span class="sxs-lookup"><span data-stu-id="ed980-131">Type</span></span>|<span data-ttu-id="ed980-132">说明</span><span class="sxs-lookup"><span data-stu-id="ed980-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed980-133">id</span><span class="sxs-lookup"><span data-stu-id="ed980-133">id</span></span>|<span data-ttu-id="ed980-134">字符串</span><span class="sxs-lookup"><span data-stu-id="ed980-134">String</span></span>|<span data-ttu-id="ed980-135">T&C 策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ed980-135">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="ed980-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed980-136">createdDateTime</span></span>|<span data-ttu-id="ed980-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed980-137">DateTimeOffset</span></span>|<span data-ttu-id="ed980-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ed980-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="ed980-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed980-139">lastModifiedDateTime</span></span>|<span data-ttu-id="ed980-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed980-140">DateTimeOffset</span></span>|<span data-ttu-id="ed980-141">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ed980-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="ed980-142">displayName</span><span class="sxs-lookup"><span data-stu-id="ed980-142">displayName</span></span>|<span data-ttu-id="ed980-143">String</span><span class="sxs-lookup"><span data-stu-id="ed980-143">String</span></span>|<span data-ttu-id="ed980-144">管理员提供的 T&C 策略名称。</span><span class="sxs-lookup"><span data-stu-id="ed980-144">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="ed980-145">说明</span><span class="sxs-lookup"><span data-stu-id="ed980-145">description</span></span>|<span data-ttu-id="ed980-146">字符串</span><span class="sxs-lookup"><span data-stu-id="ed980-146">String</span></span>|<span data-ttu-id="ed980-147">管理员提供的 T&C 策略描述。</span><span class="sxs-lookup"><span data-stu-id="ed980-147">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="ed980-148">title</span><span class="sxs-lookup"><span data-stu-id="ed980-148">title</span></span>|<span data-ttu-id="ed980-149">String</span><span class="sxs-lookup"><span data-stu-id="ed980-149">String</span></span>|<span data-ttu-id="ed980-150">管理员提供的条款和条件标题。</span><span class="sxs-lookup"><span data-stu-id="ed980-150">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="ed980-151">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="ed980-151">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="ed980-152">bodyText</span><span class="sxs-lookup"><span data-stu-id="ed980-152">bodyText</span></span>|<span data-ttu-id="ed980-153">String</span><span class="sxs-lookup"><span data-stu-id="ed980-153">String</span></span>|<span data-ttu-id="ed980-154">管理员提供的条款和条件正文文本，通常为条款本身。</span><span class="sxs-lookup"><span data-stu-id="ed980-154">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="ed980-155">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="ed980-155">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="ed980-156">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="ed980-156">acceptanceStatement</span></span>|<span data-ttu-id="ed980-157">String</span><span class="sxs-lookup"><span data-stu-id="ed980-157">String</span></span>|<span data-ttu-id="ed980-158">管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。</span><span class="sxs-lookup"><span data-stu-id="ed980-158">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="ed980-159">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="ed980-159">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="ed980-160">version</span><span class="sxs-lookup"><span data-stu-id="ed980-160">version</span></span>|<span data-ttu-id="ed980-161">Int32</span><span class="sxs-lookup"><span data-stu-id="ed980-161">Int32</span></span>|<span data-ttu-id="ed980-162">指示当前条款版本的整数。</span><span class="sxs-lookup"><span data-stu-id="ed980-162">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="ed980-163">当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。</span><span class="sxs-lookup"><span data-stu-id="ed980-163">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed980-164">关系</span><span class="sxs-lookup"><span data-stu-id="ed980-164">Relationships</span></span>
|<span data-ttu-id="ed980-165">关系</span><span class="sxs-lookup"><span data-stu-id="ed980-165">Relationship</span></span>|<span data-ttu-id="ed980-166">类型</span><span class="sxs-lookup"><span data-stu-id="ed980-166">Type</span></span>|<span data-ttu-id="ed980-167">说明</span><span class="sxs-lookup"><span data-stu-id="ed980-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed980-168">assignments</span><span class="sxs-lookup"><span data-stu-id="ed980-168">assignments</span></span>|<span data-ttu-id="ed980-169">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed980-169">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="ed980-170">此 T&C 策略的分配列表。</span><span class="sxs-lookup"><span data-stu-id="ed980-170">The list of assignments for this T&C policy.</span></span>|
|<span data-ttu-id="ed980-171">acceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="ed980-171">acceptanceStatuses</span></span>|<span data-ttu-id="ed980-172">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ed980-172">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="ed980-173">此 T&C 策略的接受状态列表。</span><span class="sxs-lookup"><span data-stu-id="ed980-173">The list of acceptance statuses for this T&C policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed980-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed980-174">JSON Representation</span></span>
<span data-ttu-id="ed980-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed980-175">Here is a JSON representation of the resource.</span></span>
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



