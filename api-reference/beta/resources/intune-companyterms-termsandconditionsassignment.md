---
title: termsAndConditionsAssignment 资源类型
description: termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36cabb2ca2e6f375701b17901445650740dead73
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996608"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="803c8-104">termsAndConditionsAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="803c8-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="803c8-105">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="803c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="803c8-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="803c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="803c8-107">termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。</span><span class="sxs-lookup"><span data-stu-id="803c8-107">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="803c8-108">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="803c8-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="803c8-109">方法</span><span class="sxs-lookup"><span data-stu-id="803c8-109">Methods</span></span>
|<span data-ttu-id="803c8-110">方法</span><span class="sxs-lookup"><span data-stu-id="803c8-110">Method</span></span>|<span data-ttu-id="803c8-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="803c8-111">Return Type</span></span>|<span data-ttu-id="803c8-112">说明</span><span class="sxs-lookup"><span data-stu-id="803c8-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="803c8-113">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="803c8-113">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="803c8-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="803c8-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="803c8-115">列出 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="803c8-115">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="803c8-116">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="803c8-116">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="803c8-117">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="803c8-117">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="803c8-118">读取 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="803c8-118">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="803c8-119">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="803c8-119">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="803c8-120">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="803c8-120">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="803c8-121">创建新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="803c8-121">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="803c8-122">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="803c8-122">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="803c8-123">无</span><span class="sxs-lookup"><span data-stu-id="803c8-123">None</span></span>|<span data-ttu-id="803c8-124">删除 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="803c8-124">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="803c8-125">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="803c8-125">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="803c8-126">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="803c8-126">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="803c8-127">更新 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="803c8-127">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="803c8-128">属性</span><span class="sxs-lookup"><span data-stu-id="803c8-128">Properties</span></span>
|<span data-ttu-id="803c8-129">属性</span><span class="sxs-lookup"><span data-stu-id="803c8-129">Property</span></span>|<span data-ttu-id="803c8-130">类型</span><span class="sxs-lookup"><span data-stu-id="803c8-130">Type</span></span>|<span data-ttu-id="803c8-131">说明</span><span class="sxs-lookup"><span data-stu-id="803c8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="803c8-132">id</span><span class="sxs-lookup"><span data-stu-id="803c8-132">id</span></span>|<span data-ttu-id="803c8-133">String</span><span class="sxs-lookup"><span data-stu-id="803c8-133">String</span></span>|<span data-ttu-id="803c8-134">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="803c8-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="803c8-135">target</span><span class="sxs-lookup"><span data-stu-id="803c8-135">target</span></span>|[<span data-ttu-id="803c8-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="803c8-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="803c8-137">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="803c8-137">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="803c8-138">关系</span><span class="sxs-lookup"><span data-stu-id="803c8-138">Relationships</span></span>
<span data-ttu-id="803c8-139">无</span><span class="sxs-lookup"><span data-stu-id="803c8-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="803c8-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="803c8-140">JSON Representation</span></span>
<span data-ttu-id="803c8-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="803c8-141">Here is a JSON representation of the resource.</span></span>
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





