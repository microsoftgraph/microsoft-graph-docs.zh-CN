---
title: termsAndConditionsAssignment 资源类型
description: termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ead01aac6a0ae8b297b6c013ce2a2a3b4e421956
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758923"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="67d15-104">termsAndConditionsAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="67d15-104">termsAndConditionsAssignment resource type</span></span>

<span data-ttu-id="67d15-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67d15-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67d15-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="67d15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67d15-107">termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。</span><span class="sxs-lookup"><span data-stu-id="67d15-107">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="67d15-108">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="67d15-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="67d15-109">方法</span><span class="sxs-lookup"><span data-stu-id="67d15-109">Methods</span></span>
|<span data-ttu-id="67d15-110">方法</span><span class="sxs-lookup"><span data-stu-id="67d15-110">Method</span></span>|<span data-ttu-id="67d15-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="67d15-111">Return Type</span></span>|<span data-ttu-id="67d15-112">说明</span><span class="sxs-lookup"><span data-stu-id="67d15-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="67d15-113">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="67d15-113">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="67d15-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="67d15-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="67d15-115">列出 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="67d15-115">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="67d15-116">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="67d15-116">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="67d15-117">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="67d15-117">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="67d15-118">读取 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="67d15-118">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="67d15-119">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="67d15-119">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="67d15-120">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="67d15-120">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="67d15-121">创建新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="67d15-121">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="67d15-122">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="67d15-122">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="67d15-123">无</span><span class="sxs-lookup"><span data-stu-id="67d15-123">None</span></span>|<span data-ttu-id="67d15-124">删除 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="67d15-124">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="67d15-125">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="67d15-125">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="67d15-126">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="67d15-126">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="67d15-127">更新 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="67d15-127">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="67d15-128">属性</span><span class="sxs-lookup"><span data-stu-id="67d15-128">Properties</span></span>
|<span data-ttu-id="67d15-129">属性</span><span class="sxs-lookup"><span data-stu-id="67d15-129">Property</span></span>|<span data-ttu-id="67d15-130">类型</span><span class="sxs-lookup"><span data-stu-id="67d15-130">Type</span></span>|<span data-ttu-id="67d15-131">说明</span><span class="sxs-lookup"><span data-stu-id="67d15-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67d15-132">id</span><span class="sxs-lookup"><span data-stu-id="67d15-132">id</span></span>|<span data-ttu-id="67d15-133">String</span><span class="sxs-lookup"><span data-stu-id="67d15-133">String</span></span>|<span data-ttu-id="67d15-134">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="67d15-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="67d15-135">target</span><span class="sxs-lookup"><span data-stu-id="67d15-135">target</span></span>|[<span data-ttu-id="67d15-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="67d15-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="67d15-137">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="67d15-137">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67d15-138">关系</span><span class="sxs-lookup"><span data-stu-id="67d15-138">Relationships</span></span>
<span data-ttu-id="67d15-139">无</span><span class="sxs-lookup"><span data-stu-id="67d15-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67d15-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67d15-140">JSON Representation</span></span>
<span data-ttu-id="67d15-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67d15-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "collectionId": "String"
  }
}
```




