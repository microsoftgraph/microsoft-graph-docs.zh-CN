---
title: termsAndConditionsAssignment 资源类型
description: C） 到给定的组策略。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
author: tfitzmac
ms.openlocfilehash: a7b0e9deb391b9431be1ed4f282cb6e5a63ced6e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351049"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="04173-104">termsAndConditionsAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="04173-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="04173-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="04173-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04173-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="04173-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04173-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="04173-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04173-108">termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。</span><span class="sxs-lookup"><span data-stu-id="04173-108">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="04173-109">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="04173-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="04173-110">方法</span><span class="sxs-lookup"><span data-stu-id="04173-110">Methods</span></span>
|<span data-ttu-id="04173-111">方法</span><span class="sxs-lookup"><span data-stu-id="04173-111">Method</span></span>|<span data-ttu-id="04173-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="04173-112">Return Type</span></span>|<span data-ttu-id="04173-113">说明</span><span class="sxs-lookup"><span data-stu-id="04173-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="04173-114">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="04173-114">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="04173-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="04173-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="04173-116">列出 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="04173-116">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="04173-117">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="04173-117">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="04173-118">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="04173-118">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="04173-119">读取 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="04173-119">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="04173-120">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="04173-120">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="04173-121">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="04173-121">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="04173-122">创建新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="04173-122">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="04173-123">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="04173-123">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="04173-124">无</span><span class="sxs-lookup"><span data-stu-id="04173-124">None</span></span>|<span data-ttu-id="04173-125">删除 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="04173-125">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="04173-126">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="04173-126">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="04173-127">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="04173-127">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="04173-128">更新 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="04173-128">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="04173-129">属性</span><span class="sxs-lookup"><span data-stu-id="04173-129">Properties</span></span>
|<span data-ttu-id="04173-130">属性</span><span class="sxs-lookup"><span data-stu-id="04173-130">Property</span></span>|<span data-ttu-id="04173-131">类型</span><span class="sxs-lookup"><span data-stu-id="04173-131">Type</span></span>|<span data-ttu-id="04173-132">说明</span><span class="sxs-lookup"><span data-stu-id="04173-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04173-133">id</span><span class="sxs-lookup"><span data-stu-id="04173-133">id</span></span>|<span data-ttu-id="04173-134">String</span><span class="sxs-lookup"><span data-stu-id="04173-134">String</span></span>|<span data-ttu-id="04173-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="04173-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="04173-136">target</span><span class="sxs-lookup"><span data-stu-id="04173-136">target</span></span>|[<span data-ttu-id="04173-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="04173-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="04173-138">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="04173-138">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04173-139">关系</span><span class="sxs-lookup"><span data-stu-id="04173-139">Relationships</span></span>
<span data-ttu-id="04173-140">无</span><span class="sxs-lookup"><span data-stu-id="04173-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="04173-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04173-141">JSON Representation</span></span>
<span data-ttu-id="04173-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04173-142">Here is a JSON representation of the resource.</span></span>
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





