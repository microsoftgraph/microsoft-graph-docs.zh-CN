---
title: termsAndConditionsGroupAssignment 资源类型
description: TermsAndConditionsGroupAssignment 实体表示将给定条款和条件 (T&C) 策略分配给给定组。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 804ac878ef2ec691d1dd4ca5e62cf28ec4ef1770
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996601"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="7ba43-104">termsAndConditionsGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ba43-104">termsAndConditionsGroupAssignment resource type</span></span>

> <span data-ttu-id="7ba43-105">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7ba43-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ba43-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7ba43-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ba43-107">TermsAndConditionsGroupAssignment 实体表示将给定条款和条件 (T&C) 策略分配给给定组。</span><span class="sxs-lookup"><span data-stu-id="7ba43-107">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="7ba43-108">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="7ba43-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="7ba43-109">方法</span><span class="sxs-lookup"><span data-stu-id="7ba43-109">Methods</span></span>
|<span data-ttu-id="7ba43-110">方法</span><span class="sxs-lookup"><span data-stu-id="7ba43-110">Method</span></span>|<span data-ttu-id="7ba43-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="7ba43-111">Return Type</span></span>|<span data-ttu-id="7ba43-112">说明</span><span class="sxs-lookup"><span data-stu-id="7ba43-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7ba43-113">列出 termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="7ba43-113">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="7ba43-114">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="7ba43-114">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="7ba43-115">列出[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7ba43-115">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="7ba43-116">获取 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="7ba43-116">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="7ba43-117">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="7ba43-117">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="7ba43-118">读取[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7ba43-118">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="7ba43-119">创建 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="7ba43-119">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="7ba43-120">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="7ba43-120">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="7ba43-121">创建新的[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7ba43-121">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="7ba43-122">删除 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="7ba43-122">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="7ba43-123">无</span><span class="sxs-lookup"><span data-stu-id="7ba43-123">None</span></span>|<span data-ttu-id="7ba43-124">删除[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="7ba43-124">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="7ba43-125">更新 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="7ba43-125">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="7ba43-126">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="7ba43-126">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="7ba43-127">更新[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7ba43-127">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7ba43-128">属性</span><span class="sxs-lookup"><span data-stu-id="7ba43-128">Properties</span></span>
|<span data-ttu-id="7ba43-129">属性</span><span class="sxs-lookup"><span data-stu-id="7ba43-129">Property</span></span>|<span data-ttu-id="7ba43-130">类型</span><span class="sxs-lookup"><span data-stu-id="7ba43-130">Type</span></span>|<span data-ttu-id="7ba43-131">说明</span><span class="sxs-lookup"><span data-stu-id="7ba43-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ba43-132">id</span><span class="sxs-lookup"><span data-stu-id="7ba43-132">id</span></span>|<span data-ttu-id="7ba43-133">String</span><span class="sxs-lookup"><span data-stu-id="7ba43-133">String</span></span>|<span data-ttu-id="7ba43-134">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7ba43-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="7ba43-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="7ba43-135">targetGroupId</span></span>|<span data-ttu-id="7ba43-136">String</span><span class="sxs-lookup"><span data-stu-id="7ba43-136">String</span></span>|<span data-ttu-id="7ba43-137">向其分配 T&C 策略的组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7ba43-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ba43-138">关系</span><span class="sxs-lookup"><span data-stu-id="7ba43-138">Relationships</span></span>
|<span data-ttu-id="7ba43-139">关系</span><span class="sxs-lookup"><span data-stu-id="7ba43-139">Relationship</span></span>|<span data-ttu-id="7ba43-140">类型</span><span class="sxs-lookup"><span data-stu-id="7ba43-140">Type</span></span>|<span data-ttu-id="7ba43-141">说明</span><span class="sxs-lookup"><span data-stu-id="7ba43-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ba43-142">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="7ba43-142">termsAndConditions</span></span>|[<span data-ttu-id="7ba43-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="7ba43-143">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="7ba43-144">所分配的条款和条件的导航链接。</span><span class="sxs-lookup"><span data-stu-id="7ba43-144">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ba43-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ba43-145">JSON Representation</span></span>
<span data-ttu-id="7ba43-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ba43-146">Here is a JSON representation of the resource.</span></span>
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





