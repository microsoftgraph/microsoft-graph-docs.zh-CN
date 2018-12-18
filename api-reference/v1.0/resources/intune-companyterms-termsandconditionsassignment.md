---
title: termsAndConditionsAssignment 资源类型
description: C） 到给定的组策略。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
author: tfitzmac
ms.openlocfilehash: cfc38c491cc7c619dd6e3fea42fc2b1f34b20847
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311996"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="f1d6a-104">termsAndConditionsAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1d6a-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="f1d6a-105">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f1d6a-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1d6a-106">termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。</span><span class="sxs-lookup"><span data-stu-id="f1d6a-106">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="f1d6a-107">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="f1d6a-107">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="f1d6a-108">方法</span><span class="sxs-lookup"><span data-stu-id="f1d6a-108">Methods</span></span>
|<span data-ttu-id="f1d6a-109">方法</span><span class="sxs-lookup"><span data-stu-id="f1d6a-109">Method</span></span>|<span data-ttu-id="f1d6a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f1d6a-110">Return Type</span></span>|<span data-ttu-id="f1d6a-111">说明</span><span class="sxs-lookup"><span data-stu-id="f1d6a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f1d6a-112">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="f1d6a-112">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="f1d6a-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1d6a-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="f1d6a-114">列出 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f1d6a-114">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="f1d6a-115">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="f1d6a-115">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="f1d6a-116">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="f1d6a-116">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="f1d6a-117">读取 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f1d6a-117">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="f1d6a-118">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="f1d6a-118">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="f1d6a-119">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="f1d6a-119">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="f1d6a-120">创建新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f1d6a-120">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="f1d6a-121">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="f1d6a-121">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="f1d6a-122">无</span><span class="sxs-lookup"><span data-stu-id="f1d6a-122">None</span></span>|<span data-ttu-id="f1d6a-123">删除 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f1d6a-123">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="f1d6a-124">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="f1d6a-124">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="f1d6a-125">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="f1d6a-125">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="f1d6a-126">更新 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f1d6a-126">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f1d6a-127">属性</span><span class="sxs-lookup"><span data-stu-id="f1d6a-127">Properties</span></span>
|<span data-ttu-id="f1d6a-128">属性</span><span class="sxs-lookup"><span data-stu-id="f1d6a-128">Property</span></span>|<span data-ttu-id="f1d6a-129">类型</span><span class="sxs-lookup"><span data-stu-id="f1d6a-129">Type</span></span>|<span data-ttu-id="f1d6a-130">说明</span><span class="sxs-lookup"><span data-stu-id="f1d6a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1d6a-131">id</span><span class="sxs-lookup"><span data-stu-id="f1d6a-131">id</span></span>|<span data-ttu-id="f1d6a-132">String</span><span class="sxs-lookup"><span data-stu-id="f1d6a-132">String</span></span>|<span data-ttu-id="f1d6a-133">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f1d6a-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="f1d6a-134">target</span><span class="sxs-lookup"><span data-stu-id="f1d6a-134">target</span></span>|[<span data-ttu-id="f1d6a-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f1d6a-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f1d6a-136">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="f1d6a-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1d6a-137">关系</span><span class="sxs-lookup"><span data-stu-id="f1d6a-137">Relationships</span></span>
<span data-ttu-id="f1d6a-138">无</span><span class="sxs-lookup"><span data-stu-id="f1d6a-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f1d6a-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1d6a-139">JSON Representation</span></span>
<span data-ttu-id="f1d6a-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1d6a-140">Here is a JSON representation of the resource.</span></span>
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



