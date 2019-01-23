---
title: termsAndConditionsAssignment 资源类型
description: termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b2de08d2bc90061ed4096a9a010b332872eb36ef
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422024"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="248d6-104">termsAndConditionsAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="248d6-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="248d6-105">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="248d6-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="248d6-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="248d6-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="248d6-107">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="248d6-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="248d6-108">termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。</span><span class="sxs-lookup"><span data-stu-id="248d6-108">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="248d6-109">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="248d6-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="248d6-110">方法</span><span class="sxs-lookup"><span data-stu-id="248d6-110">Methods</span></span>
|<span data-ttu-id="248d6-111">方法</span><span class="sxs-lookup"><span data-stu-id="248d6-111">Method</span></span>|<span data-ttu-id="248d6-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="248d6-112">Return Type</span></span>|<span data-ttu-id="248d6-113">说明</span><span class="sxs-lookup"><span data-stu-id="248d6-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="248d6-114">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="248d6-114">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="248d6-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="248d6-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="248d6-116">列出 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="248d6-116">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="248d6-117">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="248d6-117">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="248d6-118">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="248d6-118">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="248d6-119">读取 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="248d6-119">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="248d6-120">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="248d6-120">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="248d6-121">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="248d6-121">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="248d6-122">创建新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="248d6-122">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="248d6-123">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="248d6-123">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="248d6-124">无</span><span class="sxs-lookup"><span data-stu-id="248d6-124">None</span></span>|<span data-ttu-id="248d6-125">删除 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="248d6-125">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="248d6-126">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="248d6-126">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="248d6-127">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="248d6-127">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="248d6-128">更新 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="248d6-128">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="248d6-129">属性</span><span class="sxs-lookup"><span data-stu-id="248d6-129">Properties</span></span>
|<span data-ttu-id="248d6-130">属性</span><span class="sxs-lookup"><span data-stu-id="248d6-130">Property</span></span>|<span data-ttu-id="248d6-131">类型</span><span class="sxs-lookup"><span data-stu-id="248d6-131">Type</span></span>|<span data-ttu-id="248d6-132">说明</span><span class="sxs-lookup"><span data-stu-id="248d6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="248d6-133">id</span><span class="sxs-lookup"><span data-stu-id="248d6-133">id</span></span>|<span data-ttu-id="248d6-134">String</span><span class="sxs-lookup"><span data-stu-id="248d6-134">String</span></span>|<span data-ttu-id="248d6-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="248d6-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="248d6-136">target</span><span class="sxs-lookup"><span data-stu-id="248d6-136">target</span></span>|[<span data-ttu-id="248d6-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="248d6-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="248d6-138">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="248d6-138">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="248d6-139">关系</span><span class="sxs-lookup"><span data-stu-id="248d6-139">Relationships</span></span>
<span data-ttu-id="248d6-140">无</span><span class="sxs-lookup"><span data-stu-id="248d6-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="248d6-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="248d6-141">JSON Representation</span></span>
<span data-ttu-id="248d6-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="248d6-142">Here is a JSON representation of the resource.</span></span>
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




