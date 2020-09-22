---
title: termsAndConditions 资源类型
description: TermsAndConditions 实体表示给定条款和条件 (T&C) 策略的元数据和内容。 当用户第一次尝试注册到 Intune 时向用户显示 T&C 策略的内容，之后会在进行了管理员要求重新接受的编辑时显示。 这允许管理员与用户必须同意的预配进行通信，以便将设备注册到 Intune 中。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de0999a449c8f92cb026743c344ec2cdbc82ab57
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088620"
---
# <a name="termsandconditions-resource-type"></a><span data-ttu-id="646ae-105">termsAndConditions 资源类型</span><span class="sxs-lookup"><span data-stu-id="646ae-105">termsAndConditions resource type</span></span>

<span data-ttu-id="646ae-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="646ae-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="646ae-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="646ae-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="646ae-108">TermsAndConditions 实体表示给定条款和条件 (T&C) 策略的元数据和内容。</span><span class="sxs-lookup"><span data-stu-id="646ae-108">A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy.</span></span> <span data-ttu-id="646ae-109">当用户第一次尝试注册到 Intune 时向用户显示 T&C 策略的内容，之后会在进行了管理员要求重新接受的编辑时显示。</span><span class="sxs-lookup"><span data-stu-id="646ae-109">T&C policies’ contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance.</span></span> <span data-ttu-id="646ae-110">这允许管理员与用户必须同意的预配进行通信，以便将设备注册到 Intune 中。</span><span class="sxs-lookup"><span data-stu-id="646ae-110">They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="646ae-111">方法</span><span class="sxs-lookup"><span data-stu-id="646ae-111">Methods</span></span>
|<span data-ttu-id="646ae-112">方法</span><span class="sxs-lookup"><span data-stu-id="646ae-112">Method</span></span>|<span data-ttu-id="646ae-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="646ae-113">Return Type</span></span>|<span data-ttu-id="646ae-114">说明</span><span class="sxs-lookup"><span data-stu-id="646ae-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="646ae-115">列出 termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="646ae-115">List termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-list.md)|<span data-ttu-id="646ae-116">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 集合</span><span class="sxs-lookup"><span data-stu-id="646ae-116">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) collection</span></span>|<span data-ttu-id="646ae-117">列出 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="646ae-117">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>|
|[<span data-ttu-id="646ae-118">Get termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="646ae-118">Get termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-get.md)|[<span data-ttu-id="646ae-119">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="646ae-119">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="646ae-120">读取 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="646ae-120">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="646ae-121">Create termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="646ae-121">Create termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-create.md)|[<span data-ttu-id="646ae-122">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="646ae-122">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="646ae-123">创建新的 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="646ae-123">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="646ae-124">Delete termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="646ae-124">Delete termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-delete.md)|<span data-ttu-id="646ae-125">无</span><span class="sxs-lookup"><span data-stu-id="646ae-125">None</span></span>|<span data-ttu-id="646ae-126">删除 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)。</span><span class="sxs-lookup"><span data-stu-id="646ae-126">Deletes a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>|
|[<span data-ttu-id="646ae-127">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="646ae-127">Update termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-update.md)|[<span data-ttu-id="646ae-128">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="646ae-128">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="646ae-129">更新 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="646ae-129">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="646ae-130">属性</span><span class="sxs-lookup"><span data-stu-id="646ae-130">Properties</span></span>
|<span data-ttu-id="646ae-131">属性</span><span class="sxs-lookup"><span data-stu-id="646ae-131">Property</span></span>|<span data-ttu-id="646ae-132">类型</span><span class="sxs-lookup"><span data-stu-id="646ae-132">Type</span></span>|<span data-ttu-id="646ae-133">说明</span><span class="sxs-lookup"><span data-stu-id="646ae-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="646ae-134">id</span><span class="sxs-lookup"><span data-stu-id="646ae-134">id</span></span>|<span data-ttu-id="646ae-135">String</span><span class="sxs-lookup"><span data-stu-id="646ae-135">String</span></span>|<span data-ttu-id="646ae-136">T&C 策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="646ae-136">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="646ae-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="646ae-137">createdDateTime</span></span>|<span data-ttu-id="646ae-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="646ae-138">DateTimeOffset</span></span>|<span data-ttu-id="646ae-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="646ae-139">DateTime the object was created.</span></span>|
|<span data-ttu-id="646ae-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="646ae-140">lastModifiedDateTime</span></span>|<span data-ttu-id="646ae-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="646ae-141">DateTimeOffset</span></span>|<span data-ttu-id="646ae-142">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="646ae-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="646ae-143">displayName</span><span class="sxs-lookup"><span data-stu-id="646ae-143">displayName</span></span>|<span data-ttu-id="646ae-144">String</span><span class="sxs-lookup"><span data-stu-id="646ae-144">String</span></span>|<span data-ttu-id="646ae-145">管理员提供的 T&C 策略名称。</span><span class="sxs-lookup"><span data-stu-id="646ae-145">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="646ae-146">description</span><span class="sxs-lookup"><span data-stu-id="646ae-146">description</span></span>|<span data-ttu-id="646ae-147">String</span><span class="sxs-lookup"><span data-stu-id="646ae-147">String</span></span>|<span data-ttu-id="646ae-148">管理员提供的 T&C 策略描述。</span><span class="sxs-lookup"><span data-stu-id="646ae-148">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="646ae-149">title</span><span class="sxs-lookup"><span data-stu-id="646ae-149">title</span></span>|<span data-ttu-id="646ae-150">String</span><span class="sxs-lookup"><span data-stu-id="646ae-150">String</span></span>|<span data-ttu-id="646ae-151">管理员提供的条款和条件标题。</span><span class="sxs-lookup"><span data-stu-id="646ae-151">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="646ae-152">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="646ae-152">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="646ae-153">bodyText</span><span class="sxs-lookup"><span data-stu-id="646ae-153">bodyText</span></span>|<span data-ttu-id="646ae-154">String</span><span class="sxs-lookup"><span data-stu-id="646ae-154">String</span></span>|<span data-ttu-id="646ae-155">管理员提供的条款和条件正文文本，通常为条款本身。</span><span class="sxs-lookup"><span data-stu-id="646ae-155">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="646ae-156">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="646ae-156">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="646ae-157">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="646ae-157">acceptanceStatement</span></span>|<span data-ttu-id="646ae-158">String</span><span class="sxs-lookup"><span data-stu-id="646ae-158">String</span></span>|<span data-ttu-id="646ae-159">管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。</span><span class="sxs-lookup"><span data-stu-id="646ae-159">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="646ae-160">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="646ae-160">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="646ae-161">version</span><span class="sxs-lookup"><span data-stu-id="646ae-161">version</span></span>|<span data-ttu-id="646ae-162">Int32</span><span class="sxs-lookup"><span data-stu-id="646ae-162">Int32</span></span>|<span data-ttu-id="646ae-163">指示当前条款版本的整数。</span><span class="sxs-lookup"><span data-stu-id="646ae-163">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="646ae-164">当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。</span><span class="sxs-lookup"><span data-stu-id="646ae-164">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="646ae-165">关系</span><span class="sxs-lookup"><span data-stu-id="646ae-165">Relationships</span></span>
|<span data-ttu-id="646ae-166">关系</span><span class="sxs-lookup"><span data-stu-id="646ae-166">Relationship</span></span>|<span data-ttu-id="646ae-167">类型</span><span class="sxs-lookup"><span data-stu-id="646ae-167">Type</span></span>|<span data-ttu-id="646ae-168">说明</span><span class="sxs-lookup"><span data-stu-id="646ae-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="646ae-169">assignments</span><span class="sxs-lookup"><span data-stu-id="646ae-169">assignments</span></span>|<span data-ttu-id="646ae-170">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="646ae-170">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="646ae-171">此 T&C 策略的分配列表。</span><span class="sxs-lookup"><span data-stu-id="646ae-171">The list of assignments for this T&C policy.</span></span>|
|<span data-ttu-id="646ae-172">acceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="646ae-172">acceptanceStatuses</span></span>|<span data-ttu-id="646ae-173">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="646ae-173">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="646ae-174">此 T&C 策略的接受状态列表。</span><span class="sxs-lookup"><span data-stu-id="646ae-174">The list of acceptance statuses for this T&C policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="646ae-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="646ae-175">JSON Representation</span></span>
<span data-ttu-id="646ae-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="646ae-176">Here is a JSON representation of the resource.</span></span>
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









