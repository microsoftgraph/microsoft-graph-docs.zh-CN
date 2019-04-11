---
title: termsAndConditionsAssignment 资源类型
description: termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9b6bff777bfaf093d1148a584cc8524069304b70
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788482"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="7ba6a-104">termsAndConditionsAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ba6a-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="7ba6a-105">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7ba6a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ba6a-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7ba6a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ba6a-107">termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。</span><span class="sxs-lookup"><span data-stu-id="7ba6a-107">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="7ba6a-108">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="7ba6a-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="7ba6a-109">方法</span><span class="sxs-lookup"><span data-stu-id="7ba6a-109">Methods</span></span>
|<span data-ttu-id="7ba6a-110">方法</span><span class="sxs-lookup"><span data-stu-id="7ba6a-110">Method</span></span>|<span data-ttu-id="7ba6a-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="7ba6a-111">Return Type</span></span>|<span data-ttu-id="7ba6a-112">说明</span><span class="sxs-lookup"><span data-stu-id="7ba6a-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7ba6a-113">列出 termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="7ba6a-113">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="7ba6a-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7ba6a-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="7ba6a-115">列出 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7ba6a-115">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="7ba6a-116">获取 termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7ba6a-116">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="7ba6a-117">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7ba6a-117">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="7ba6a-118">读取 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7ba6a-118">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="7ba6a-119">创建 termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7ba6a-119">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="7ba6a-120">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7ba6a-120">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="7ba6a-121">创建新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7ba6a-121">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="7ba6a-122">删除 termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7ba6a-122">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="7ba6a-123">无</span><span class="sxs-lookup"><span data-stu-id="7ba6a-123">None</span></span>|<span data-ttu-id="7ba6a-124">删除 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7ba6a-124">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="7ba6a-125">更新 termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7ba6a-125">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="7ba6a-126">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7ba6a-126">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="7ba6a-127">更新 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7ba6a-127">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7ba6a-128">属性</span><span class="sxs-lookup"><span data-stu-id="7ba6a-128">Properties</span></span>
|<span data-ttu-id="7ba6a-129">属性</span><span class="sxs-lookup"><span data-stu-id="7ba6a-129">Property</span></span>|<span data-ttu-id="7ba6a-130">类型</span><span class="sxs-lookup"><span data-stu-id="7ba6a-130">Type</span></span>|<span data-ttu-id="7ba6a-131">说明</span><span class="sxs-lookup"><span data-stu-id="7ba6a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ba6a-132">id</span><span class="sxs-lookup"><span data-stu-id="7ba6a-132">id</span></span>|<span data-ttu-id="7ba6a-133">String</span><span class="sxs-lookup"><span data-stu-id="7ba6a-133">String</span></span>|<span data-ttu-id="7ba6a-134">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7ba6a-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="7ba6a-135">target</span><span class="sxs-lookup"><span data-stu-id="7ba6a-135">target</span></span>|[<span data-ttu-id="7ba6a-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7ba6a-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7ba6a-137">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="7ba6a-137">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ba6a-138">关系</span><span class="sxs-lookup"><span data-stu-id="7ba6a-138">Relationships</span></span>
<span data-ttu-id="7ba6a-139">无</span><span class="sxs-lookup"><span data-stu-id="7ba6a-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ba6a-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ba6a-140">JSON Representation</span></span>
<span data-ttu-id="7ba6a-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ba6a-141">Here is a JSON representation of the resource.</span></span>
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





