---
title: termsAndConditionsAssignment 资源类型
description: termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 07c08866205338aa0d03f5fef4663935b6896b9d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088606"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="de9ec-104">termsAndConditionsAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="de9ec-104">termsAndConditionsAssignment resource type</span></span>

<span data-ttu-id="de9ec-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de9ec-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de9ec-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="de9ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de9ec-107">termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。</span><span class="sxs-lookup"><span data-stu-id="de9ec-107">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="de9ec-108">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="de9ec-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="de9ec-109">方法</span><span class="sxs-lookup"><span data-stu-id="de9ec-109">Methods</span></span>
|<span data-ttu-id="de9ec-110">方法</span><span class="sxs-lookup"><span data-stu-id="de9ec-110">Method</span></span>|<span data-ttu-id="de9ec-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="de9ec-111">Return Type</span></span>|<span data-ttu-id="de9ec-112">说明</span><span class="sxs-lookup"><span data-stu-id="de9ec-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="de9ec-113">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="de9ec-113">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="de9ec-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de9ec-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="de9ec-115">列出 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="de9ec-115">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="de9ec-116">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="de9ec-116">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="de9ec-117">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="de9ec-117">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="de9ec-118">读取 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="de9ec-118">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="de9ec-119">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="de9ec-119">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="de9ec-120">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="de9ec-120">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="de9ec-121">创建新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="de9ec-121">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="de9ec-122">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="de9ec-122">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="de9ec-123">无</span><span class="sxs-lookup"><span data-stu-id="de9ec-123">None</span></span>|<span data-ttu-id="de9ec-124">删除 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="de9ec-124">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="de9ec-125">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="de9ec-125">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="de9ec-126">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="de9ec-126">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="de9ec-127">更新 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="de9ec-127">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="de9ec-128">属性</span><span class="sxs-lookup"><span data-stu-id="de9ec-128">Properties</span></span>
|<span data-ttu-id="de9ec-129">属性</span><span class="sxs-lookup"><span data-stu-id="de9ec-129">Property</span></span>|<span data-ttu-id="de9ec-130">类型</span><span class="sxs-lookup"><span data-stu-id="de9ec-130">Type</span></span>|<span data-ttu-id="de9ec-131">说明</span><span class="sxs-lookup"><span data-stu-id="de9ec-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de9ec-132">id</span><span class="sxs-lookup"><span data-stu-id="de9ec-132">id</span></span>|<span data-ttu-id="de9ec-133">String</span><span class="sxs-lookup"><span data-stu-id="de9ec-133">String</span></span>|<span data-ttu-id="de9ec-134">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="de9ec-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="de9ec-135">target</span><span class="sxs-lookup"><span data-stu-id="de9ec-135">target</span></span>|[<span data-ttu-id="de9ec-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="de9ec-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="de9ec-137">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="de9ec-137">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de9ec-138">关系</span><span class="sxs-lookup"><span data-stu-id="de9ec-138">Relationships</span></span>
<span data-ttu-id="de9ec-139">无</span><span class="sxs-lookup"><span data-stu-id="de9ec-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de9ec-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de9ec-140">JSON Representation</span></span>
<span data-ttu-id="de9ec-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de9ec-141">Here is a JSON representation of the resource.</span></span>
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









