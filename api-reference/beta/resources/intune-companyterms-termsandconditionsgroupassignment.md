---
title: termsAndConditionsGroupAssignment 资源类型
description: TermsAndConditionsGroupAssignment 实体表示分配的给定条款和条件 (T&C) 到给定的组策略。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0cdb629c380898af078bf0b5eaeb3c39344a5657
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418573"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="caf13-104">termsAndConditionsGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="caf13-104">termsAndConditionsGroupAssignment resource type</span></span>

> <span data-ttu-id="caf13-105">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="caf13-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="caf13-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="caf13-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="caf13-107">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="caf13-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="caf13-108">TermsAndConditionsGroupAssignment 实体表示分配的给定条款和条件 (T&C) 到给定的组策略。</span><span class="sxs-lookup"><span data-stu-id="caf13-108">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="caf13-109">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="caf13-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="caf13-110">方法</span><span class="sxs-lookup"><span data-stu-id="caf13-110">Methods</span></span>
|<span data-ttu-id="caf13-111">方法</span><span class="sxs-lookup"><span data-stu-id="caf13-111">Method</span></span>|<span data-ttu-id="caf13-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="caf13-112">Return Type</span></span>|<span data-ttu-id="caf13-113">说明</span><span class="sxs-lookup"><span data-stu-id="caf13-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="caf13-114">列表 termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="caf13-114">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="caf13-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="caf13-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="caf13-116">列出属性和[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="caf13-116">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="caf13-117">获取 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="caf13-117">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="caf13-118">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="caf13-118">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="caf13-119">读取属性和[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="caf13-119">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="caf13-120">创建 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="caf13-120">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="caf13-121">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="caf13-121">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="caf13-122">创建新的[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="caf13-122">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="caf13-123">删除 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="caf13-123">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="caf13-124">无</span><span class="sxs-lookup"><span data-stu-id="caf13-124">None</span></span>|<span data-ttu-id="caf13-125">删除[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="caf13-125">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="caf13-126">更新 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="caf13-126">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="caf13-127">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="caf13-127">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="caf13-128">更新[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="caf13-128">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="caf13-129">属性</span><span class="sxs-lookup"><span data-stu-id="caf13-129">Properties</span></span>
|<span data-ttu-id="caf13-130">属性</span><span class="sxs-lookup"><span data-stu-id="caf13-130">Property</span></span>|<span data-ttu-id="caf13-131">类型</span><span class="sxs-lookup"><span data-stu-id="caf13-131">Type</span></span>|<span data-ttu-id="caf13-132">说明</span><span class="sxs-lookup"><span data-stu-id="caf13-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caf13-133">id</span><span class="sxs-lookup"><span data-stu-id="caf13-133">id</span></span>|<span data-ttu-id="caf13-134">String</span><span class="sxs-lookup"><span data-stu-id="caf13-134">String</span></span>|<span data-ttu-id="caf13-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="caf13-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="caf13-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="caf13-136">targetGroupId</span></span>|<span data-ttu-id="caf13-137">String</span><span class="sxs-lookup"><span data-stu-id="caf13-137">String</span></span>|<span data-ttu-id="caf13-138">T&C 策略分配给组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="caf13-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="caf13-139">关系</span><span class="sxs-lookup"><span data-stu-id="caf13-139">Relationships</span></span>
|<span data-ttu-id="caf13-140">关系</span><span class="sxs-lookup"><span data-stu-id="caf13-140">Relationship</span></span>|<span data-ttu-id="caf13-141">类型</span><span class="sxs-lookup"><span data-stu-id="caf13-141">Type</span></span>|<span data-ttu-id="caf13-142">说明</span><span class="sxs-lookup"><span data-stu-id="caf13-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caf13-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="caf13-143">termsAndConditions</span></span>|[<span data-ttu-id="caf13-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="caf13-144">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="caf13-145">所分配的条款和条件的导航链接。</span><span class="sxs-lookup"><span data-stu-id="caf13-145">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="caf13-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="caf13-146">JSON Representation</span></span>
<span data-ttu-id="caf13-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="caf13-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```




