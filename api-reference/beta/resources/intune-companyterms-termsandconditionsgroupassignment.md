---
title: termsAndConditionsGroupAssignment 资源类型
description: TermsAndConditionsGroupAssignment 实体表示将给定的条款和条件分配给给定组 (T&C) 策略。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 29cc8d853c9cb9bf426544681a9e69a0f4e4a5ea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024372"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="4bc44-104">termsAndConditionsGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="4bc44-104">termsAndConditionsGroupAssignment resource type</span></span>

<span data-ttu-id="4bc44-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bc44-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4bc44-106">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4bc44-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bc44-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4bc44-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bc44-108">TermsAndConditionsGroupAssignment 实体表示将给定的条款和条件分配给给定组 (T&C) 策略。</span><span class="sxs-lookup"><span data-stu-id="4bc44-108">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="4bc44-109">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="4bc44-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="4bc44-110">方法</span><span class="sxs-lookup"><span data-stu-id="4bc44-110">Methods</span></span>
|<span data-ttu-id="4bc44-111">方法</span><span class="sxs-lookup"><span data-stu-id="4bc44-111">Method</span></span>|<span data-ttu-id="4bc44-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="4bc44-112">Return Type</span></span>|<span data-ttu-id="4bc44-113">说明</span><span class="sxs-lookup"><span data-stu-id="4bc44-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4bc44-114">列出 termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="4bc44-114">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="4bc44-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4bc44-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="4bc44-116">列出 [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4bc44-116">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="4bc44-117">获取 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4bc44-117">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="4bc44-118">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4bc44-118">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="4bc44-119">读取 [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4bc44-119">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="4bc44-120">创建 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4bc44-120">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="4bc44-121">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4bc44-121">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="4bc44-122">创建新的 [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4bc44-122">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="4bc44-123">删除 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4bc44-123">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="4bc44-124">无</span><span class="sxs-lookup"><span data-stu-id="4bc44-124">None</span></span>|<span data-ttu-id="4bc44-125">删除 [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="4bc44-125">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="4bc44-126">更新 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4bc44-126">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="4bc44-127">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4bc44-127">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="4bc44-128">更新 [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4bc44-128">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4bc44-129">属性</span><span class="sxs-lookup"><span data-stu-id="4bc44-129">Properties</span></span>
|<span data-ttu-id="4bc44-130">属性</span><span class="sxs-lookup"><span data-stu-id="4bc44-130">Property</span></span>|<span data-ttu-id="4bc44-131">类型</span><span class="sxs-lookup"><span data-stu-id="4bc44-131">Type</span></span>|<span data-ttu-id="4bc44-132">说明</span><span class="sxs-lookup"><span data-stu-id="4bc44-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bc44-133">id</span><span class="sxs-lookup"><span data-stu-id="4bc44-133">id</span></span>|<span data-ttu-id="4bc44-134">String</span><span class="sxs-lookup"><span data-stu-id="4bc44-134">String</span></span>|<span data-ttu-id="4bc44-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4bc44-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="4bc44-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="4bc44-136">targetGroupId</span></span>|<span data-ttu-id="4bc44-137">String</span><span class="sxs-lookup"><span data-stu-id="4bc44-137">String</span></span>|<span data-ttu-id="4bc44-138">向其分配 T&C 策略的组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4bc44-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4bc44-139">关系</span><span class="sxs-lookup"><span data-stu-id="4bc44-139">Relationships</span></span>
|<span data-ttu-id="4bc44-140">关系</span><span class="sxs-lookup"><span data-stu-id="4bc44-140">Relationship</span></span>|<span data-ttu-id="4bc44-141">类型</span><span class="sxs-lookup"><span data-stu-id="4bc44-141">Type</span></span>|<span data-ttu-id="4bc44-142">说明</span><span class="sxs-lookup"><span data-stu-id="4bc44-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bc44-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="4bc44-143">termsAndConditions</span></span>|[<span data-ttu-id="4bc44-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="4bc44-144">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="4bc44-145">所分配的条款和条件的导航链接。</span><span class="sxs-lookup"><span data-stu-id="4bc44-145">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4bc44-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4bc44-146">JSON Representation</span></span>
<span data-ttu-id="4bc44-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4bc44-147">Here is a JSON representation of the resource.</span></span>
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






