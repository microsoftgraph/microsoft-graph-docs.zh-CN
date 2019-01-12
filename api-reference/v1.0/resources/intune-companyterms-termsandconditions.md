---
title: termsAndConditions 资源类型
description: C 策略内容显示给用户时注册 Intune 到其第一次尝试并随后在编辑时管理员必须重新接受。 这允许管理员与用户必须同意的预配进行通信，以便将设备注册到 Intune 中。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 9dc1e8b2ea6c8b00296cb3a55aba6e8059e5728a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935470"
---
# <a name="termsandconditions-resource-type"></a><span data-ttu-id="6d1a0-104">termsAndConditions 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d1a0-104">termsAndConditions resource type</span></span>

> <span data-ttu-id="6d1a0-105">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d1a0-106">TermsAndConditions 实体表示给定条款和条件 (T&C) 策略的元数据和内容。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-106">A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (T&C) policy.</span></span> <span data-ttu-id="6d1a0-107">当用户第一次尝试注册到 Intune 时向用户显示 T&C 策略的内容，之后会在进行了管理员要求重新接受的编辑时显示。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-107">T&C policies’ contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance.</span></span> <span data-ttu-id="6d1a0-108">这允许管理员与用户必须同意的预配进行通信，以便将设备注册到 Intune 中。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-108">They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="6d1a0-109">方法</span><span class="sxs-lookup"><span data-stu-id="6d1a0-109">Methods</span></span>
|<span data-ttu-id="6d1a0-110">方法</span><span class="sxs-lookup"><span data-stu-id="6d1a0-110">Method</span></span>|<span data-ttu-id="6d1a0-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="6d1a0-111">Return Type</span></span>|<span data-ttu-id="6d1a0-112">说明</span><span class="sxs-lookup"><span data-stu-id="6d1a0-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6d1a0-113">List termsAndConditionses</span><span class="sxs-lookup"><span data-stu-id="6d1a0-113">List termsAndConditionses</span></span>](../api/intune-companyterms-termsandconditions-list.md)|<span data-ttu-id="6d1a0-114">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6d1a0-114">[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) collection</span></span>|<span data-ttu-id="6d1a0-115">列出 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-115">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>|
|[<span data-ttu-id="6d1a0-116">Get termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="6d1a0-116">Get termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-get.md)|[<span data-ttu-id="6d1a0-117">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="6d1a0-117">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="6d1a0-118">读取 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-118">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="6d1a0-119">Create termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="6d1a0-119">Create termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-create.md)|[<span data-ttu-id="6d1a0-120">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="6d1a0-120">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="6d1a0-121">创建新的 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-121">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|
|[<span data-ttu-id="6d1a0-122">Delete termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="6d1a0-122">Delete termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-delete.md)|<span data-ttu-id="6d1a0-123">无</span><span class="sxs-lookup"><span data-stu-id="6d1a0-123">None</span></span>|<span data-ttu-id="6d1a0-124">删除 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-124">Deletes a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>|
|[<span data-ttu-id="6d1a0-125">Update termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="6d1a0-125">Update termsAndConditions</span></span>](../api/intune-companyterms-termsandconditions-update.md)|[<span data-ttu-id="6d1a0-126">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="6d1a0-126">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="6d1a0-127">更新 [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-127">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6d1a0-128">属性</span><span class="sxs-lookup"><span data-stu-id="6d1a0-128">Properties</span></span>
|<span data-ttu-id="6d1a0-129">属性</span><span class="sxs-lookup"><span data-stu-id="6d1a0-129">Property</span></span>|<span data-ttu-id="6d1a0-130">类型</span><span class="sxs-lookup"><span data-stu-id="6d1a0-130">Type</span></span>|<span data-ttu-id="6d1a0-131">说明</span><span class="sxs-lookup"><span data-stu-id="6d1a0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d1a0-132">id</span><span class="sxs-lookup"><span data-stu-id="6d1a0-132">id</span></span>|<span data-ttu-id="6d1a0-133">String</span><span class="sxs-lookup"><span data-stu-id="6d1a0-133">String</span></span>|<span data-ttu-id="6d1a0-134">T&C 策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-134">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="6d1a0-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d1a0-135">createdDateTime</span></span>|<span data-ttu-id="6d1a0-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d1a0-136">DateTimeOffset</span></span>|<span data-ttu-id="6d1a0-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="6d1a0-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d1a0-138">lastModifiedDateTime</span></span>|<span data-ttu-id="6d1a0-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d1a0-139">DateTimeOffset</span></span>|<span data-ttu-id="6d1a0-140">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="6d1a0-141">displayName</span><span class="sxs-lookup"><span data-stu-id="6d1a0-141">displayName</span></span>|<span data-ttu-id="6d1a0-142">String</span><span class="sxs-lookup"><span data-stu-id="6d1a0-142">String</span></span>|<span data-ttu-id="6d1a0-143">管理员提供的 T&C 策略名称。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-143">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="6d1a0-144">说明</span><span class="sxs-lookup"><span data-stu-id="6d1a0-144">description</span></span>|<span data-ttu-id="6d1a0-145">String</span><span class="sxs-lookup"><span data-stu-id="6d1a0-145">String</span></span>|<span data-ttu-id="6d1a0-146">管理员提供的 T&C 策略描述。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-146">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="6d1a0-147">title</span><span class="sxs-lookup"><span data-stu-id="6d1a0-147">title</span></span>|<span data-ttu-id="6d1a0-148">String</span><span class="sxs-lookup"><span data-stu-id="6d1a0-148">String</span></span>|<span data-ttu-id="6d1a0-149">管理员提供的条款和条件标题。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-149">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="6d1a0-150">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-150">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="6d1a0-151">bodyText</span><span class="sxs-lookup"><span data-stu-id="6d1a0-151">bodyText</span></span>|<span data-ttu-id="6d1a0-152">String</span><span class="sxs-lookup"><span data-stu-id="6d1a0-152">String</span></span>|<span data-ttu-id="6d1a0-153">管理员提供的条款和条件正文文本，通常为条款本身。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-153">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="6d1a0-154">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-154">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="6d1a0-155">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="6d1a0-155">acceptanceStatement</span></span>|<span data-ttu-id="6d1a0-156">String</span><span class="sxs-lookup"><span data-stu-id="6d1a0-156">String</span></span>|<span data-ttu-id="6d1a0-157">管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-157">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="6d1a0-158">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-158">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="6d1a0-159">version</span><span class="sxs-lookup"><span data-stu-id="6d1a0-159">version</span></span>|<span data-ttu-id="6d1a0-160">Int32</span><span class="sxs-lookup"><span data-stu-id="6d1a0-160">Int32</span></span>|<span data-ttu-id="6d1a0-161">指示当前条款版本的整数。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-161">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="6d1a0-162">当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-162">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d1a0-163">关系</span><span class="sxs-lookup"><span data-stu-id="6d1a0-163">Relationships</span></span>
|<span data-ttu-id="6d1a0-164">关系</span><span class="sxs-lookup"><span data-stu-id="6d1a0-164">Relationship</span></span>|<span data-ttu-id="6d1a0-165">类型</span><span class="sxs-lookup"><span data-stu-id="6d1a0-165">Type</span></span>|<span data-ttu-id="6d1a0-166">说明</span><span class="sxs-lookup"><span data-stu-id="6d1a0-166">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d1a0-167">assignments</span><span class="sxs-lookup"><span data-stu-id="6d1a0-167">assignments</span></span>|<span data-ttu-id="6d1a0-168">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6d1a0-168">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="6d1a0-169">此 T&C 策略的分配列表。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-169">The list of assignments for this T&C policy.</span></span>|
|<span data-ttu-id="6d1a0-170">acceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="6d1a0-170">acceptanceStatuses</span></span>|<span data-ttu-id="6d1a0-171">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6d1a0-171">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="6d1a0-172">此 T&C 策略的接受状态列表。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-172">The list of acceptance statuses for this T&C policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d1a0-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d1a0-173">JSON Representation</span></span>
<span data-ttu-id="6d1a0-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d1a0-174">Here is a JSON representation of the resource.</span></span>
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



