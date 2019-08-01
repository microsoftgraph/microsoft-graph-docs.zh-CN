---
title: termsAndConditionsAssignment 资源类型
description: termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b11f96cb6c8b1062c25e194ab8e3d96ea7c1deeb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031981"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="e76b4-104">termsAndConditionsAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="e76b4-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="e76b4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e76b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e76b4-106">termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。</span><span class="sxs-lookup"><span data-stu-id="e76b4-106">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="e76b4-107">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="e76b4-107">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="e76b4-108">方法</span><span class="sxs-lookup"><span data-stu-id="e76b4-108">Methods</span></span>
|<span data-ttu-id="e76b4-109">方法</span><span class="sxs-lookup"><span data-stu-id="e76b4-109">Method</span></span>|<span data-ttu-id="e76b4-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e76b4-110">Return Type</span></span>|<span data-ttu-id="e76b4-111">说明</span><span class="sxs-lookup"><span data-stu-id="e76b4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e76b4-112">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="e76b4-112">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="e76b4-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e76b4-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="e76b4-114">列出 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e76b4-114">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="e76b4-115">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="e76b4-115">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="e76b4-116">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="e76b4-116">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="e76b4-117">读取 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e76b4-117">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="e76b4-118">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="e76b4-118">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="e76b4-119">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="e76b4-119">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="e76b4-120">创建新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e76b4-120">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="e76b4-121">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="e76b4-121">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="e76b4-122">无</span><span class="sxs-lookup"><span data-stu-id="e76b4-122">None</span></span>|<span data-ttu-id="e76b4-123">删除 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e76b4-123">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="e76b4-124">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="e76b4-124">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="e76b4-125">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="e76b4-125">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="e76b4-126">更新 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e76b4-126">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e76b4-127">属性</span><span class="sxs-lookup"><span data-stu-id="e76b4-127">Properties</span></span>
|<span data-ttu-id="e76b4-128">属性</span><span class="sxs-lookup"><span data-stu-id="e76b4-128">Property</span></span>|<span data-ttu-id="e76b4-129">类型</span><span class="sxs-lookup"><span data-stu-id="e76b4-129">Type</span></span>|<span data-ttu-id="e76b4-130">说明</span><span class="sxs-lookup"><span data-stu-id="e76b4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e76b4-131">id</span><span class="sxs-lookup"><span data-stu-id="e76b4-131">id</span></span>|<span data-ttu-id="e76b4-132">String</span><span class="sxs-lookup"><span data-stu-id="e76b4-132">String</span></span>|<span data-ttu-id="e76b4-133">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e76b4-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="e76b4-134">target</span><span class="sxs-lookup"><span data-stu-id="e76b4-134">target</span></span>|[<span data-ttu-id="e76b4-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e76b4-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e76b4-136">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="e76b4-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e76b4-137">关系</span><span class="sxs-lookup"><span data-stu-id="e76b4-137">Relationships</span></span>
<span data-ttu-id="e76b4-138">无</span><span class="sxs-lookup"><span data-stu-id="e76b4-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e76b4-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e76b4-139">JSON Representation</span></span>
<span data-ttu-id="e76b4-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e76b4-140">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



