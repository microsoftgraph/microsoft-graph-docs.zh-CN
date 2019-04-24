---
title: termsAndConditionsGroupAssignment 资源类型
description: termsAndConditionsGroupAssignment 实体表示分配给给定组的给定条款和条件 (T&C) 策略。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f3518dcc31bf703d3fe42e6bab15d5731d5beb5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463523"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="f7715-104">termsAndConditionsGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7715-104">termsAndConditionsGroupAssignment resource type</span></span>

> <span data-ttu-id="f7715-105">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f7715-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7715-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7715-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7715-107">termsAndConditionsGroupAssignment 实体表示分配给给定组的给定条款和条件 (T&C) 策略。</span><span class="sxs-lookup"><span data-stu-id="f7715-107">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="f7715-108">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="f7715-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="f7715-109">方法</span><span class="sxs-lookup"><span data-stu-id="f7715-109">Methods</span></span>
|<span data-ttu-id="f7715-110">方法</span><span class="sxs-lookup"><span data-stu-id="f7715-110">Method</span></span>|<span data-ttu-id="f7715-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="f7715-111">Return Type</span></span>|<span data-ttu-id="f7715-112">说明</span><span class="sxs-lookup"><span data-stu-id="f7715-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f7715-113">列出 termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="f7715-113">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="f7715-114">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="f7715-114">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="f7715-115">列出[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f7715-115">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="f7715-116">获取 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="f7715-116">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="f7715-117">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="f7715-117">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="f7715-118">读取[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f7715-118">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="f7715-119">创建 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="f7715-119">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="f7715-120">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="f7715-120">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="f7715-121">创建新的[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f7715-121">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="f7715-122">删除 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="f7715-122">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="f7715-123">无</span><span class="sxs-lookup"><span data-stu-id="f7715-123">None</span></span>|<span data-ttu-id="f7715-124">删除[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="f7715-124">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="f7715-125">更新 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="f7715-125">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="f7715-126">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="f7715-126">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="f7715-127">更新[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f7715-127">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f7715-128">属性</span><span class="sxs-lookup"><span data-stu-id="f7715-128">Properties</span></span>
|<span data-ttu-id="f7715-129">属性</span><span class="sxs-lookup"><span data-stu-id="f7715-129">Property</span></span>|<span data-ttu-id="f7715-130">类型</span><span class="sxs-lookup"><span data-stu-id="f7715-130">Type</span></span>|<span data-ttu-id="f7715-131">说明</span><span class="sxs-lookup"><span data-stu-id="f7715-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7715-132">id</span><span class="sxs-lookup"><span data-stu-id="f7715-132">id</span></span>|<span data-ttu-id="f7715-133">String</span><span class="sxs-lookup"><span data-stu-id="f7715-133">String</span></span>|<span data-ttu-id="f7715-134">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f7715-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="f7715-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="f7715-135">targetGroupId</span></span>|<span data-ttu-id="f7715-136">字符串</span><span class="sxs-lookup"><span data-stu-id="f7715-136">String</span></span>|<span data-ttu-id="f7715-137">向其分配 T&C 策略的组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f7715-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7715-138">关系</span><span class="sxs-lookup"><span data-stu-id="f7715-138">Relationships</span></span>
|<span data-ttu-id="f7715-139">关系</span><span class="sxs-lookup"><span data-stu-id="f7715-139">Relationship</span></span>|<span data-ttu-id="f7715-140">类型</span><span class="sxs-lookup"><span data-stu-id="f7715-140">Type</span></span>|<span data-ttu-id="f7715-141">说明</span><span class="sxs-lookup"><span data-stu-id="f7715-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7715-142">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="f7715-142">termsAndConditions</span></span>|[<span data-ttu-id="f7715-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="f7715-143">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="f7715-144">所分配的条款和条件的导航链接。</span><span class="sxs-lookup"><span data-stu-id="f7715-144">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f7715-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7715-145">JSON Representation</span></span>
<span data-ttu-id="f7715-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7715-146">Here is a JSON representation of the resource.</span></span>
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





