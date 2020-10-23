---
title: termsAndConditionsAssignment 资源类型
description: termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67724290399ea1a279e690c26dfbff9face79034
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726519"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="b5e8c-104">termsAndConditionsAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5e8c-104">termsAndConditionsAssignment resource type</span></span>

<span data-ttu-id="b5e8c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5e8c-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5e8c-106">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b5e8c-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5e8c-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5e8c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5e8c-108">termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。</span><span class="sxs-lookup"><span data-stu-id="b5e8c-108">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="b5e8c-109">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="b5e8c-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="b5e8c-110">Methods</span><span class="sxs-lookup"><span data-stu-id="b5e8c-110">Methods</span></span>
|<span data-ttu-id="b5e8c-111">方法</span><span class="sxs-lookup"><span data-stu-id="b5e8c-111">Method</span></span>|<span data-ttu-id="b5e8c-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="b5e8c-112">Return Type</span></span>|<span data-ttu-id="b5e8c-113">说明</span><span class="sxs-lookup"><span data-stu-id="b5e8c-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b5e8c-114">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="b5e8c-114">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="b5e8c-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b5e8c-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="b5e8c-116">列出 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b5e8c-116">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="b5e8c-117">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="b5e8c-117">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="b5e8c-118">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="b5e8c-118">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="b5e8c-119">读取 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b5e8c-119">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="b5e8c-120">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="b5e8c-120">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="b5e8c-121">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="b5e8c-121">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="b5e8c-122">创建新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b5e8c-122">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="b5e8c-123">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="b5e8c-123">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="b5e8c-124">无</span><span class="sxs-lookup"><span data-stu-id="b5e8c-124">None</span></span>|<span data-ttu-id="b5e8c-125">删除 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b5e8c-125">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="b5e8c-126">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="b5e8c-126">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="b5e8c-127">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="b5e8c-127">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="b5e8c-128">更新 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b5e8c-128">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b5e8c-129">属性</span><span class="sxs-lookup"><span data-stu-id="b5e8c-129">Properties</span></span>
|<span data-ttu-id="b5e8c-130">属性</span><span class="sxs-lookup"><span data-stu-id="b5e8c-130">Property</span></span>|<span data-ttu-id="b5e8c-131">类型</span><span class="sxs-lookup"><span data-stu-id="b5e8c-131">Type</span></span>|<span data-ttu-id="b5e8c-132">说明</span><span class="sxs-lookup"><span data-stu-id="b5e8c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5e8c-133">id</span><span class="sxs-lookup"><span data-stu-id="b5e8c-133">id</span></span>|<span data-ttu-id="b5e8c-134">String</span><span class="sxs-lookup"><span data-stu-id="b5e8c-134">String</span></span>|<span data-ttu-id="b5e8c-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b5e8c-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="b5e8c-136">target</span><span class="sxs-lookup"><span data-stu-id="b5e8c-136">target</span></span>|[<span data-ttu-id="b5e8c-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b5e8c-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b5e8c-138">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="b5e8c-138">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5e8c-139">关系</span><span class="sxs-lookup"><span data-stu-id="b5e8c-139">Relationships</span></span>
<span data-ttu-id="b5e8c-140">无</span><span class="sxs-lookup"><span data-stu-id="b5e8c-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5e8c-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5e8c-141">JSON Representation</span></span>
<span data-ttu-id="b5e8c-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5e8c-142">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```





