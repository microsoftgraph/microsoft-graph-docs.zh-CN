---
title: termsAndConditionsAssignment 资源类型
description: termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e4c8b7ac86f86f2b89bcd21a0576f68b823b9f6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262200"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="75301-104">termsAndConditionsAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="75301-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="75301-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="75301-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75301-106">termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。</span><span class="sxs-lookup"><span data-stu-id="75301-106">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="75301-107">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="75301-107">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="75301-108">方法</span><span class="sxs-lookup"><span data-stu-id="75301-108">Methods</span></span>
|<span data-ttu-id="75301-109">方法</span><span class="sxs-lookup"><span data-stu-id="75301-109">Method</span></span>|<span data-ttu-id="75301-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="75301-110">Return Type</span></span>|<span data-ttu-id="75301-111">说明</span><span class="sxs-lookup"><span data-stu-id="75301-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="75301-112">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="75301-112">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="75301-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75301-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="75301-114">列出 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="75301-114">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="75301-115">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="75301-115">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="75301-116">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="75301-116">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="75301-117">读取 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="75301-117">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="75301-118">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="75301-118">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="75301-119">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="75301-119">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="75301-120">创建新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="75301-120">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="75301-121">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="75301-121">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="75301-122">无</span><span class="sxs-lookup"><span data-stu-id="75301-122">None</span></span>|<span data-ttu-id="75301-123">删除 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="75301-123">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="75301-124">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="75301-124">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="75301-125">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="75301-125">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="75301-126">更新 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="75301-126">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="75301-127">属性</span><span class="sxs-lookup"><span data-stu-id="75301-127">Properties</span></span>
|<span data-ttu-id="75301-128">属性</span><span class="sxs-lookup"><span data-stu-id="75301-128">Property</span></span>|<span data-ttu-id="75301-129">类型</span><span class="sxs-lookup"><span data-stu-id="75301-129">Type</span></span>|<span data-ttu-id="75301-130">说明</span><span class="sxs-lookup"><span data-stu-id="75301-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75301-131">id</span><span class="sxs-lookup"><span data-stu-id="75301-131">id</span></span>|<span data-ttu-id="75301-132">String</span><span class="sxs-lookup"><span data-stu-id="75301-132">String</span></span>|<span data-ttu-id="75301-133">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="75301-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="75301-134">target</span><span class="sxs-lookup"><span data-stu-id="75301-134">target</span></span>|[<span data-ttu-id="75301-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="75301-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="75301-136">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="75301-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75301-137">关系</span><span class="sxs-lookup"><span data-stu-id="75301-137">Relationships</span></span>
<span data-ttu-id="75301-138">无</span><span class="sxs-lookup"><span data-stu-id="75301-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75301-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="75301-139">JSON Representation</span></span>
<span data-ttu-id="75301-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75301-140">Here is a JSON representation of the resource.</span></span>
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



