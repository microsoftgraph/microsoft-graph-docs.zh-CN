---
title: termsAndConditionsGroupAssignment 资源类型
description: TermsAndConditionsGroupAssignment 实体表示将给定条款和条件（T&C）策略分配给给定组。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b156b05809990b84d2fdddf71f9e307586cfc699
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42487548"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="1b8f8-104">termsAndConditionsGroupAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b8f8-104">termsAndConditionsGroupAssignment resource type</span></span>

<span data-ttu-id="1b8f8-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1b8f8-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b8f8-106">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1b8f8-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b8f8-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1b8f8-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b8f8-108">TermsAndConditionsGroupAssignment 实体表示将给定条款和条件（T&C）策略分配给给定组。</span><span class="sxs-lookup"><span data-stu-id="1b8f8-108">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="1b8f8-109">组中的用户需要接受这些条款，才能将设备注册到 Intune。</span><span class="sxs-lookup"><span data-stu-id="1b8f8-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="1b8f8-110">方法</span><span class="sxs-lookup"><span data-stu-id="1b8f8-110">Methods</span></span>
|<span data-ttu-id="1b8f8-111">方法</span><span class="sxs-lookup"><span data-stu-id="1b8f8-111">Method</span></span>|<span data-ttu-id="1b8f8-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="1b8f8-112">Return Type</span></span>|<span data-ttu-id="1b8f8-113">说明</span><span class="sxs-lookup"><span data-stu-id="1b8f8-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1b8f8-114">列出 termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="1b8f8-114">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="1b8f8-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="1b8f8-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="1b8f8-116">列出[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1b8f8-116">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="1b8f8-117">获取 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="1b8f8-117">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="1b8f8-118">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="1b8f8-118">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="1b8f8-119">读取[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1b8f8-119">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="1b8f8-120">创建 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="1b8f8-120">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="1b8f8-121">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="1b8f8-121">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="1b8f8-122">创建新的[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1b8f8-122">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="1b8f8-123">删除 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="1b8f8-123">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="1b8f8-124">无</span><span class="sxs-lookup"><span data-stu-id="1b8f8-124">None</span></span>|<span data-ttu-id="1b8f8-125">删除[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="1b8f8-125">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="1b8f8-126">更新 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="1b8f8-126">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="1b8f8-127">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="1b8f8-127">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="1b8f8-128">更新[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1b8f8-128">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1b8f8-129">属性</span><span class="sxs-lookup"><span data-stu-id="1b8f8-129">Properties</span></span>
|<span data-ttu-id="1b8f8-130">属性</span><span class="sxs-lookup"><span data-stu-id="1b8f8-130">Property</span></span>|<span data-ttu-id="1b8f8-131">类型</span><span class="sxs-lookup"><span data-stu-id="1b8f8-131">Type</span></span>|<span data-ttu-id="1b8f8-132">说明</span><span class="sxs-lookup"><span data-stu-id="1b8f8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b8f8-133">id</span><span class="sxs-lookup"><span data-stu-id="1b8f8-133">id</span></span>|<span data-ttu-id="1b8f8-134">String</span><span class="sxs-lookup"><span data-stu-id="1b8f8-134">String</span></span>|<span data-ttu-id="1b8f8-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1b8f8-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="1b8f8-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="1b8f8-136">targetGroupId</span></span>|<span data-ttu-id="1b8f8-137">String</span><span class="sxs-lookup"><span data-stu-id="1b8f8-137">String</span></span>|<span data-ttu-id="1b8f8-138">向其分配 T&C 策略的组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1b8f8-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b8f8-139">关系</span><span class="sxs-lookup"><span data-stu-id="1b8f8-139">Relationships</span></span>
|<span data-ttu-id="1b8f8-140">关系</span><span class="sxs-lookup"><span data-stu-id="1b8f8-140">Relationship</span></span>|<span data-ttu-id="1b8f8-141">类型</span><span class="sxs-lookup"><span data-stu-id="1b8f8-141">Type</span></span>|<span data-ttu-id="1b8f8-142">说明</span><span class="sxs-lookup"><span data-stu-id="1b8f8-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b8f8-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="1b8f8-143">termsAndConditions</span></span>|[<span data-ttu-id="1b8f8-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="1b8f8-144">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="1b8f8-145">所分配的条款和条件的导航链接。</span><span class="sxs-lookup"><span data-stu-id="1b8f8-145">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b8f8-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b8f8-146">JSON Representation</span></span>
<span data-ttu-id="1b8f8-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b8f8-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```



