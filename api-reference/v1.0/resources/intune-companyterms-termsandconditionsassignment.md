---
title: termsAndConditionsAssignment 资源类型
description: termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 914a1f9a92a1071e37a1f0ed853ead70135a14c4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530984"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="de103-104">termsAndConditionsAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="de103-104">termsAndConditionsAssignment resource type</span></span>

<span data-ttu-id="de103-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de103-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de103-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="de103-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de103-107">termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。</span><span class="sxs-lookup"><span data-stu-id="de103-107">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="de103-108">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="de103-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="de103-109">Methods</span><span class="sxs-lookup"><span data-stu-id="de103-109">Methods</span></span>
|<span data-ttu-id="de103-110">方法</span><span class="sxs-lookup"><span data-stu-id="de103-110">Method</span></span>|<span data-ttu-id="de103-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="de103-111">Return Type</span></span>|<span data-ttu-id="de103-112">说明</span><span class="sxs-lookup"><span data-stu-id="de103-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="de103-113">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="de103-113">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="de103-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de103-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="de103-115">列出 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="de103-115">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="de103-116">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="de103-116">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="de103-117">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="de103-117">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="de103-118">读取 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="de103-118">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="de103-119">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="de103-119">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="de103-120">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="de103-120">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="de103-121">创建新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="de103-121">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="de103-122">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="de103-122">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="de103-123">无</span><span class="sxs-lookup"><span data-stu-id="de103-123">None</span></span>|<span data-ttu-id="de103-124">删除 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="de103-124">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="de103-125">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="de103-125">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="de103-126">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="de103-126">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="de103-127">更新 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="de103-127">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="de103-128">属性</span><span class="sxs-lookup"><span data-stu-id="de103-128">Properties</span></span>
|<span data-ttu-id="de103-129">属性</span><span class="sxs-lookup"><span data-stu-id="de103-129">Property</span></span>|<span data-ttu-id="de103-130">类型</span><span class="sxs-lookup"><span data-stu-id="de103-130">Type</span></span>|<span data-ttu-id="de103-131">说明</span><span class="sxs-lookup"><span data-stu-id="de103-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de103-132">id</span><span class="sxs-lookup"><span data-stu-id="de103-132">id</span></span>|<span data-ttu-id="de103-133">字符串</span><span class="sxs-lookup"><span data-stu-id="de103-133">String</span></span>|<span data-ttu-id="de103-134">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="de103-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="de103-135">target</span><span class="sxs-lookup"><span data-stu-id="de103-135">target</span></span>|[<span data-ttu-id="de103-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="de103-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="de103-137">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="de103-137">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de103-138">关系</span><span class="sxs-lookup"><span data-stu-id="de103-138">Relationships</span></span>
<span data-ttu-id="de103-139">无</span><span class="sxs-lookup"><span data-stu-id="de103-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de103-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de103-140">JSON Representation</span></span>
<span data-ttu-id="de103-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de103-141">Here is a JSON representation of the resource.</span></span>
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




