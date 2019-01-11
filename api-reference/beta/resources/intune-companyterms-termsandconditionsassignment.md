---
title: termsAndConditionsAssignment 资源类型
description: C） 到给定的组策略。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ce4a1d77f3a3db1f1faee94c5435730515ff6af6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875059"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="06ee4-104">termsAndConditionsAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="06ee4-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="06ee4-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="06ee4-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06ee4-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="06ee4-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06ee4-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="06ee4-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06ee4-108">termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。</span><span class="sxs-lookup"><span data-stu-id="06ee4-108">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="06ee4-109">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="06ee4-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="06ee4-110">方法</span><span class="sxs-lookup"><span data-stu-id="06ee4-110">Methods</span></span>
|<span data-ttu-id="06ee4-111">方法</span><span class="sxs-lookup"><span data-stu-id="06ee4-111">Method</span></span>|<span data-ttu-id="06ee4-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="06ee4-112">Return Type</span></span>|<span data-ttu-id="06ee4-113">说明</span><span class="sxs-lookup"><span data-stu-id="06ee4-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="06ee4-114">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="06ee4-114">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="06ee4-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06ee4-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="06ee4-116">列出 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="06ee4-116">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="06ee4-117">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="06ee4-117">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="06ee4-118">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="06ee4-118">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="06ee4-119">读取 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="06ee4-119">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="06ee4-120">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="06ee4-120">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="06ee4-121">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="06ee4-121">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="06ee4-122">创建新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06ee4-122">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="06ee4-123">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="06ee4-123">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="06ee4-124">无</span><span class="sxs-lookup"><span data-stu-id="06ee4-124">None</span></span>|<span data-ttu-id="06ee4-125">删除 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="06ee4-125">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="06ee4-126">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="06ee4-126">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="06ee4-127">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="06ee4-127">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="06ee4-128">更新 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="06ee4-128">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="06ee4-129">属性</span><span class="sxs-lookup"><span data-stu-id="06ee4-129">Properties</span></span>
|<span data-ttu-id="06ee4-130">属性</span><span class="sxs-lookup"><span data-stu-id="06ee4-130">Property</span></span>|<span data-ttu-id="06ee4-131">类型</span><span class="sxs-lookup"><span data-stu-id="06ee4-131">Type</span></span>|<span data-ttu-id="06ee4-132">说明</span><span class="sxs-lookup"><span data-stu-id="06ee4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06ee4-133">id</span><span class="sxs-lookup"><span data-stu-id="06ee4-133">id</span></span>|<span data-ttu-id="06ee4-134">String</span><span class="sxs-lookup"><span data-stu-id="06ee4-134">String</span></span>|<span data-ttu-id="06ee4-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="06ee4-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="06ee4-136">target</span><span class="sxs-lookup"><span data-stu-id="06ee4-136">target</span></span>|[<span data-ttu-id="06ee4-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="06ee4-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="06ee4-138">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="06ee4-138">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06ee4-139">关系</span><span class="sxs-lookup"><span data-stu-id="06ee4-139">Relationships</span></span>
<span data-ttu-id="06ee4-140">无</span><span class="sxs-lookup"><span data-stu-id="06ee4-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="06ee4-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06ee4-141">JSON Representation</span></span>
<span data-ttu-id="06ee4-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06ee4-142">Here is a JSON representation of the resource.</span></span>
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





