---
title: termsAndConditionsAssignment 资源类型
description: termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: db16fac75dd402fe478145834709294cfdb2060f
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179409"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="2c897-104">termsAndConditionsAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c897-104">termsAndConditionsAssignment resource type</span></span>

<span data-ttu-id="2c897-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c897-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c897-106">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2c897-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c897-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2c897-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c897-108">termsAndConditionsAssignment 实体表示对给定组的给定条款和条件 (T & C) 策略的分配。</span><span class="sxs-lookup"><span data-stu-id="2c897-108">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="2c897-109">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="2c897-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="2c897-110">方法</span><span class="sxs-lookup"><span data-stu-id="2c897-110">Methods</span></span>
|<span data-ttu-id="2c897-111">方法</span><span class="sxs-lookup"><span data-stu-id="2c897-111">Method</span></span>|<span data-ttu-id="2c897-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="2c897-112">Return Type</span></span>|<span data-ttu-id="2c897-113">说明</span><span class="sxs-lookup"><span data-stu-id="2c897-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2c897-114">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="2c897-114">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="2c897-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2c897-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="2c897-116">列出 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2c897-116">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="2c897-117">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="2c897-117">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="2c897-118">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="2c897-118">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="2c897-119">读取 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2c897-119">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="2c897-120">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="2c897-120">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="2c897-121">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="2c897-121">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="2c897-122">创建新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2c897-122">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="2c897-123">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="2c897-123">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="2c897-124">无</span><span class="sxs-lookup"><span data-stu-id="2c897-124">None</span></span>|<span data-ttu-id="2c897-125">删除 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2c897-125">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="2c897-126">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="2c897-126">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="2c897-127">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="2c897-127">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="2c897-128">更新 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2c897-128">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2c897-129">属性</span><span class="sxs-lookup"><span data-stu-id="2c897-129">Properties</span></span>
|<span data-ttu-id="2c897-130">属性</span><span class="sxs-lookup"><span data-stu-id="2c897-130">Property</span></span>|<span data-ttu-id="2c897-131">类型</span><span class="sxs-lookup"><span data-stu-id="2c897-131">Type</span></span>|<span data-ttu-id="2c897-132">说明</span><span class="sxs-lookup"><span data-stu-id="2c897-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c897-133">id</span><span class="sxs-lookup"><span data-stu-id="2c897-133">id</span></span>|<span data-ttu-id="2c897-134">字符串</span><span class="sxs-lookup"><span data-stu-id="2c897-134">String</span></span>|<span data-ttu-id="2c897-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2c897-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="2c897-136">target</span><span class="sxs-lookup"><span data-stu-id="2c897-136">target</span></span>|[<span data-ttu-id="2c897-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2c897-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2c897-138">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="2c897-138">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c897-139">关系</span><span class="sxs-lookup"><span data-stu-id="2c897-139">Relationships</span></span>
<span data-ttu-id="2c897-140">无</span><span class="sxs-lookup"><span data-stu-id="2c897-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c897-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c897-141">JSON Representation</span></span>
<span data-ttu-id="2c897-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c897-142">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```



